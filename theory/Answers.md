1. Regular Expressions: Antelopes

    * Single Regex matching 'antelope' and 'antelopes': 
    
    /antelopes?/g

    * Matching both 'antelope rocks out' and 'antelopes rock out': 
    
    /antelopes?\srocks?\sout/g

2. Regular Expressions: Goats and Moats and Boats

    * Regex matching either 'goat' or 'moat' but not' boat':

    /[gm]oat/g

3. Regular Expressions: Dates

    * Regex matching dates in YYYY-MM-DD format:

    /\d{1,4}-\d{1,2}-\d{1,2}/g

-----------------------------

1. State Machine
    * VT-100 Regex

        /\e\[(1m)?(\d{1,2};\d{1,2}f)?/gi
