def is_anagram(word1, word2):
    # 去除空格并将单词转换为小写
    word1 = word1.replace(' ', '').lower()
    word2 = word2.replace(' ', '').lower()
  
    # 检查两个单词的长度是否相同
    if len(word1) != len(word2):
        return False

    # 将两个单词的字符排序后比较
    sorted_word1 = sorted(word1)
    sorted_word2 = sorted(word2)
  
    # 检查排序后的字符列表是否相同
    if sorted_word1 == sorted_word2:
        return True
    else:
        return False

# 测试示例
word1 = input("请输入第一个单词：")
word2 = input("请输入第二个单词：")

if is_anagram(word1, word2):
    print("是变位词！")
else:
    print("不是变位词。")
