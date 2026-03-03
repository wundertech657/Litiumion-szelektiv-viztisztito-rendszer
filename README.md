# Litiumion-szelektiv-viztisztito-rendszer
## 2026. március 1.
Ma dolgoztunk a vízpumpa projekten. A projektet azzal kezdtük, hogy bekötöttük a hőmérséklet‑érzékelőt az ESP32 5-ös lábára. Az 5-ös láb analóg bemenet. Ezután a pumpa kapcsolóját a 7-es lábra kötöttük, ami digitális kimenet. Ezután egy nyomógombot kötöttünk a 13-as lábra és a földre, hogy egy reteszelő áramkört alakítsunk ki.
A kódot C++ nyelven írtuk az ESP32‑WROOM számára. A soros monitorhoz 115200-as baud rátát választottunk. Hozzáadtunk egy 50 milliszekundumos késleltetést a gombzaj kiszűrésére, hogy a kapcsoló megbízhatóan működjön. A kód beolvassa a hőmérséklet‑érzékelő analóg feszültségét, Celsius-fokra alakítja, és két másodpercenként kiírja. A gomb megnyomására a pumpa állapotát is átváltja.
A projekt most már működőképes. Az érzékelő olvassa a hőmérsékletet. A gomb ki‑ és bekapcsolja a pumpát. A soros monitor pedig a kívánt módon jeleníti meg az adatokat.
