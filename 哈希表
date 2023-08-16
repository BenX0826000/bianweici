def is_anagram(word1, word2):
    # 去除空格并将单词转换为小写
    word1 = word1.replace(' ', '').lower()
    word2 = word2.replace(' ', '').lower()
  
    # 检查两个单词的长度是否相同
    if len(word1) != len(word2):
        return False

    # 创建字母计数的哈希表
    letter_count = {}
    
    # 统计第一个单词中的字母出现次数
    for letter in word1:
        if letter in letter_count:
            letter_count[letter] += 1
        else:
            letter_count[letter] = 1

    # 检查第二个单词中的字母是否与哈希表匹配
    for letter in word2:
        if letter in letter_count:
            letter_count[letter] -= 1
            if letter_count[letter] == 0:
                del letter_count[letter]
        else:
            return False

    # 如果哈希表为空，则两个单词是变位词
    if len(letter_count) == 0:
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
