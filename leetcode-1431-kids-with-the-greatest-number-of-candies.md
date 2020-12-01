```go
func kidsWithCandies(candies []int, extraCandies int) []bool {
    max := 0
    for _, candy := range candies {
        if candy > max {
            max = candy
        }
    }

    arr := make([]bool, len(candies))

    for i, candy := range candies {
        if (candy + extraCandies) >= max {
            arr[i] = true
        } else {
            arr[i] = false
        }
    }

    return arr

}
```