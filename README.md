<!-- วิธีเพิ่มสี
1. add ค่า columnSetting : {fille am5.color(ค่าสี)} ลงใน data json
Ex.

for (var i = 0; i < data.length; i++) {
    if (data[i].value > 500) {
        data[i] = {
            ...data[i],
            columnSettings: {
                fill: am5.color(0xdc4534)
            }
        };
    } else if (data[i].value > 300) {
        data[i] = {
            ...data[i],
            columnSettings: {
                fill: am5.color(0xd7a700)
            }
        };
    }
    else{
        data[i] = {
            ...data[i],
            columnSettings: {
                fill: am5.color(0x68ad5c)
            }
        };
    }

}

2.
series.slices.template.setAll({
    templateField: "columnSettings"
}); ต้องทำก่อน adddata ลง series

3.
series.data.setAll(data);
 -->
