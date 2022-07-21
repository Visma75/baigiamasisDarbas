
# Nuoroda į testuojamą puslapį:

https://www.saucedemo.com/

# Testų scenarijų ir jų žingsnių aprašymai:

**Launch** - Tikrina ar pasileidžia puslapis
	
**testLogInGood**- Tikrina ar pavyksta prisijungti naudotojui (paskyra kurioje viskas veikia)

	suvedami prisijungimo duomenys ir paspaudžiamas "Login" mygtukas
	usr: standard_user
	pass: secret_sauce
	
	
**testLogInBad** -  Tikrina ar pavyksta prisijungti naudotojui (paskyra kurioje yra klaidų)
		
	suvedami prisijungimo duomenys ir paspaudžiamas "Login" mygtukas
	usr: problem_user
	pass: secret_sauce
		
		
**testAddProductToCart** - Tikrina ar produktas įsideda į krepšelį

	 Pridedami trys produktai paspaudžiant "Add to cart" ir žiūrima į ženkliuką prie krepšelio (ar didėja))
	
**testRemoveProductFromCartInProducts** - Tikrina ar produktas pasišalina iš krepšelio (produktų lange)

	 Pašalina produktą paspaudžiant "Remove" mygtuką ir žiūrima į ženkliuką prie krepšelio (ar mažėja))
	
**testRemoveProductFromCartInCart** - Tikrina ar produktas pasišalina iš krepšelio (krepšelio lange)

	 Pašalina produktą paspaudžiant "Remove" mygtuką ir žiūrima į ženkliuką prie krepšelio (ar mažėja))
	
	
**testCheckoutInformation** - Tikrina ar tvarkingai susiveda naudotojo informacija

	 Suvedamas vardas, pavardė ir pašto kodas, paspaudžiamas mygtukas "Checkout".
	
**testCheckout** - Tikrina ar pavyksta užbaigti pirkimą

	 Spaudžiant mygtuką "Finish" turi dingti produktai iš krepšelio ir rodyt "order colmplete"

---

**TestaiRunGeri.xml**
naudoja metodus:

					Launch
					testLogInGood
					testAddProductToCart
					testRemoveProductFromCartInProducts
					testRemoveProductFromCartInCart
					testCheckoutInformation
					testCheckout
Šiame scenarijuje praeinama viskas nuo prisijungimo iki atsiskaitymo (Turi viskas būti sėkminga)

---
**TestaiRunBlogi.xml**
naudoja metodus:

					Launch
					testLogInBad
					testAddProductToCart
					testRemoveProductFromCartInProducts
					testRemoveProductFromCartInCart
					testCheckoutInformation
					testCheckout
					
Šiame scenarijuje praeinama viskas nuo prisijungimo iki atsiskaitymo naudojant sugadintą paskyrą (Turi testas mesti klaidas ir daryti screenshots)

---