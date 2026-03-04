# hledger-webuix
web interface for editing/reporting a hledger plain text accounting file. 

This is a single file HTML file that provides a web interface for hledger. Load the file in your browser, throw in your ledger data file and you get three tabs:

- one tab for the transactions. You can edit and append transactions
- one tab for the balance sheet
- one tab for the P&L.

That's it. Super simple, should be self-explanatory.

Please note:
- I am in Europe and my ledger data files use 'EUR' as the currency symbol. There is a test ledger file bcexample.hledger available at https://github.com/simonmichael/hledger/blob/master/examples/bcexample.hledger, that files has 'USD' as currency. hledger-webuix seems to eat this file without any complaints, but in the presentation then it shows EUR instead of USD. The amounts seem to be correct, but still may need some work here...
- I have not implemented multi-currency.
- my accounts start with ass: lia: inc: exp. I am not sure if that is standard hledger lingo, but it is what I use at the moment. I may need to change that for others to use this web-interface, not sure.
- my dates are in 2026/01/31 format. I don't think my regexp parses other formats.
- functionality is limited, hledger CLI provides more functionality.

So more work may be required to make this a useful tool for other people. For now you're free to try and leave comments.

<img width="1497" height="958" alt="Screenshot 2026-03-04 195250" src="https://github.com/user-attachments/assets/a52e6368-3fae-4abe-9e45-07e6114db6dd" />

Final note: No I am NOT a programmer. I have some basic knowledge of Javascript and Python and Pascal and stuff like that, but I am not a programmer. This web interface I built just by talking to Claude at claude.io. Amazing tool!
