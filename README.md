# Json
data exchange format

// 2 struktury json

{} 

{
    "name": "Karo",
    "surname": "Szyszka",
    "age": 30,
    "city": "",
    "isProgrammer": true,
    "addresses": {
        "street": "",
        "school": "",
        "work": ""
    },
    "hobbies": ["snowboard", "ski", "thai chi"],
    "animals": null

}

// pojedynczy, bez przecinkow na koncu
// 1 obiekt lub tablica
// male litery tylko
// nie ma komentarzy xp

///
[] 

["value1, value2,value3"]


// typy:
- string (text)
- number - bez cudzyslowia
- boolean
- obiekt
- tablica
- null

//Json 
- uzywany w npm 
- plik konfiguracyjny 

//a jak sa przesylane? 

- musi byc zmieniony na tekst, zeby mozna bylo go odczytac prawidlowo przez inne jezyki. odpowiednie formatowanie
dla innych jezykow. sformatowanie zdatne dla inncyh - zwykly text
w consoli mozna zmienic

=> JSON.stringify () - tekst mozna wyslac przez api, wyslac do innego systemu, zapisac w lokalnie, zapisac w bazie danych 

'{"name":"Karo","surname":"Szyszka","age":30,"city":"","isProgrammer":true,"addresses":{"street":"","school":"","work":""},"hobbies":["snowboard","ski","thai chi"],"animals":null}'

//mozna przypisywac i zapamietywac w pamieci takiego json z danymi poprzez zmienna np. 
const jsonText = JSON.stringify ({
    "name": "Karo",
    "surname": "Szyszka",
    "age": 30,
    "city": "Wroc",
    "isProgrammer": true,
    "addresses": {
        "street": "",
        "school": "",
        "work": ""
    },
    "hobbies": ["snowboard", "ski", "thai chi"],
    "animals": null

})

jsonText cklick i w consoli mamy zapamietany string

mozna go parsowac czyli przetwarz z tekstu na obiekt 

JSON.parse(jsonText)
