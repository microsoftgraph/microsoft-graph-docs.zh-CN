---
title: comanagementEligibleDeviceEntity 资源类型
description: comanagementEligibleDeviceEntity 资源类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5ad068a348eabaceafd9ca736f27cf6fda3218e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636551"
---
# <a name="comanagementeligibledeviceentity-resource-type"></a>comanagementEligibleDeviceEntity 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的托管设备移动应用配置状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 comanagementEligibleDeviceEntity](../api/intune-device-comanagementEligibleDeviceEntity-list.md)|[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)集合|列出[comanagementEligibleDeviceEntity](../resources/intune-device-comanagementEligibleDeviceEntity.md)对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|EligibleDeviceEntity 的唯一 Id|
|deviceId|字符串|DeviceId|
|deviceName|字符串|DeviceName|
|deviceType|String|DeviceType|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus. 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|所有者|[所有者](../resources/intune-shared-ownertype.md)|所有者. 可取值为：`unknown`、`company`、`personal`。|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgentType. 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|ManagementState. 可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。|
|referenceId|字符串|ReferenceId|
|mdmStatus|字符串|MDMStatus|
|osVersion|字符串|OSVersion|
|serialNumber|String|序列号|
|manufacturer|字符串|负责|
|model|字符串|模型|
|osDescription|字符串|OSDescription|
|entitySource|Int32|EntitySource|
|userId|String|UserId|
|upn|字符串|UPN|
|userEmail|字符串|UserEmail|
|userName|字符串|UserName|
|coManageEligibleStatus|[coManagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|CoManagementEligibleType. 可取值为：`coManaged`、`eligible`、`eligibleButNotAadJoined`、`needsOSUpdate`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDeviceEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "clientRegistrationStatus": "String",
  "ownerType": "String",
  "managementAgents": "String",
  "managementState": "String",
  "referenceId": "String",
  "mdmStatus": "String",
  "osVersion": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "osDescription": "String",
  "entitySource": 1024,
  "userId": "String",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "coManageEligibleStatus": "String"
}
```

