纳西妲：
.\runtime\python.exe api.py -s "models\nxd\nxd_.pth" -g "models\nxd\nxd_.ckpt" -dr "models\nxd\nxd.wav" -dt "快去避雨吧，小心头顶上长出蘑菇哦。" -dl "zh"

流萤：
.\runtime\python.exe api.py -s "models\ly\ly.pth" -g "models\ly\ly.ckpt" -dr "models\ly\ly.wav" -dt "所有人在这里平等的睡去，无论缘由，尽管我们确实各怀目的。" -dl "zh"

符华：
.\runtime\python.exe api.py -s "models\fh\Fuka_e24_s408.pth" -g "models\fh\Fuka-e50.ckpt" -dr "models\fh\fh.wav" -dt "从监控画面来看，金库完好无损。" -dl "zh"

yousa：
.\runtime\python.exe api.py -s "models\yousa\yousa_e312_s82056.pth" -g "models\yousa\yousa-e10.ckpt" -dr "models\yousa\yousa.wav" -dt "好冷啊，你那边已经冷起来了吗？我们这边是我们四川这边好像是明天开始降温。" -dl "zh"

花火：
.\runtime\python.exe api.py -s "models\hh\hh_e12_s216.pth" -g "models\hh\hh-e12.ckpt" -dr "models\hh\hh.wav" -dt "你拿走记忆，我收获欢愉，我们能从彼此身上各取所需。" -dl "zh"




.\frpc.exe -c frpc.toml




GET请求：
http://47.98.113.218:9880?text={{speakText}}&text_language=zh


POST请求：
http://47.98.113.218:9880,
{
    "method": "POST",
    "body":
    {
        "text": "{{speakText}}",
        "text_language": "zh"
    }
}
