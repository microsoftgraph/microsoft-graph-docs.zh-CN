---
title: onenotePage 资源类型
description: 笔记本OneNote页。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: 4f4b556b048d535236d40259bc9736de4e3e5ee4
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176724"
---
# <a name="onenotepage-resource-type"></a>onenotePage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

笔记本OneNote页。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|content|流|页面的 HTML 内容。|
|contentUrl|String|页面 HTML 内容的 URL。  只读。|
|createdByAppId|字符串|创建页面的应用程序的唯一标识符。 只读。|
|createdDateTime|DateTimeOffset|页面的创建日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|String|页面的唯一标识符。  只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改页面的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|水平|Int32|页面的缩进级别。 只读。|
|links|[pageLinks](pagelinks.md)|用于打开页面的链接。 如果已安装，链接`oneNoteClientURL`将在OneNote本机客户端中打开该页面。 链接`oneNoteWebUrl`在OneNote web 版中打开页面。 只读。|
|以|Int32|页面在其父部分中的顺序。 只读。|
|自我|字符串|可在其中获取有关页面的详细信息的终结点。 只读。|
|title|String|页面的标题。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|parentNotebook|[笔记本](notebook.md)|包含页面的笔记本。  只读。|
|parentSection|[onenoteSection](onenotesection.md)|包含页面的部分。 只读的。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[获取页面](../api/page-get.md) | [onenotePage](onenotepage.md) |读取页面的属性和关系。|
|[更新页面内容](../api/page-update.md) | 无 |更新页面的 HTML 内容。 |
|[删除页面](../api/page-delete.md) | 无 |删除页面。 |
|[copyToSection](../api/page-copytosection.md)| 无 |将页面复制到特定部分。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


