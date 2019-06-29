# Google API object generator
Given a Google API discovery document and an object name, generates a JSON that follows the object description

## Usage

    ./genObject.py <discovery document> <object name>

## Example

    wget -O discovery.json 'https://iam.googleapis.com/$discovery/rest'
    ./genObject.py discovery.json ServiceAccount > serviceAccount.json

## Notes

 * "_Oneof_" properties cannot be recognized by the script, they need to be removed from the result by hand
