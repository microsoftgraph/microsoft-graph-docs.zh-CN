---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: eadd5947a03fce69f790e2e9f0a4d738078002cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522065"
---
# <a name="outlookuser-resource-type"></a>outlookUser 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户可用的 Outlook 服务。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create category](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |在用户主类别列表中创建 **outlookCategory** 对象。|
|[List categories](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) 集合 |获取为用户定义的所有类别。|
|[创建 outlookTaskFolder](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| 在用户邮箱的默认任务组（`My Tasks`）中创建一个任务文件夹。|
|[列出 taskFolders](../api/outlookuser-list-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)集合| 获取用户邮箱中的所有 Outlook 任务文件夹。|
|[创建 outlookTaskGroup](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| 在用户的邮箱中创建一个 Outlook 任务组。|
|[列出 taskGroups](../api/outlookuser-list-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)集合| 获取用户邮箱中的所有 Outlook 任务组。|
|[创建 outlookTask](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| 在用户邮箱中的默认任务组（`My Tasks`）和默认任务文件夹（`Tasks`）中创建一个 Outlook 任务。|
|[列出任务](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md) 集合| 获取用户邮箱中的所有 Outlook 任务。|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) 集合 | 获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。 |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md) 集合 | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。 |


## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) 集合| 为用户定义的类别列表。 | 
|taskFolders|[outlookTaskFolder](outlooktaskfolder.md)集合| 用户的 Outlook 任务文件夹。 只读。 可为 NULL。|
|taskGroups|[outlookTaskGroup](outlooktaskgroup.md)集合| 用户的 Outlook 任务组。 只读。 可为 NULL。|
|任务|[outlookTask](outlooktask.md) 集合| 用户的 Outlook 任务。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
