# Questions for LX Scala e.Near Stand #

## Notes ##

- Questions are marked with an extimated dificulty level from 1 to 5


## Questions ##


What is the well known code patern present in the following Scala code? (3)

```scala
trait Encoder[-T] {
    def encode(t: T): Array[Byte]
}

object Encoder {
    def instance[T](implicit encoder: Encoder[T]) = encoder
}
```

- [ ] Serializer
- [x] Type class
- [ ] Functional interface

---

What will be the value of `a` in the following code? (2)
a`variable in the following code? (2)

```scala
val x = 2
val a = if(x > 2) 1
```

- [x] ()
- [ ] NaN
- [ ] 0


---


What is *not* a known Scala functional programming library? (3)

- [ ] Cats
- [ ] Dogs
- [x] Rabbits

---

In the following code, what does `d.T`stand for? (4)

```scala
trait Decoder {
    type T
}

def decodeList(d: Decoder, l: List[String]): List[d.T] = ???
```

- [ ] Type Member
- [ ] Abstract type
- [x] Path dependent type

---


What is true regarding the following code? (3)


```scala
trait encoder[-T] {
    def encode(t: T): Array[Byte]
}
```

- [x] `Encode[Any]` is a subtype of `encoder[SString]`
- [ ] `Encoder[Int]` is a subtype of `Ecoder[Anyval]`
- [ ] `Encoder[String]` is a subtype of `Encoder[Any]`


---


What is the return type of the standard library's `???`method?

- [ ] Any
- [ ] Unit
- [x] Nothing

---


What is the main goal of the Shapeless library? (3)

- [ ] Json encoding / decoding
- [x] Generic Programming
- [ ] Application configuration

---

What is the type of the following value? (1)

```scala
1 :: 2 :: 3 :: Nil
```

- [ ] `LinkedList[Int]`
- [ ] `Stack[Int]`
- [x] `List[Int]`


---

What is `T, in the following definition? (2)

```scala
trait Operations {
    type T
}
```

- [ ] Existential type
- [x] Type member
- [ ] Abstract type

