---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c1d8805e54a194eeb584bb980ed8082502b4a872
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895630"
---
# <a name="printer-resource-type"></a>打印机资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取打印机](../api/printer-get.md) | [印刷](printer.md) | 读取 printer 对象的属性和关系。 |
| [更新](../api/printer-update.md) | [印刷](printer.md) | 更新 printer 对象。 |
| [删除](../api/printer-delete.md) | 无 | 在通用打印服务中注销物理 printerfrom。 |
| [getCapabilities](../api/printer-getcapabilities.md) | [printerCapabilities](printercapabilities.md) | 获取打印机的功能列表。 |
| [resetDefaults](../api/printer-resetdefaults.md) | 无 | 重置打印机的默认设置。 |
| [列出作业](../api/printer-list-jobs.md) | [printJob](printjob.md)集合 | 获取排队等待打印机处理的打印作业的列表。 |
| [创建作业](../api/printer-post-jobs.md) | [printJob](printjob.md) | 为打印机创建一个新的打印作业。 若要开始打印作业，请使用[startPrintJob](../api/printjob-startprintjob.md)。 |
| [列出连接器](../api/printer-list-connectors.md) | [printConnector](printconnector.md)集合 | 获取此打印机关联的连接器的列表。 |
| [列出 allowedUsers](../api/printer-list-allowedusers.md) | [userIdentity](useridentity.md)集合 | 检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。 |
| [添加 allowedUser](../api/printer-post-allowedusers.md) | 无 | 向指定的用户授予向关联打印机提交打印作业的权限。 |
| [删除 allowedUser](../api/printer-delete-alloweduser.md) | 无 | 撤销指定用户的打印机访问权限。 |
| [列出 allowedGroups](../api/printer-list-allowedgroups.md) | [标识](identity.md)集合 | 检索已向其授予将打印作业提交到关联打印机的访问权限的组列表。 |
| [添加 allowedGroup](../api/printer-post-allowedgroups.md) | 无 | 向指定的组授予向关联打印机提交打印作业的权限。 |
| [删除 allowedGroup](../api/printer-delete-allowedgroup.md) | 无 | 撤销指定组的打印机访问权限。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|文档的标识符。 只读。|
|name|String|打印机的名称。|
|manufacturer|String|打印机报告的制造商。 只读。|
|model|String|打印机报告的模型名称。 只读。|
|registeredBy|[userIdentity](useridentity.md)|注册打印机的用户。|
|registeredDateTime|DateTimeOffset|注册打印机时的 DateTimeOffset。 只读。|
|状态|[printerStatus](printerstatus.md)|打印机的处理状态，包括任何错误。 只读。|
|isShared|Boolean|如果打印机是共享的，则为 True;否则为 false。 只读。|
|acceptingJobs|布尔|打印机当前是否正在接受新的打印作业。|
|位置|[printerLocation](printerlocation.md)|打印机的物理和/或组织位置。|
|缺省值|[printerDefaults](printerdefaults.md)|打印机的默认打印设置。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|jobs|[printJob](printjob.md)集合| 打印机排队等待打印的作业的列表。 只读。 可为 NULL。|
|shares|[printerShare](printershare.md)| 与打印机关联的 printerShare。 只读。 可为 NULL。|
|插槽|[printConnector](printconnector.md)|与打印机关联的连接器。|
|allowedUsers|[userIdentity](useridentity.md)集合|有权使用打印机打印的用户。|
|allowedGroups|[identity](identity.md)|其用户有权使用打印机打印的组。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->