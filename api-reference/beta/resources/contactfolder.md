---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 450c683d91eeb789c8c54b2bbfd38db695fbbba2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967544"
---
# <a name="contactfolder-resource-type"></a>contactFolder 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含联系人的文件夹。

该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 contactFolder](../api/contactfolder-get.md) | [contactFolder](contactfolder.md) |通过使用联系人文件夹 ID 获取联系人文件夹。|
|[更新](../api/contactfolder-update.md) | [contactFolder](contactfolder.md) |更新 contactFolder 对象。 |
|[删除](../api/contactfolder-delete.md) | 无 |删除 contactFolder 对象。 |
|[列出 childFolder](../api/contactfolder-list-childfolders.md) |[contactFolder](contactfolder.md)集合| 获取指定联系人文件夹下的子文件夹的集合。|
|[创建子 ContactFolder](../api/contactfolder-post-childfolders.md) |[contactFolder](contactfolder.md)| 创建新的 contactFolder 作为指定文件夹的子文件夹。|
|[delta](../api/contact-delta.md)|[联系人](contact.md)集合| 获取用户邮箱中已添加、删除或移除的联系人文件夹集。|
|[列出文件夹中的联系人](../api/contactfolder-list-contacts.md) |[联系人](contact.md)集合| 从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。|
|[在文件夹中创建联系人](../api/contactfolder-post-contacts.md) |[联系人](contact.md)| 将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contactFolder](contactfolder.md)  |在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。   |
|[获取包含单值扩展属性的 contactFolder](../api/singlevaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contactFolder](contactfolder.md) | 在新建或现有的 contactFolder 创建一个或多个多值扩展属性。  |
|[获取包含多值扩展属性的 contactFolder](../api/multivaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | 使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|文件夹的显示名称。|
|id|String|联系人文件夹的唯一标识符。只读。|
|parentFolderId|String|文件夹的父文件夹 ID。|
|wellKnownName|string|如果文件夹为识别的文件夹的文件夹的名称。 当前`contacts`是仅识别联系人文件夹。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|childFolders|[ContactFolder](contactfolder.md) 集合|文件夹中的子文件夹集合。导航属性。只读。可为 Null。|
|contacts|[联系人](contact.md) 集合|文件夹中的联系人。导航属性。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合| 为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
