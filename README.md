# Втора лабараториска вежба по Софтверско инженерство
## Стефан Стојанов, бр. на индекс 222062
### Control Flow Graph
![CFG](https://github.com/Stefkjo/Test/assets/138608772/bc69f023-3d95-454d-9dd0-3d3f6615337d)
 <br />
### Цикломатска комплексност 
Цикломатската комплексност на овој код е 10, каде што ја добив со формулата P + 1, каде P е број на предикатни јазли во овој случај 9 + 1 = 10. <br />
### Тест случаи според критериумот Every brach
1. if(allitems == null) <br />
checkCart(null, 350); <br />
2. if (item.getName() == null || item.getName().length() == 0) <br />
Item = (null,"3456789", 100, 0) <br />
checkCart(items, 150)
3. if (item.getBarcode() != null) <br />
Item = ("Mleko","null", 200, 0) <br />
checkCart(items, 2500) <br />
4. if (allowed.indexOf(c) == -1) <br />
Item = ("Leb", "123C567", 200, 0) <br />
checkCart(items, 350); <br />
5. if (item.getDiscount() > 0) <br />
Item = ("Kaskaval", "123123123", 450, 0.15) <br />
checkCart(items, 500) <br />
6. if (item.getBarcode().charAt(0) == '0') <br /> 
Item = ("Penkalo", "456456456", 800, 0.35) <br />
checkCart(items, 500) <br />
7. if (sum <= payment) <br />
Item = ("Orbit", "11111111", 50, 0) <br />
checkCart(items, 60) <br />
8. if (sum > payment) <br />
Item = ("Laptop", "888888", 100000, 0.20) <br />
checkCart(items, 60000) <br />
### Тест случаеви според критериумот Multiple Condition
1. Item = ("List", "01234560", 400, 0.15) True, True, True <br />
2. Item = ("Pizza", "0101010101", 500, 0) True False ... <br />
3. Item = ("Sladoled", "123123123", 320, 0.1) True True False <br />
4. Item = ("Pivo", "0123123", 150, 0) False ... ... <br />
Со првите 8 тест примери се изминуваат сите гранки (4), вторите 4 тест примери се разгледуваат сите опции, бидејќи има логички оператор && не се разгледуваат другите услови доколку еден од условите е False. 


