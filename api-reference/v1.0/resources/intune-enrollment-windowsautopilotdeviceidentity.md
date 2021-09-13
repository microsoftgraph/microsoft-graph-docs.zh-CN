---
title: windowsAutopilotDeviceIdentity 资源类型
description: windowsAutopilotDeviceIdentity 资源表示一Windows Autopilot 设备。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd481a0b527e9665e145a48a23b41b6a2aab24f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028917"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

windowsAutopilotDeviceIdentity 资源表示一Windows Autopilot 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合|列出 [windowsAutopilotDeviceIdentity 对象的属性和](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 关系。|
|[获取 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|读取 [windowsAutopilotDeviceIdentity 对象的属性和](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 关系。|
|[创建 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。|
|[删除 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|None|删除 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)。|
|[assignUserToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|None|将用户分配给 Autopilot 设备。|
|[unassignUserFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None|取消分配 Autopilot 设备中的用户。|
|[updateDeviceProperties 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|None|更新 Autopilot 设备上的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|groupTag|String|autopilot Windows组标记。|
|purchaseOrderIdentifier|String|Purchase Order Autopilot Windows标识符。|
|serialNumber|String|Windows autopilot 设备序列号。|
|productKey|String|Windows autopilot 设备产品密钥。|
|manufacturer|String|autopilot Windows Oem 制造商。|
|model|String|autopilot Windows型号名称。|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Autopilot 设备的 intune Windows状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`。|
|lastContactedDateTime|DateTimeOffset|Intune Autopilot 设备的上次Windows日期时间。|
|addressableUserName|String|可地址用户名。|
|userPrincipalName|String|用户主体名称。|
|resourceName|String|资源名称。|
|skuNumber|String|SKU 号|
|systemFamily|String|系统系列|
|azureActiveDirectoryDeviceId|String|AAD 设备 ID - 已弃用|
|managedDeviceId|String|托管设备 ID|
|displayName|String|显示名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String"
}
```




