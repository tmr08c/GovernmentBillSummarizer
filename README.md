# GovernmentBillSummarizer

Use NLP to classify and summarize bills available through the [govinfo API](https://api.govinfo.gov/docs/).

## Using

To run program correctly, the program must be initialized by running `UserInterface.py`:

```bash
python UserInterface.py
```

### Additional Notes

- For *package bills*, the government api sorts these by *upload date* and not issue date.

  If you are searching for a bill from a certain date, this will not find it, you must use general bills.

  General bills can be searched by bill issue/creation date.

- Some very large bills summaries take a few minutes to load, if it seems like the program hangs up, it is probably loading a summary so be patient.

- Some summaries have repeated sentences, this is a known issue, and is due to quirks in the .gov api.

- All folder's (train and test folder) must remain in their location. They must be in the working directory for the program to work as intended.

## Development

### Dependencies

This project relies on the following packages:

- Gensim
- numpy
- asciiplotlib
- matplotlib
- json
- requests
- datetime
- math
- os
