---
title: 页面资源类型
description: 笔记本中的OneNote页。
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f2a21f47d0e29930cf4012f4a2713b372cd77d2c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117975"
---
# <a name="page-resource-type"></a>页面资源类型

命名空间：microsoft.graph

笔记本中的OneNote页。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|content|流|页面的 HTML 内容。|
|contentUrl|String|页面的 HTML 内容的 URL。  只读。|
|createdByAppId|字符串|创建页面的应用程序的唯一标识符。 只读。|
|createdDateTime|DateTimeOffset|页面的创建日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|String|页面的唯一标识符。  只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改页面的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|level|Int32|页面的缩进级别。 只读。|
|links|[PageLinks](pagelinks.md)|用于打开页面的链接。 如果 `oneNoteClientURL` 已安装，该链接将在OneNote客户端中打开页面。 链接 `oneNoteWebUrl` 将在页面打开OneNote web 版。 只读。|
|order|Int32|页面在其父节中的顺序。 只读。|
|self|String|可在其中获取页面详细信息的终结点。 只读。|
|title|String|页面的标题。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|parentNotebook|[笔记本](notebook.md)|包含页面的笔记本。  只读。|
|parentSection|[OnenoteSection](section.md)|包含页面的部分。 只读的。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取页面](../api/page-get.md) | [Page](page.md) |读取页面的属性和关系。|
|[更新页面内容](../api/page-update.md) | 无 |更新页面的 HTML 内容。 |
|[删除页面](../api/page-delete.md) | 无 |删除页面。 |
|[copyToSection](../api/page-copytosection.md)| 无 |将页面复制到特定部分。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

