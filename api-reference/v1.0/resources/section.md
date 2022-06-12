---
title: 节资源类型
description: 笔记本OneNote部分。 分区可包含页面。
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: 532bf71ff7963f4b70588d54d7d5f6b13c78332c
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034836"
---
# <a name="section-resource-type"></a>节资源类型

命名空间：microsoft.graph

笔记本OneNote部分。 分区可包含页面。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|createdDateTime|DateTimeOffset|节的创建日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|String|节的唯一标识符。  只读。|
|isDefault|Boolean|指示这是否是用户的默认部分。 只读。|
|lastModifiedBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改节的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|links|[SectionLinks](sectionlinks.md)|用于打开该部分的链接。 如果已安装，链接`oneNoteClientURL`将在OneNote本机客户端中打开该部分。 链接`oneNoteWebURL`将在OneNote web 版中打开该部分。|
|displayName|String|节的名称。 |
|pagesUrl|字符串|`pages`可在其中获取部分中所有页面的详细信息的终结点。 只读。|
|自我|String|终结点，您可在此处获取关于节的详细信息。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|pages|[OnenotePage](page.md) 集合|分区中的一组页面。  只读。 可为 Null。|
|parentNotebook|[笔记本](notebook.md)|包含该部分的笔记本。  只读。|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|包含节的节组。  只读的。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取分区](../api/section-get.md) | [OnenoteSection](section.md) |读取节的属性和关系。|
|[创建页面](../api/section-post-pages.md) |[页面](page.md)| 通过发布到指定部分中的页面集合来创建页面。|
|[列出页面](../api/section-list-pages.md) |[页面](page.md)集合| 获取指定部分中的页面集合。|
|[copyToNotebook](../api/section-copytonotebook.md)|无|将该部分复制到特定笔记本。|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|无|将该节复制到特定节组。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

