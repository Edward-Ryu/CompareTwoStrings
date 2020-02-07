/*
How to use!
1. copy & paste below code in your playground.
2. change both of str1 & str2 with your sentences to compare.
3. run
*/


let str1 = "abcdefghijkl"
var str2 = "abcdefghsjkl"

func compareTwoStr() -> Bool {
    if str1.count != str2.count {
        return false
    } else {
        for item in str1 {
            if item != str2.removeFirst() {
                return false
            }
        }
        return true
    }
}

if compareTwoStr() {
    print("Two sentences are identical.")
} else {
    print("Two sentecces are different from each other.")
}
