# CTCAE code server experiment
Experiments regarding Common Terminology Criteria for Adverse Events (CTCAE)

The original files and info about CTCAE can be found at https://ctep.cancer.gov/protocoldevelopment/electronic_applications/ctc.htm

Process used to create a JSON file and providing it via a API for testing (not for production use).

1. The file Excel file for CTCAE Version 5.0 https://ctep.cancer.gov/protocoldevelopment/electronic_applications/docs/CTCAE_v5.0.xlsx was downloeded and opened in a spreadsheet program.
2. Change the header of first column from `MedDRA Code` to `id`
3. Select and copy columns A throug J
4. Paste into https://csvjson.com/csv2json and convert
5. Download resulting file and add surrunding DB structure plus acces via URL as described at https://my-json-server.typicode.com/
6. Access (for testing, not for production use) via the described URL-patterns. For my particular example repo that would be https://my-json-server.typicode.com/ErikSundvall/ctcae/medra_code/{add_code_here} for example looking up "Fatigue" by it's code https://my-json-server.typicode.com/ErikSundvall/ctcae/medra_code/10016256 



