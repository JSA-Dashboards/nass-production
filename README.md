# JSA NASS Production

USDA NASS production by state, ASD district and county: the first tab of the RMA dashboard as its own app.

**This folder is generated.** `app.py` is produced by `sync_nass_mirror.py` in `JSA-Dashboards/rma-production-map` from that dashboard's `app.py`; change the NASS tab there and run the sync, do not edit here.

    streamlit run app.py

Secret needed: `NASS_API_KEY` (Streamlit Cloud: Settings > Secrets). County boundaries come from a public URL; there is no database.
