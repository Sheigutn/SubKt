[subkt](../../index.md) / [myaa.subkt.tasks](../index.md) / [Merge](index.md) / [scriptInfo](./script-info.md)

# scriptInfo

`val scriptInfo: `[`ScriptInfoSection`](../../myaa.subkt.ass/-script-info-section/index.md) [(source)](https://github.com/Myaamori/SubKt/blob/0.1.13/src/main/kotlin/myaa/subkt/tasks/asstasks.kt#L194)

A [ScriptInfoSection](../../myaa.subkt.ass/-script-info-section/index.md) instance for overriding the script info read from the
merged files. A [scriptInfo](./script-info.md) method is available for easier modification.

**Getter**

A [ScriptInfoSection](../../myaa.subkt.ass/-script-info-section/index.md) instance for overriding the script info read from the
merged files. A [scriptInfo](./script-info.md) method is available for easier modification.

`fun scriptInfo(action: `[`ScriptInfoSection`](../../myaa.subkt.ass/-script-info-section/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/Myaamori/SubKt/blob/0.1.13/src/main/kotlin/myaa/subkt/tasks/asstasks.kt#L276)

Allows you to override values in the Script Info section as needed.

``` kotlin
scriptInfo {
    playResX = 1920
    playResY = 1080
}
```

### Parameters

`action` - A closure operating on a [ScriptInfoSection](../../myaa.subkt.ass/-script-info-section/index.md) instance.