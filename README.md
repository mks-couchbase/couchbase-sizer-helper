# couchbase-sizer-helper

The purpose of this tool is to simplify the sizing of a couchbase cluster using our internal tools. The output from Nutshell is the input for this tool and the out from this tool is a loadable sizing calculation that can be used with the online sizing calculator.

# Code base is found:
Github location: https://github.com/mminichino/couchbase-sizer-helper

# Setup / Install on MacOS (Ventura):
1. Clone the git repo
    1. Git clone https://github.com/mminichino/couchbase-sizer-helper.git
2. Run setup
    1. ./setup.sh
    2. Password: <this is the password for th emachin
    3. Creating virtual environment... Done.
    4. Activating virtual environment... Done.
    5. Installing dependencies... Done.
    6. Setup successful.

# Using the tool:

From the couchbase-sizer-helper folder, the command to run the input and output
                       
bin/create-config -i 'SOURCE-FILE' -o 'OUTPUT-FILE'

'SOURCE-FILE' : this is the JSON file output from the tar.gz emitted from the nutshell script run by Lumberjack (decompress the file to get to the JSON file. Usually named: sizing-analysis-<TIMESTAMP>.json
'OUTPUT-FILE': this is the name of the file you want emitted from the process, such as customer-name-sizing-<date>.json

That's it.
