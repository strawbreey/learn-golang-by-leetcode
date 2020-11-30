
```go
func maximumWealth(accounts [][]int) int {
    max := 0
    for _, nums :=range accounts {
        sum := 0
        for _, num := range nums {
            sum+=num
        }
        if (sum > max) {
            max = sum
        }
    }
    return max
}
```