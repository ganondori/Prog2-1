1#

Write-Host "Write your name: "

$Name = Read-Host

Write-Host "Your name is:" $Name 



---------------------------------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------------------------------

2#

package main



import (

  "fmt"

  "os"

)



func main() {

  var Name string

  fmt.Println("Welcome")

  fmt.Println("Write your name")

  fmt.Scanf("%s", &Name)

  if Name != "" {

​    os.Stdout.WriteString("Your name is: " + Name)

  } else {

​    fmt.Println("Error code 100")

  }

}

----------------------------------------------------------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------------------

#3

package main



import (

  "fmt"

  "os"

)



func main() {

  var N int

  fmt.Println("Welcome")

  fmt.Println("Write a Number: ")

  fmt.Scanf("%d", &N)

  if N > 0 {

​    os.Stdout.WriteString("Good one")

  } else {

​    os.Stderr.WriteString("Invalid imput")

  }

}

----------------------------------------------------------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------------------

#4

package main



import (

  "fmt"

  "os"

)



func main() {

  var N int

  fmt.Println("Welcome")

  fmt.Println("Write a Number: ")

  fmt.Scanf("%d", &N)

  if N > 0 {

​    os.Stdout.WriteString("Good one")

  } else {

​    os.Stderr.WriteString("Invalid imput")

  }

}

----------------------------------------------------------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------------------

#5

package main



import (

  "fmt"

  "os"

  "strconv"

)



func main() {

  N := 0



  fmt.Println("Write your number")

  fmt.Scanf("%d", &N)

  fmt.Println(" ")

  for i := 1; i <= N; i++ {

​    s := strconv.Itoa(i)

​    os.Stdout.WriteString(s)

​    fmt.Println(" ")

  }

}

----------------------------------------------------------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------------------

#6

package main



import (

  "fmt"

  "os"

  "strconv"

)



func main() {

  N := 0

  X := 0

  Y := 0

  i := 0

  // Suma := 0



  fmt.Println("How many numbers you want to introduce")

  fmt.Scanf("%d", &N)

  fmt.Println(" ")

  for i = N; i >= 0; i-- {



​    s := strconv.Itoa(X)

​    if s == "\n" {

​      break

​    }

​    fmt.Scanf("%d\n", &X)

​    Y = X + Y



​    fmt.Print("Whats your number?\n")

  }

  S := strconv.Itoa(Y)

  os.Stdout.WriteString(S)

}

----------------------------------------------------------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------------------

#7

package main



import (

  "fmt"

  "os"

  "strconv"

)



func main() {

  N := 0

  X := 0

  Y := 0

  i := 0

  // Suma := 0



  fmt.Println("How many numbers you want to introduce")

  fmt.Scanf("%d", &N)

  fmt.Println(" ")

  for i = N; i >= 0; i-- {



​    s := strconv.Itoa(X)

​    if s == "\n" {

​      break

​    }

​    fmt.Scanf("%d\n", &X)

​    Y = (X*X) + Y



​    fmt.Print("Whats your number?\n")

  }

  S := strconv.Itoa(Y)

  os.Stdout.WriteString(S)

}