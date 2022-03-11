import argparse

import string

import random


parser = argparse.ArgumentParser

args = parser.parse_args()


openWordTxt = open(word.txt)

wordTxt = openWordTxt.read().splitlines()

wordSS = random.sample(wordTxt, args.words)

capitalList = [], capitalNumber = 0

if 0 < args.capital <= args.words:
    string.capitalize()
    capitalSS = random.sample(wordSS, args.capital)
    wordSS = list((wordSS) - (capitalSS))
    while  args.capital > args.capitalNumber:
        capitalList.extend(capitalSS)
        capitalNumber += 1

    wordSS = wordSS + capitalList

    random.shuffle(wordSS)


numberList = [], numberNumber = 0

if args.numbers > 0:
    while args.numbers > numberNumber:
        temporaryList = [str(random.randint(0, 9))]
        numberList = numberList + temporaryList
        numberNumber += 1

    wordSS = wordSS + numberList
    
    random.shuffle(wordSS)


if args.symbols > 0:
    symbolList = ["!", "@", "#", "%", "$", "^", "&", "*", "_", "-", "+", ":", ";", "/", "?", "~"]
    symbolSS = random.sample(symbolList, args.symbols)
    symbolNumber += 1

    wordSS = wordSS + symbolSS
    
    random.shuffle(wordSS)

parser.add_argument("-h", "--help", int=0, "Show this help message and exit")

parser.add_argument("-w WORDS", "--words", type=int, help="Include WORDS words in the password", default=4)

parser.add_argument("-c CAPS", "--caps", type=int, help="Capitalize the first letter of CAPS random words",
                    default=0)
                    
parser.add_argument("-n NUMBERS", "--numbers", type=int, help="Insert NUMBERS random numbers in the password",
                    default=0)

parser.add_argument("-s SYMBOLS", "--symbols", type=int, help="insert SYMBOLS random symbols in the password",
                    default=0)

password = "".join(wordSS)

print(password)


