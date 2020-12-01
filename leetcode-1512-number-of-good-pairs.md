```go
func numIdenticalPairs(nums []int) int {
    count:=0
    length:= len(nums)
    for i:= 0; i < length; i++ {
        for j:=i+1; j < length; j++ {
            if (nums[i] == nums[j]) {
                count++
            }
        }
    }
    return count
}
```
