---
title: 笔记本资源类型
description: OneNote 笔记本。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: f8562670441c756e5263511304225440ec063a9a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721899"
---
# <a name="notebook-resource-type"></a>笔记本资源类型

命名空间：microsoft.graph

OneNote 笔记本。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|createdDateTime|DateTimeOffset|笔记本的创建日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|字符串|笔记本的唯一标识符。 只读。|
|isDefault|Boolean|指示这是否是用户的默认笔记本。 只读。|
|isShared|Boolean|指明笔记本是否为共享。 如果是，笔记本的内容可供所有者以外的用户查看。 只读。|
|lastModifiedBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改笔记本的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|links|[NotebookLinks](notebooklinks.md)|用于打开笔记本的链接。 链接 `oneNoteClientURL` 将在 OneNote 本机客户端中打开笔记本（如果已安装）。 该 `oneNoteWebURL` 链接在 OneNote 网页中打开笔记本。|
|displayName|字符串|笔记本的名称。|
|sectionGroupsUrl|字符串|导航属性的 `sectionGroups` URL，可返回笔记本中所有节组。 只读。|
|sectionsUrl|字符串|导航属性的 `sections` URL，可返回笔记本中所有节。 只读。|
|self|字符串|终结点，您可在此处获取关于笔记本的详细信息。 只读。|
|userRole|onenoteUserRole|可取值为：`Owner`、`Contributor`、`Reader`、`None`。 所有者表示对笔记本的所有者级别访问权限。 参与者表示笔记本的读/写访问权限。 Reader 表示对笔记本的只读访问权限。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|sectionGroups|[SectionGroup](sectiongroup.md) 集合|笔记本中的分区组。 只读。 可为 NULL。|
|sections|[OnenoteSection](section.md) 集合|笔记本中的节。 只读。 可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取笔记本](../api/notebook-get.md) | [笔记本](notebook.md) |读取笔记本的属性和关系。|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md) 集合 | 获取用户最近访问过的一组笔记本。 |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [笔记本](notebook.md) | 使用笔记本对象 URL 路径检索其属性和关系。 |
|[创建分区组](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| 通过发布到指定笔记本中的 sectionGroups 集合创建分区组。|
|[列出分区组](../api/notebook-list-sectiongroups.md) |[SectionGroup](sectiongroup.md) 集合| 获取指定笔记本中的分区组集合。|
|[创建分区](../api/notebook-post-sections.md) |[OnenoteSection](section.md)| 通过发布到指定笔记本中的节集合创建分区。|
|[列出节](../api/notebook-list-sections.md) |[OnenoteSection](section.md) 集合| 获取指定笔记本中的分区集合。|
|[copyNotebook](../api/notebook-copynotebook.md)| 无 | 复制笔记本。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

