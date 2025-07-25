# C++ RPG Game Project

Sebuah game RPG sederhana yang dibuat dengan bahasa pemrograman C++. Game ini menampilkan sistem pertarungan turn-based, sistem leveling, dan penyimpanan progress permainan.

## Deskripsi

Game RPG ini memungkinkan pemain untuk:

- Membuat karakter dengan memilih nama dan class
- Bertarung melawan berbagai jenis monster
- Mendapatkan experience points (EXP) dan gold
- Melakukan leveling up
- Menyimpan dan memuat progress permainan
- Menyembuhkan karakter dengan gold

## Fitur Game

### Character Classes

| Class   | Damage | Health | Deskripsi                               |
| ------- | ------ | ------ | --------------------------------------- |
| Warrior | 5      | 150    | Tanky fighter dengan health tinggi      |
| Rogue   | 10     | 75     | High damage dealer dengan health rendah |
| Archer  | 7      | 100    | Balanced character                      |

### Monster Types

| Monster | Damage | Health | Reward           |
| ------- | ------ | ------ | ---------------- |
| Goblin  | 5      | 20     | 10 EXP + 5 Gold  |
| Orc     | 3      | 25     | 12 EXP + 7 Gold  |
| Wizard  | 10     | 15     | 15 EXP + 10 Gold |

### Game Systems

- Turn-based Combat: Pemain dan monster bergantian menyerang
- Leveling System: Setiap 100 EXP = naik 1 level
- Healing System: Bayar 20 gold untuk full heal
- Save/Load: Progress tersimpan di file `account.txt`

## Cara Bermain

1. Start Game: Pilih "Start New Game" atau "Continue Game"
2. Character Creation:

- Masukkan nama karakter
- Pilih class (Warrior/Rogue/Archer)

3. Main Menu:

- Fight: Pilih monster untuk dilawan
- Heal: Sembuhkan karakter (cost: 20 gold)
- Save: Simpan progress
- Quit: Keluar game

### Combat System

- Pilih "Attack" untuk menyerang monster
- Pilih "Run" untuk kabur dari pertarungan
- Jika menang: dapatkan EXP dan Gold
- Jika kalah: kehilangan semua EXP dan Gold, health direset

## Technical Details

### Data Structures

- `classes`: Struktur untuk class karakter
- `monster`: Struktur untuk data monster
- `character`: Struktur untuk data pemain

### Key Functions

- `newGame()`: Inisialisasi karakter baru
- `loadAccount()` & `saveAccount()`: Load/save progress
- `fight()`: Sistem pertarungan
- `heal()`: Sistem penyembuhan

## Known Issues

- Game hanya bisa berjalan di Windows (karena `system("cls")`)
- Input validation terbatas
- File `account.txt` harus dihapus manual untuk reset complete

## License

Project ini dibuat untuk tujuan pembelajaran. Feel free to use and modify!

## Author

**dickyhaa** - [GitHub Profile](https://github.com/dickyhaa)

---

Jangan lupa berikan star jika project ini membantu Anda!
