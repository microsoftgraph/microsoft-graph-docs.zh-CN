---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 15afe75d10bad489b913eaf7215cbc8327e02317
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130667"
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
|[创建已弃 (outlookTaskFolder](../api/outlookuser-post-taskfolders.md))  |[outlookTaskFolder](outlooktaskfolder.md)| 在用户邮箱的默认任务组 () `My Tasks` 任务文件夹。|
|[列出已 (taskFolders](../api/outlookuser-list-taskfolders.md))  |[outlookTaskFolder](outlooktaskfolder.md) 集合| 获取用户邮箱中所有 Outlook 任务文件夹。|
|[创建已弃 (outlookTaskGroup](../api/outlookuser-post-taskgroups.md))  |[outlookTaskGroup](outlooktaskgroup.md)| 在用户邮箱中创建 Outlook 任务组。|
|[列出已 (](../api/outlookuser-list-taskgroups.md) 任务组)  |[outlookTaskGroup](outlooktaskgroup.md) 集合| 获取用户邮箱中所有的 Outlook 任务组。|
|[创建 outlookTask](../api/outlookuser-post-tasks.md)（已弃用） |[outlookTask](outlooktask.md)| 在默认任务组 () 创建 Outlook 任务， () `My Tasks` `Tasks` 用户邮箱中的默认任务文件夹。|
|[列出任务](../api/outlookuser-list-tasks.md)（已弃用） |[outlookTask](outlooktask.md) 集合| 获取用户邮箱中的所有 Outlook 任务。|



## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) 集合| 为用户定义的类别列表。 | 
|taskFolders (弃用) |[outlookTaskFolder](outlooktaskfolder.md) 集合| 用户的 Outlook 任务文件夹。 只读。 可为 NULL。|
|taskGroups (弃用) |[outlookTaskGroup](outlooktaskgroup.md) 集合| 用户的 Outlook 任务组。 只读。 可为 NULL。|
|任务 (已弃) |[outlookTask](outlooktask.md) 集合| 用户的 Outlook 任务。 只读。 可为 Null。|

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


