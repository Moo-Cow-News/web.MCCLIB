## MCCLIB

Welcome to the MCCLIB documentation. This will come with download instructions and the documentation of the libary.


## Install Instructions

Fist, go to the main reposotory [Here](https://github.com/Moo-Cow-News/MCCLIB) and then go to clone repository. All the code will be in the source folder. 
Now, you can put your project files inside the source folder. This will let you use the `using MCCLIB.commands` namespace.

Versions:

Version | Stable
--------| ------
Alpha   | Not stable
Main    | Stable


## Documentation

### Calculator:

Add Method:

```CSharp

using MCCLIB.Commands;

class Sample {
  static void Main(string[] args) {
    Calculator.Add(5, 5, 5);
  }
}

```

Subtract Method:


```CSharp

using MCCLIB.Commands;

class Sample {
  static void Main(string[] args) {
    Calculator.Subtract(5, 5, 5);
  }
}

```

Multiply Method:


```CSharp

using MCCLIB.Commands;

class Sample {
  static void Main(string[] args) {
    Calculator.Multiply(5, 5, 5);
  }
}

```

Divide Method:


```CSharp

using MCCLIB.Commands;

class Sample {
  static void Main(string[] args) {
    Calculator.Divide(5, 5, 5);
  }
}

```
### Double Data List

The double data list lets you create a list with multiple values per index.

How to Create a list.

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

```

For paramaters, you can also import lists that are already made:

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>(list1, list2);

```

How to add value to list.

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

name.AddItem(value1, value2);

```

Value1 and Value2 must be the type you gave in the constructor.

How to add multiple values to the list.

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

name.AddItems(value1List, value2List);

```

Value1List and value2List need to be lists of the type you entered in the constructor.

How to remove a value:

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

name.RemoveItem(index);

```

Index is type int and will return true if it did remove it and false if it did not.

How to get a value:

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

name.GetItem(index);

```

Returns a class called DoubleData that contains the two values. You can run ``` ToString ``` on it to get both the values in string format.

How to get all the values:

```CSharp

DoubleDataList<Type1, Type2> name = new DoubleDataList<Type1, Type2>();

name.GetItems();

```

Returns a class called ListDoubleData that contains two lists. You can also run  ``` ToString ``` on it to get all the vales in a readable format.
