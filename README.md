# Quadpass---newer-RNG

QuadPass - (c) 2021 Rich Amies  
Licensed under the GPLv3 - https://www.gnu.org/licenses/gpl-3.0.en.html  
This program comes with ABSOLUTELY NO WARRANTY.  
This is free software, and you are welcome to redistribute it under certain conditions.
    
QuadPass - a QUick And Dirty Passphrase generator using EFF wordlists.  
https://www.eff.org/files/2016/09/08/eff_short_wordlist_2_0.txt
    
This is just a simple passphrase generator I made when learning a little about C#.  Uses the more secure RNG:  
https://docs.microsoft.com/en-us/dotnet/api/system.security.cryptography.rngcryptoserviceprovider?view=net-5.0

'Rolls' 4 dice for each word, as-per the EFF:  
https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases

Would be quicker if it didn't make multiple RNG calls per-word - but I wanted to follow the overall approach.  The RNG may appear unbalanced, or biased - there are four very high word count options that may be selected to give the user peace of mind that, in fact, the numbers generated are quite evenly spread when meaesured over a larger range.