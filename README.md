# challemges-for-coding
def permuteation(s, answer):
    if (len(s) == 0):
        print(answer, end=" ")
        return

    for i in range(len(s)):
        ch = s[i]
        left_substr = s[0:i]
        right_substr = s[i + 1:]
        rest = left_substr + right_substr
        permuteation(rest, answer + ch)



answer = ""
string =   input("Enter the string")
character_input = input("Enter the character")
print(string.replace(character_input,''))
