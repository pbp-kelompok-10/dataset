Dataset untuk tugas kelompok PBP

dataset menggunakan format json

Teams : Dataset untuk teams : (negara)</br>
Players : Dataset untuk pemain : (nama, asal negara, umur, nomor baju, tim)</br>
Rounds : dataset untuk hasil dari ronde-ronde sebelumnya (ambil dari https://www.fifa.com/en/tournaments/mens/worldcup/canadamexicousa2026/qualifiers/afc/scores-fixtures?country=ID&wtw-filter=ALL)
(skor, tempat, tim, lineup (pemain dan posisi))`

Template json :

`Teams` (penamaan : `<negara>.json`, Contoh : `indonesia.json`)
```json
{
    "negara" : <negara>
}
```

`Players` (penamaan : `player_<tim>.json`, Contoh : `player_indonesia.json`)
```json
{
    {
    "nama" : <nama>,
    "asal" : <asal_negara>,
    "umur" : <umur>,
    "nomor" : <nomor_baju>,
    "tim" : <tim> (sesuain sama Teams, contoh: Indonesia)
    },
    dst
}
```

`Rounds` (penamaan: `round_<no>.json`, contoh: `round_1.json`)
```json
{
    {
    "tempat" : <tempat>,
    "tim1" : <tim1>,
    "tim2" : <tim2>,
    "skor1": <skor tim 1>,
    "skor2": <skor tim 2>,
    "lineup" : {
        <nama> : <posisi>
        dst
    }
    },
    dst
}
```

`