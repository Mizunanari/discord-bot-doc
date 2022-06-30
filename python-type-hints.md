#　Pythonで型を活用する

mypyを活用することで、Pythonでも型を強制することができます。

まずはPythonで型を指定する方法を解説します。

```python
def counter(count: int) -> str:
    
    display: str = "現在のカウント : " + str(count)

    return display

print(counter(1))
```

- 関数では`-> str`の表記から返り値がstr型であることがわかります。
- 引数では`counter(count: int)`でint型であることを指定しています。
- 変数では`display: str`でstrを指定しています。

## Typingを使う

また、型がわからない場合はUnionやAnyが使用できます。

__Union__

```python
# new
display: str | int = zisho.get("test")

# old
dispaly: Union[str,int] = zisho.get("test")
```

Unionは、指定した複数の型を代入できます。

__Any__

```python
display: Any = zisho["test"]
```

`Any`は型のチェックをしません。

#　mypyを設定する。

プロジェクトの`pyproject.toml`には、mypyの設定がコメントアウトされています。  
これをコメントインすることで、mypyの設定が有効になります。

mypyでは、型が指定されていないとエラーを表示します。

## 参考リンク

https://docs.python.org/ja/3/library/typing.html

[home](/index.md)