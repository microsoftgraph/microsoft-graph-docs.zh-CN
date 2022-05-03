---
title: printerShare 资源类型
description: 表示用户和打印应用程序可发现的打印机。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ab0dbf8ff2e7a8e64f51cf72afec5415bec265e6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176686"
---
# <a name="printershare-resource-type"></a>printerShare 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户和打印应用程序可发现的打印机。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/print-list-shares.md) | [printerShare](printershare.md) 集合 | 获取租户中的打印机共享列表。 |
| [Get](../api/printershare-get.md) | [printerShare](printershare.md) | 读取 **printerShare** 对象的属性和关系。 |
| [更新](../api/printershare-update.md) | [printerShare](printershare.md) | 更新 **printerShare** 对象。 |
| [删除](../api/printershare-delete.md) | 无 | 取消共享打印机。 |
| [列出作业](../api/printershare-list-jobs.md) | [printJob](printjob.md) 集合 | 获取打印机Share 排队处理的打印作业列表。 |
| [创建作业](../api/printershare-post-jobs.md) | [printJob](printjob.md) | 为 printerShare 创建新的打印作业。 若要开始打印作业，请使用 [“开始](../api/printjob-start.md)”。 |
| [列出 allowedUsers](../api/printershare-list-allowedusers.md) | [user](user.md) 集合 | 检索已被授予访问权限的用户列表，以便将打印作业提交到关联的打印机共享。 |
| [添加 allowedUser](../api/printershare-post-allowedusers.md) | 无 | 授予指定的用户访问权限，以便将打印作业提交到关联的打印机共享。 |
| [删除 allowedUser](../api/printershare-delete-alloweduser.md) | 无 | 从指定用户撤消打印机共享访问权限。 |
| [列出 allowedGroups](../api/printershare-list-allowedgroups.md) | [group](group.md) 集合 | 检索已授予访问权限的组列表，以便将打印作业提交到关联的打印机共享。 |
| [添加 allowedGroup](../api/printershare-post-allowedgroups.md) | 无 | 授予指定的组访问权限，以便将打印作业提交到关联的打印机共享。 |
| [删除 allowedGroup](../api/printershare-delete-allowedgroup.md) | 无 | 从指定组撤消打印机共享访问权限。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| printerShare 的标识符。 只读。|
|displayName|字符串|打印客户端应显示的打印机共享的名称。|
|createdDateTime|DateTimeOffset|创建打印机共享时的 DateTimeOffset。 只读。|
|manufacturer|String|与此打印机共享关联的打印机报告的制造商。 只读。|
|model|String|与此打印机共享关联的打印机报告的模型名称。 只读。|
|isAcceptingJobs|Boolean|与此打印机共享关联的打印机当前是否接受新的打印作业。|
|defaults|[printerDefaults](printerdefaults.md)|与此打印机共享关联的打印机的默认打印设置。|
|capabilities|[printerCapabilities](printercapabilities.md)|与此打印机共享关联的打印机的功能。|
|位置|[printerLocation](printerlocation.md)|与此打印机共享关联的打印机的物理和/或组织位置。|
|状态|[printerStatus](printerstatus.md)|与此打印机共享关联的打印机的处理状态（包括任何错误）。 只读。|
|allowAllUsers|Boolean|如果为 true，则将向所有用户和组授予对此打印机共享的访问权限。 这会取代 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。|

## <a name="relationships"></a>关系
| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|打印机|[打印机](printer.md)|此打印机共享的打印机与之相关。 |
|allowedUsers|[user](user.md) 集合|有权使用打印机打印的用户。|
|allowedGroups|[组](group.md)|用户有权使用打印机打印的组。|
|jobs|[printJob](printjob.md) 集合| 与此打印机共享关联的打印机排队打印的作业列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


