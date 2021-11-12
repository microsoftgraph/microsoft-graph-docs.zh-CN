---
title: printerShare 资源类型
description: 表示旨在供用户和打印应用程序发现的打印机。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 52d3bc8adedd8f05c4cc4493df533d074ce19f58
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944940"
---
# <a name="printershare-resource-type"></a>printerShare 资源类型

命名空间：microsoft.graph

表示旨在供用户和打印应用程序发现的打印机。

继承自 [printerBase](../resources/printerbase.md)。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [List](../api/print-list-shares.md) | [printerShare](printershare.md) 集合 | 获取租户中打印机共享的列表。 |
| [获取](../api/printershare-get.md) | [printerShare](printershare.md) | 读取 **printerShare** 对象的属性和关系。 |
| [更新](../api/printershare-update.md) | [printerShare](printershare.md) | 更新 **printerShare** 对象。 |
| [删除](../api/printershare-delete.md) | 无 | 取消共享打印机。 |
| [列出作业](../api/printershare-list-jobs.md) | [printJob](printjob.md) 集合 | 获取等待 printerShare 处理的打印作业列表。 |
| [创建作业](../api/printershare-post-jobs.md) | [printJob](printjob.md) | 为 printerShare 创建新的打印作业。 若要开始打印作业 [，请使用](../api/printjob-start.md)start 。 |
| [列出 allowedUsers](../api/printershare-list-allowedusers.md) | [user](user.md) 集合 | 检索已被授予将打印作业提交到关联的打印机共享的权限的用户的列表。 |
| [添加 allowedUser](../api/printershare-post-allowedusers.md) | 无 | 向指定的用户授予将打印作业提交到关联的打印机共享的权限。 |
| [删除 allowedUser](../api/printershare-delete-alloweduser.md) | 无 | 撤销指定用户的打印机共享访问权限。 |
| [列出 allowedGroups](../api/printershare-list-allowedgroups.md) | [group](group.md) 集合 | 检索已被授予将打印作业提交到关联的打印机共享的权限的组列表。 |
| [添加 allowedGroup](../api/printershare-post-allowedgroups.md) | 无 | 授予指定的组访问权限，以将打印作业提交到关联的打印机共享。 |
| [删除 allowedGroup](../api/printershare-delete-allowedgroup.md) | 无 | 从指定组撤消打印机共享访问权限。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| printerShare 的标识符。 继承自 [printerBase](../resources/printerbase.md)。 只读。|
|displayName|String|打印客户端应显示的打印机共享的名称。 继承自 [printerBase](../resources/printerbase.md)。|
|createdDateTime|DateTimeOffset|创建打印机共享时的日期时间Offset 。 只读。|
|manufacturer|String|与此打印机共享关联的打印机报告的制造商。 继承自 [printerBase](../resources/printerbase.md)。 只读。|
|model|String|与此打印机共享关联的打印机报告的型号名称。 继承自 [printerBase](../resources/printerbase.md)。 只读。|
|isAcceptingJobs|Boolean|与此打印机共享关联的打印机当前是否接受新的打印作业。 继承自 [printerBase](../resources/printerbase.md)。|
|defaults|[printerDefaults](printerdefaults.md)|与此打印机共享关联的打印机的默认打印设置。 继承自 [printerBase](../resources/printerbase.md)。|
|capabilities|[printerCapabilities](printercapabilities.md)|与此打印机共享关联的打印机的功能。 继承自 [printerBase](../resources/printerbase.md)。|
|位置|[printerLocation](printerlocation.md)|与此打印机共享关联的打印机的物理和/或组织位置。 继承自 [printerBase](../resources/printerbase.md)。|
|status|[printerStatus](printerstatus.md)|与此打印机共享关联的打印机的处理状态（包括任何错误）。继承自 [printerBase](../resources/printerbase.md)。 只读。|
|allowAllUsers|Boolean|如果为 true，将授予所有用户和组对此打印机共享的访问权限。 这将取代 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|打印机|[打印机](printer.md)|此打印机共享相关的打印机。 |
|allowedUsers|[user](user.md) 集合|有权访问使用打印机打印的用户。|
|allowedGroups|[group](group.md)|用户有权访问使用打印机打印的组。|
|jobs|[printJob](printjob.md) 集合| 由与此打印机共享关联的打印机排入打印队列的作业列表。|
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "allowAllUsers": "Boolean",
  "createdDateTime": "String (timestamp)"
}
```

