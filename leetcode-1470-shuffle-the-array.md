```go
func shuffle(nums []int, n int) []int {
    // 声明数组
    arr := [] int {}
    for i:=0; i < n; i++ {
       arr = append(arr, nums[i])
       arr = append(arr, nums[n + i])
    }
    return arr
}
```

```go
func shuffle(nums []int, n int) []int {
    // 声明数组
    arr := make([]int,len(nums))
    for i:=0; i < n; i++ {
      arr[2*i] = nums[i]
      arr[2*i + 1] = nums[n + i]
    }
    return arr
}
```