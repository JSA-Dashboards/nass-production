# JSA NASS Production

USDA NASS production by state, ASD district and county: the first tab of the RMA dashboard as its own app.

**This folder is generated.** `app.py` is produced by `sync_nass_mirror.py` in `JSA-Dashboards/rma-production-map` from that dashboard's `app.py`; change the NASS tab there and run the sync, do not edit here.

    streamlit run app.py

NASS data comes from the shared cache that `usda-nass-etl` fills, so the app needs the Snowflake secrets (`USE_SNOWFLAKE`, `SNOWFLAKE_ACCOUNT`, `SNOWFLAKE_USER`, `SNOWFLAKE_PRIVATE_KEY`, `SNOWFLAKE_ROLE`, `SNOWFLAKE_WAREHOUSE`; Streamlit Cloud: Settings > Secrets). `NASS_API_KEY` is only a fallback while the cache fills: leave it out and the app reads the cache alone. County boundaries come from a public URL.
