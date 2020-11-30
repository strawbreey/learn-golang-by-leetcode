
```go
func runningSum(nums []int) []int {
    arr := [] int {} 
    sum := 0
    for _, num := range nums {
        sum += num
        arr = append(arr, sum)
    }
    return arr
}
```


```go
func runningSum(nums []int) []int {
    sum := 0
    for i, num := range nums {
        sum += num
        nums[i] = sum
    }
    return nums
}
```

```go
func runningSum(nums []int) []int {
	for i := 1; i < len(nums); i++ {
		nums[i] = nums[i] + nums[i-1]
	}
	return nums
}
```

```go
func runningSum(nums []int) []int {
	for i:=range nums{
		if i!=0{
			nums[i]=nums[i-1]+nums[i]
		}
	}
	return nums
}
```