---
title: 寻址 OneDrive 上驱动器中的资源
description: 了解如何使用基于 ID 和基于路径的寻址访问 OneDrive 上驱动器内的项目，以及如何正确编码 Microsoft Graph 的路径。
ms.localizationpriority: high
ms.prod: sharepoint
author: JeremyKelley
doc_type: conceptualPageType
ms.openlocfilehash: 46f0304dc81245c79213f96cde30efb95766a580
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447119"
---
# <a name="address-resources-in-a-drive-on-onedrive"></a>寻址 OneDrive 上驱动器中的资源

了解如何使用基于 ID 和基于路径的寻址访问 OneDrive 上驱动器内的项目，以及如何正确编码 Microsoft Graph 的路径。

## <a name="id-based-addressing"></a>基于 ID 的寻址
OneDrive 支持对项进行基于 ID 的寻址。 项在创建时即分配有唯一标识符，此 ID 保持不变，无论用户对项执行的操作如何。 重命名或移动项不会更改项 ID。

借助基于 ID 的寻址，可以非常方便地跟踪可能被用户移到 OneDrive 中其他位置上的项。 只要有项 ID 且项存在，就可以找到项。

## <a name="path-based-addressing"></a>基于路径的寻址
OneDrive 还支持基于路径的寻址。 这样一来，可以使用易记的 URL 语法，根据 OneDrive 中可见项的层次结构寻址项。 如果知道项所处的层次结构，可以直接寻址此项，而无需为了发现层次结构的每一层级而花费时间进行重复调用。

然而，由于基于路径的寻址是以项名称为依据，因此重命名项或将项移到新位置将导致项路径发生变化。

可以相对于 OneDrive 中的任何项使用基于路径的寻址。 例如，使用共享文件夹时，可以使用相对于共享文件夹项 ID 的基于路径的 URL，按路径寻址共享文件夹中的某项。

## <a name="examples"></a>示例
以下示例演示可用于访问数据的不同 URL 格式。
所有这些 URL 在逻辑上是等效的，都返回 MyFile.xlsx 的内容。

| URL 示例                                       | 说明                                              |
|:--------------------------------------------------|:---------------------------------------------------------|
| `/drive/root:/Documents/MyFile.xlsx:/content`     | 由相对于驱动器根目录的路径指定。       |
| `/drive/special/documents:/MyFile.xlsx:/content`  | 由 `documents` 特殊文件夹中的文件名指定。 |
| `/drive/items/0123456789AB/content`               | 由  item-id 指定。                                    |
| `/drives/AB0987654321/items/0123456789AB/content` | 由 drive-id 和 item-id 指定。                       |


## <a name="path-encoding"></a>路径编码

OneDrive 支持使用用户 OneDrive 中项的路径寻址文件和文件夹。不过，由于路径中的用户指定内容可能包含 URL 不安全字符，因此应确保正确编码所有路径段。

Microsoft Graph 要求 URL 符合 [RFC 3986](http://tools.ietf.org/html/rfc3986)。 下面总结了如何正确编码 Microsoft Graph 路径。

### <a name="onedrive-reserved-characters"></a>OneDrive 保留字符
以下为 OneDrive 保留字符，不得用于 OneDrive 文件夹名称和文件名。

```
  onedrive-reserved  = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|"
  onedrive-business-reserved
                     = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|" / "#" / "%"
```

> [!NOTE]
> - 文件夹名称不得以句点 (`.`) 结尾。
> - 文件或文件夹名称不能以波形符(“~”)开头。
>
> 有关详细信息，请参阅[通过适用于工作或学校的 OneDrive 将 SharePoint 库同步到计算机时的局限性和限制](https://support.microsoft.com/en-us/kb/2933738)。

### <a name="uri-path-characters"></a>URI 路径字符

构造 Microsoft Graph API 的 URL 路径段时，根据 URI RFC，可以对路径名称使用下列字符。

```
  pchar       = unreserved / pct-encoded / sub-delims / ":" / "@"
  pct-encoded = "%" HEXDIG HEXDIG
  unreserved  = ALPHA / DIGIT / "-" / "." / "_" / "~"
  sub-delims  = "!" / "$" / "&" / "'" / "(" / ")"
              / "*" / "+" / "," / ";" / "="
```

必须对 `pchar` 组中不包含的项名称字符（如 `#` 和 ` `（空格））进行百分比编码。

### <a name="encoding-characters"></a>字符编码
Microsoft Graph 使用标准百分比编码，即先对 URL 无效字符进行百分比编码，然后使用 UTF-8 字符代码对字符进行编码。 例如：

* `" "` -> `%20`
* `"#"` -> `%23`

### <a name="common-url-encoding-mistakes"></a>常见 URL 编码错误
不能在一次调用中对整个 URL 进行编码，因为 URL 每个段的编码规则都不同。 如果未经正确编码，将很难通过未编码的 URL 明确判断哪些段包含哪些内容。 因此，必须在生成 URL 字符串时对 URL 路径进行编码。

例如，不用编写以下代码：

```
string url = url_encode("https://graph.microsoft.com/v1.0/me/drive/root:/" + path + ":/children")
```

而是编写以下代码：

```
string url = "https://graph.microsoft.com/v1.0/me/drive/root:/" + url_path_encode(path) + ":/children")
```

不过，并不是所有 URL 编码库都符合标准 URL 路径编码的全部要求。

### <a name="net--c-sharp--visual-basic"></a>.NET/C-Sharp/Visual Basic

`HttpUtility` 和 `Uri` 的 .NET 类包括各种 URL 编码方法。 不过，这些方法（包括 `HttpUtility.UrlPathEncode`）都无法正确编码 URL 路径组成部分的所有保留字符。

应使用 `UriBuilder` 构造经过正确转义的 URL，而不是使用这些方法。

```csharp
UriBuilder builder = new UriBuilder("https://graph.microsoft.com");
builder.Path = "/v1.0/me/drive/root:/Documents/My Files/#nine.docx";
Uri url = builder.Uri;
```

### <a name="objective-c--ios"></a>Objective-C/iOS

对于 Objective-C、iOS 和 Mac OS X 开发，使用 `stringByAddingPercentEncodingWithAllowedCharacters` 方法和 `[NSCharacterSet URLPathAllowedCharacterSet]` 对 URL 路径组成部分进行正确编码。

```objc
NSString *root = @"https://graph.microsoft.com/v1.0/me/drive/root:/";
NSString *path = @"Documents/My Files/#nine.docx";
NSString *encPath = [path stringByAddingPercentEncodingWithAllowedCharacters:[NSCharacterSet URLPathAllowedCharacterSet]];
NSURL *url = [[NSURL alloc] initWithString:[root stringByAppendingString:encPath]];
```


### <a name="android"></a>Android

使用 `Uri.Builder` 类构造经过正确编码的 URL。

```java
Uri.Builder builder = new Uri.Builder();
builder.
  scheme("https").
  authority("graph.microsoft.com").
  appendPath("v1.0").
  appendPath("me").
  appendPath("drive").
  appendPath("root:").
  appendPath("Documents").
  appendPath("My Files").
  appendPath("#nine.docx");
String url = builder.build().toString();
```

### <a name="javascript"></a>JavaScript

使用 JavaScript 中的 `escape()` 正确编码路径组成部分。

```javascript
var root = "https://graph.microsoft.com/v1.0/me/drive/root:";
var path = "/Documents/My Files/#nine.docx";
var url = root + escape(path);
```

### <a name="examples"></a>示例

下面的示例展示了具有以下文件夹层次结构的 OneDrive 用户 (Adele)：
```
OneDrive
    \Adele's Files
        \doc (1).docx
    \estimate%s.docx
    \Break#Out
        \saved_game[1].bin
```

若要寻址 Adele 的每个文件，请使用百分比编码，如下所示：

| 路径                     | 已编码的 URL 路径                      |
|:-------------------------|:------------------------------------------|
| `\Adele's Files`          | `/root:/Adele's%20Files`                   |
| `\...\doc (1).docx`      | `/root:/Adele's%20Files/doc%20(1).docx`    |
| `\...\estimate%.docx`    | `/root:/Adele's%20Files/estimate%25s.docx` |
| `\Break#Out`             | `/root:/Break%23Out`                      |
| `\...\saved_game[1].bin` | `/root:/Break%23Out/saved_game[1].bin`    |

## <a name="see-also"></a>另请参阅

- [OneDrive 文件存储 API 概述](onedrive-concept-overview.md)