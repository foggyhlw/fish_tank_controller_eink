# fish_tank_controller_v3.0
# 使用方法
- 将fonts文件夹复制到esphome的根文件夹（homeassistant系统中为config/esphome)
- 在esphome插件页面点击"+ NEW DEVICE" ,起一个名字，芯片选择esp32,然后跳过
- 选择EDIT进入yaml编辑器，将fish-tank-controller-epaper-v30.yaml中内容复制到编辑器中，点击install，esphome就会自行编译，得到bin文件可以同时esphome的网页烧录器进行烧录，也可以直接使用仓库中提供的fish-tank-controller-epaper-v30.bin文件直接进行烧录
# 硬件说明
- 本工程提供了立创eda专业版工程文件，可以直接导入
- 墨水屏驱动板采用的是开源硬件，作者“冰凌玛特”，https://oshwhub.com/lingdy2012/mo-shui-ping-tong-yong-zhuan-jie-ban-_0603_wos_v0-1
# 部分硬件参考链接
- 本工程中部分硬件采用现有模块，本人购买链接参考：
1. 220V转12V电源模块：https://item.taobao.com/item.htm?_u=g8a9787df95&id=570474888227&spm=a1z09.2.0.0.38222e8dypQl5e&skuId=4305412474565
2. 按键开关：https://item.taobao.com/item.htm?_u=g8a9787bf62&id=613800730809&spm=a1z09.2.0.0.38222e8dypQl5e&skuId=4318215092546

# 软件修改
- 控制板的pwm输出通过较长的排线连接至强电板，受电容效应pwm频率不能太高，本工程中pwm频率定为100Hz，已经可以满足普通灯带、直流电机、直流气泵的使用，除非排线较短，否则不建议提高pwm频率
