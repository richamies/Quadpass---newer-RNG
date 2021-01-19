# Quadpass---newer-RNG

__QuadPass - (c) 2021 Rich Amies  
Licensed under the GPLv3 - https://www.gnu.org/licenses/gpl-3.0.en.html  
This program comes with ABSOLUTELY NO WARRANTY.  
This is free software, and you are welcome to redistribute it under certain conditions.__  

Download the release ZIP from here: https://github.com/richamies/Quadpass---newer-RNG/releases  
__Uses Microsoft .NET 5.0 runtimes - should prompt to download if not already installed.__  
    
QuadPass - a QUick And Dirty Passphrase generator using EFF wordlists.  
https://www.eff.org/files/2016/09/08/eff_short_wordlist_2_0.txt
    
This is just a simple passphrase generator I made when learning a little about C#.  Uses the more secure RNG:  
https://docs.microsoft.com/en-us/dotnet/api/system.security.cryptography.rngcryptoserviceprovider?view=net-5.0

'Rolls' 4 dice for each word, as-per the EFF:  
https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases

Would be quicker if it didn't make multiple RNG calls per-word - but I wanted to follow the overall approach.  The RNG may appear unbalanced, or biased - there are four very high word count options that may be selected to give the user peace of mind that, in fact, the numbers generated are quite evenly spread when meaesured over a larger range.

I'm sure this can be done better.  I'm no programmer(which ought to be obvious!), and I was just looking to write/learn something one wet afternoon.  It's here as I thought it may be of use to someone wanting a simple offline passphrase generator.
