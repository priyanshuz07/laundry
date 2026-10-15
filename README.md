# FreshWash Laundry

FreshWash Laundry is a browser-based laundry management demo. It runs locally without a build step, backend, account, or paid service. Customer, order, rack, stage, and payment data are stored in the browser's `localStorage`.

## Run locally

1. Install Python 3 if it is not already available.
2. Open PowerShell in this folder.
3. Run:

   ```powershell
   python -m http.server 8765
   ```

4. Open <http://localhost:8765/> in a browser.
5. Stop the server with `Ctrl+C` when finished.

You can also open `index.html` directly in a modern browser. Using the local server is recommended for consistent browser storage and print behavior.

## Demo data and reports

The first visit seeds 20 example orders for Indian customers across laundry stages, storage locations, delivery dates, and payment statuses. Changes are saved in that browser on that device. Use **Reports → Reset Demo Data** to restore the original examples; this replaces all saved demo records in the current browser after confirmation.

Reports filter orders by received date and collections by payment date. Outstanding balances are calculated for orders received in the selected period. Use the report export buttons for order and payment CSV files; the Orders and Payments pages also provide their respective exports.

## Limitations

- This is a local demo, not a multi-user or cloud-synced service. Browser data is not automatically backed up.
- There is no authentication, role-based access, payment gateway, SMS, or external API integration.
- Business address and mobile details on printed documents are placeholders to be replaced with actual shop details.
