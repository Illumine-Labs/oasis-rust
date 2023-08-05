# Basics


## Date and Time

### `Chrono`` vs `Time`` vs `std::time`

推荐的优先选择顺序，从高到低排列：

- `icu`
- `time`
- `chrono`
- `std::time`

- [参考： Reddit Posts](https://www.reddit.com/r/rust/comments/14n9zcy/chrono_vs_time_vs_stdtime/)

---

### icu4x

Unicode-org 提供。

if you need localized (or just advanced) date formatting, or correct handling of time zones, consider the icu library.

> 如果你需要本地化（或者只是高级的）日期格式化，或者正确处理时区，请考虑使用icu库，它是由 Unicode 联盟官方维护和赞助的。
> 如果你只需要记录时间戳（使用协调世界时或本地时间），无论是 time 还是 chrono 都可以。但是，如果你需要计算日期和时间（即使你不需要本地化或格式化），真的没有好的替代方案。

[icu4x](https://github.com/unicode-org/icu4x)

> ICU4X 大多数功能依赖于客户提供给API的数据，所以使用了一个 DataProvider 的概念来将数据与逻辑分离。

### chrono

- 0.4.26

[chrono](https://github.com/chronotope/chrono)

> 在 chrono-tz 的“未来改进”部分中，列出了所有由 icu 库支持的功能。


### time-rs

- v0.3 

time 0.3 had all the functionality of chrono, but incompatible with chrono.

- [time-rs](https://github.com/time-rs/time)
- [book](https://time-rs.github.io/book/)
