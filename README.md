## Instructions

To produce the various files, run the following commands:

Create options file from hand (see docs)

Create the classifications.json with this command:
anonymize classify --database-engine SqlServer --connection-string "Server=<<SERVER>>; Database=<<Database>>; Integrated Security=true; TrustServerCertificate=true" --classification-file classification.json

Create the masking.json file with this command
anonymize map --classification-file classification.json --masking-file masking.json --options-file options.json