# Sức Mạnh cơ bản

Sức mạnh cơ bản là các chỉ số của một Elf trong chiến đấu. Mỗi Elf gồm có 15 chỉ số sức mạnh, gồm có HP, ATK, SPE, ADF, CRE, CRI, DAM, ARM, HIT, AGI, INT, STA, STR, POT, EAV.

| Tên ngắn | Tên đầy đủ          | Tên việt nam           |
| -------- | ------------------- | ---------------------- |
| ATK      | Attack Power        | Sát Thương Vật Lý      |
| HP       | Hit Points          | Điểm Sinh Lực          |
| POT      | Potential           | Điểm Tiềm Năng         |
| STA      | Stamina             | Bền Bỉ                 |
| _+sta_   | Stamina Growth      | Tăng trưởng bền bỉ     |
| STR      | Strength            | Lực Lượng              |
| _+str_   | Strength Growth     | Tăng trưởng lực lượng  |
| AGI      | Agility             | Nhanh Nhẹn             |
| _+agi_   | Agility Growth      | Tăng trưởng nhanh nhẹn |
| INT      | Intelligence        | Trí Lực                |
| _+int_   | Intelligence Growth | Tăng trưởng trí lực    |
| DAM      | Damage              | Sát Thương             |
| ADF      | Magic Defense       | Kháng Phép             |
| ARM      | Armor               | Hộ Giáp                |
| CRE      | Critical Resistance | Kháng Bạo Kích         |
| CRI      | Critical            | Bạo Kích               |
| EVA      | Vasion              | Né Tránh               |
| HIT      | Hit                 | Đánh Chính Xác         |
| SPE      | Speed               | Tốc Độ                 |

$$
HP=STA*10
$$

HP = STA\*10

ATK = DAM\*1 + ADF\*1 + ARM\*1 + HP\*0.1 + SPE\*1 + HIT\*2 + EVA\*2.4 + CRI\*2 + CRE\*2

#### Growth formula，about STA ， STR ， AGI ， INT  :&#x20;

$$
f(x) =n (x -1)* 1.17^{ i*4}+N
$$

x=Level

i=Number of Evolution

N=( STA / STR / AGI / INT )

n=( _+sta / +str / +agi / +int_ )
