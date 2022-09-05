# Numeral-decomposer-1.0

We present a performance analysis of a numeral decomposer.

From the languages accessible in https://www.languagesandnumbers.com/site-map/en/ we parsed all numerals up to 1000, and from the languages accesible in https://pypi.org/project/num2words/ we parsed numerals up to 1000 and a sample of numerals up to 27206.

For each language we display the quantity of different functions found and the quantity of irreducible numerals, i.e. numerals that could not be decomposed. The sum of these numbers is the size of a possible lexicon that could generate all the included numerals of the respective language. The languages from num2words are listed first and are only named as 2-letter-abbreviations (e.g. cz=Czech). Below, the Languages&Numbers-languages are listed with their full English term.

Below the quantities we present each found funtions by displaying 3 properties of it:

1) Its string function: The '\_'s in the string represent the input slots of the function, e.g. putting (six,two) into \_ty-\_ gives sixty-two
2) Its number function in format: coefficient-vector*x+constant. x represents a vector of variables with the same size as coefficient-vector. E.g. the function \_ty-\_ would have the number function [10,1]x+0, so a possible input x would also have to be a vector of size 2, as [6,2] is. OTOH the function \_teen with the number function [1]x+10 would only accept single numbers as inputs.
3) An example of a generated numeral with its number. Wording: e.g. sixty-one is 61.
