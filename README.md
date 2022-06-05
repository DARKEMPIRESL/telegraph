# telegraph
>[Telegraph API](https://telegra.ph/api) `Golang`
> 
> 
> `telegraph-token`？ [Telegraph API](https://telegra.ph/api) 

### APIs has achieved

---

- [x] `CreatePage`

### Getting Started

---

1. Download

```go
go get -u github.com/DARKEMPIRESL/telegraph
```

2. `test.go`

```go
package main

imoprt "github.com/DARKEMPIRESL/telegraph"

func main(){
  page := &telegraph.Page{
    AccessToken: "......<telegraph-token>......",
		AuthorURL:   "https://github.com/DARKEMPIRESL/telegraph",
		AuthorName:  "telegraph-go",
    Title: 			 "Title here",
    Data:				 "<h1>Put html strings here.</h1>",
	}
  
  link, err := page.CreatePage()
	if err != nil {
    fmt.Println("Create Page Failed: ", err)
  }else{
    fmt.Println(link) 
  }
}
```

