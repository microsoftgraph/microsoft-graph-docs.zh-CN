---
title: cloudPcRemoteActionResult 资源类型
description: 表示云电脑指定的远程操作结果。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9b708df825104cd85175543b7c16850c16d40d0d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336023"
---
# <a name="cloudpcremoteactionresult-resource-type"></a>cloudPcRemoteActionResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑指定的远程操作结果。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[getCloudPcRemoteActionResults](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|检查云电脑指定的远程操作结果。 云电脑支持重新设置远程操作并调整其大小。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|actionName|String|指定的操作。 网站门户中Microsoft Endpoint Manager的值是：、`Reprovision`、`Resize``Restore`。 企业云电脑设备中支持的值包括：、`Reboot`、`Rename`、`Reprovision``Troubleshoot`。|
|actionState|[actionState](#actionstate-values)|操作的状态。 可能的值是：`None`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。 只读。|
|cloudPcId|String|执行远程操作云电脑设备的 ID。 只读。|
|managedDeviceId|String|执行远程操作 Intune 托管设备的 ID。 只读。|
|startDateTime|DateTimeOffset|启动操作的时间。 时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。 例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。|
|lastUpdatedDateTime|DateTimeOffset|操作的最后更新时间。 时间戳以 ISO 8601 格式和 UTC 协调世界时 (显示) 。 例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcStatusDetails.md)|云电脑状态的详细信息。 |

### <a name="actionstate-values"></a>actionState 值

|成员|说明|
|:---|:---|
|无|操作状态无效。|
|pending|操作挂起。|
|canceled|操作已取消。|
|active|操作处于活动状态。|
|done|操作已完成，没有错误。|
|failed|操作失败。|
|notSupported|不支持操作。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRemoteActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "cloudPcId": "String",
  "managedDeviceId": "String",
  "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails"
  }
}
```
