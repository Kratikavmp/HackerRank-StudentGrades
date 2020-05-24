# HackerRank-StudentGrades

var grades = [24,68,37,42]
var a = grades
var multiple = 0
var diff = 0
var finalArray: [Int] = []

for i in 0..<a.count{
    if(a[i]%5 != 0){
        multiple = a[i]+5 - a[i]%5
        diff = multiple - a[i]
        if((diff < 3) && (a[i] >= 38)){
            a[i] = a[i] + diff
            finalArray.append(a[i])
        }
        else{
            finalArray.append(a[i])
        }
    }
    else{
         finalArray.append(a[i])
    }
    
}
print(finalArray)
