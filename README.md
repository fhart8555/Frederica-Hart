from googletrans import Translator

# 创建一个翻译器对象
translator = Translator()

# 翻译一段英文文本为中文
text = "Hello, World!"
translated_text = translator.translate(text, dest='zh-cn').text

# 打印翻译结果
print(translated_text)
