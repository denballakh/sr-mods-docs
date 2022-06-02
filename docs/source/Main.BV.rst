Про `Main.BV.OnSave`, `Main.BV.OnLoad`, `Main.BV.OnStart`
=========================================================

`Main.dat`:
```
BV ~{
    OnSave ~{
        <code_name> ~{
            =<code>
        }
    }
    OnLoad ~{
        <code_name> ~{
            =<code>
        }
    }
    OnStart ~{
        <code_name> ~{
            =<code>
        }
    }
}
```
Разделы `BV.OnSave`, `BV.OnLoad`, `BV.OnStart` должны содержать несколько блоков с кодом.
При создании галактики будут выполнены все блоки кода в разделе `BV.OnStart`
При сохранении игры будут выполнены все блоки кода в разделе `BV.OnSave`
При загрузке сейва будут выполнены все блоки кода в разделе `BV.OnLoad`

[см. мердж]
[см. код в датниках]
[см. генерация галактики]
[см. функцию GenerateCodeStringFromBlock]
