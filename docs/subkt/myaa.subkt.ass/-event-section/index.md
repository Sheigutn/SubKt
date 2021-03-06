[subkt](../../index.md) / [myaa.subkt.ass](../index.md) / [EventSection](./index.md)

# EventSection

`class EventSection : `[`FormatSection`](../-format-section/index.md)`<`[`EventLine`](../-event-line/index.md)`>` [(source)](https://github.com/Myaamori/SubKt/blob/0.1.13/src/main/kotlin/myaa/subkt/ass/parser.kt#L1113)

Represents an events section, containing a list of [EventLine](../-event-line/index.md) lines.

### Parameters

`name` - The name of the section, usually `Events`.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `EventSection(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)`<br>Represents an events section, containing a list of [EventLine](../-event-line/index.md) lines. |

### Properties

| Name | Summary |
|---|---|
| [format](format.md) | `var format: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>`<br>The order of the fields in the textual representation of each line. |
| [lineTypes](line-types.md) | `val lineTypes: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>`<br>The types of lines allowed in this section, e.g. `Dialogue` and `Comment` for [EventSection](./index.md). |

### Inherited Properties

| Name | Summary |
|---|---|
| [lineClass](../-format-section/line-class.md) | `val lineClass: `[`KClass`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.reflect/-k-class/index.html)`<`[`T`](../-format-section/index.md#T)`>`<br>A class object used for instantiating new lines of type [T](../-format-section/index.md#T). |
| [lines](../-format-section/lines.md) | `val lines: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`T`](../-format-section/index.md#T)`>`<br>The lines contained in this section. |

### Functions

| Name | Summary |
|---|---|
| [serializeContents](serialize-contents.md) | `fun serializeContents(includeExtraData: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>`<br>Returns a string sequence representing the serialization of the contents of this section, without the section name. |

### Inherited Functions

| Name | Summary |
|---|---|
| [formatString](../-format-section/format-string.md) | `fun formatString(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Returns a textual representation of the format line that starts the section. |
| [parse](../-format-section/parse.md) | `open fun parse(data: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`KeyValLine`](../-key-val-line/index.md)`>, extraData: `[`ExtraData`](../-extra-data.md)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Deserializes a list of lines in [KeyValLine](../-key-val-line/index.md) format and adds them to this section. |
| [parseLine](../-format-section/parse-line.md) | `fun parseLine(line: `[`KeyValLine`](../-key-val-line/index.md)`, extraData: `[`ExtraData`](../-extra-data.md)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Parses a single line from a [KeyValLine](../-key-val-line/index.md) and adds it to this section. |
| [serializeLine](../-format-section/serialize-line.md) | `fun serializeLine(line: `[`T`](../-format-section/index.md#T)`, process: (`[`MutableMap`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)` = { }): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Serializes a single line according to the field order given by [format](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.text/format.html) in this section. |
