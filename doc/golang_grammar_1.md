### Golang 语法 1  
Interface类型转换：  
  type I interface ｛
  }  
  type AnthorI interface {
  }  
  func test(a *I) {  
    t := a.(*AnthorI)  
  }

golang中的struct类似继承关系：  
  type A struct ｛
    AValue int64
  ｝
  type B struct ｛
    ＊A
  ｝
  a := &A{}
  b := &B{}
  b.A = a;
  b.AValue
  
  
