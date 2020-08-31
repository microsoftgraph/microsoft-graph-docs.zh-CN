---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 25aae9eeea7c2bf216ec94ffa2f1ac9654e04d79
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312108"
---
# <a name="outlookuser-resource-type"></a>outlookUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

表示用户可用的 Outlook 服务。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create category](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |在用户主类别列表中创建 **outlookCategory** 对象。|
|[List categories](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md) 集合 |获取为用户定义的所有类别。|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md) 集合 | 获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。 |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md) 集合 | 获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。 |
|[创建 outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (弃用)  |[outlookTaskFolder](outlooktaskfolder.md)| 在默认任务组中创建任务文件夹 (`My Tasks` 用户邮箱的) 。|
|[列出 taskFolders](../api/outlookuser-list-taskfolders.md) (弃用)  |[outlookTaskFolder](outlooktaskfolder.md) 集合| 获取用户邮箱中的所有 Outlook 任务文件夹。|
|[创建 outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (弃用)  |[outlookTaskGroup](outlooktaskgroup.md)| 在用户的邮箱中创建一个 Outlook 任务组。|
|[列出 taskGroups](../api/outlookuser-list-taskgroups.md) (弃用)  |[outlookTaskGroup](outlooktaskgroup.md) 集合| 获取用户邮箱中的所有 Outlook 任务组。|
|[创建 outlookTask](../api/outlookuser-post-tasks.md) (弃用)  |[outlookTask](outlooktask.md)| 在默认任务组中创建一个 Outlook 任务 (`My Tasks`) 和默认的任务文件夹 (`Tasks` 用户邮箱中的) 。|
| (弃用) [列出任务](../api/outlookuser-list-tasks.md) |[outlookTask](outlooktask.md) 集合| 获取用户邮箱中的所有 Outlook 任务。|



## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) 集合| 为用户定义的类别列表。 | 
|taskFolders (弃用) |[outlookTaskFolder](outlooktaskfolder.md) 集合| 用户的 Outlook 任务文件夹。 只读。 可为 Null。|
|taskGroups (弃用) |[outlookTaskGroup](outlooktaskgroup.md) 集合| 用户的 Outlook 任务组。 只读。 可为 Null。|
|任务 (弃用) |[outlookTask](outlooktask.md) 集合| 用户的 Outlook 任务。 只读。 可为 Null。|

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
