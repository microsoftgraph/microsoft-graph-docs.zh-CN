---
title: deviceManagementIntentDeviceState 资源类型
description: 表示意图的设备状态的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30cb1fcb0d8078ad6707a535a687cc617c9f0bcd1175f4437b959800d7edb744
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164221"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a>deviceManagementIntentDeviceState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示意图的设备状态的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntentDeviceStates](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 集合|列出 [deviceManagementIntentDeviceState 对象的属性和](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 关系。|
|[获取 deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|读取 [deviceManagementIntentDeviceState 对象的属性和](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 关系。|
|[创建 deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|创建新的 [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 对象。|
|[删除 deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|无|删除 [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)。|
|[更新 deviceManagementIntentDeviceState](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|更新 [deviceManagementIntentDeviceState 对象](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|The ID|
|userPrincipalName|字符串|在设备上报告的用户主体名称|
|userName|String|在设备上报告的用户名|
|deviceDisplayName|String|报告的设备名称|
|lastReportedDateTime|DateTimeOffset|意图报告的上次修改日期时间|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|意图的设备状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|deviceId|String|报告的设备 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```




