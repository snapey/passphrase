# passphrase
Utility class to provide strings of short, easy to type words

It has Laravel dependencies since it uses the Cache facade to remember the array of parsed words.

## Usage
- Create a folder within app called `Utility`
- Place PassPhrase.php and wordlist.txt in this folder
- Call the passPhrase() function with the number of words and an optional seperator

### Tinker;
```
Psy Shell v0.10.4 (PHP 7.3.11 — cli) by Justin Hileman
>>> (new App\Utility\PassPhrase)->passPhrase(4)
=> "magnum-elbow-ramp-lend"
>>> (new App\Utility\PassPhrase)->passPhrase(3,'_')
=> "fifth_stunt_adept"
>>> (new App\Utility\PassPhrase)->passPhrase(6,' - ')
=> "clip - engine - concur - club - hurry - noon"
>>> 
```
