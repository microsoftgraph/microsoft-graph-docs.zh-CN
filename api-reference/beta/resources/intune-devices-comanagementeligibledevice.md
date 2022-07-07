---
title: comanagementEligibleDevice 资源类型
description: 设备Co-Management资格状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d9c17a3de8a1b2d3bf30874f0202cf432447ef6
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670819"
---
# <a name="comanagementeligibledevice-resource-type"></a>comanagementEligibleDevice 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备Co-Management资格状态

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List comanagementEligibleDevices](../api/intune-devices-comanagementeligibledevice-list.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 集合|列出 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象的属性和关系。|
|[获取 comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-get.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|读取 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象的属性和关系。|
|[创建 comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-create.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|创建新的 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象。|
|[删除 comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-delete.md)|None|删除 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)。|
|[更新 comanagementEligibleDevice](../api/intune-devices-comanagementeligibledevice-update.md)|[comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md)|更新 [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备的唯一 ID|
|deviceName|String|DeviceName|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|DeviceType。 可能的值为：`desktop`、`windowsRT`、`winMO6`、`nokia`、`windowsPhone`、`mac`、`winEmbedded``winCE`、、`iPhone`、`iPad`、`iPod`、`iSocConsumer``android`、`unix`、`macMDM``holoLens`、`surfaceHub`、、`androidForWork`、 `unknown``cloudPC``palm``androidEnterprise``windows10x``androidnGMS``chromeOS``linux``blackberry`|
|clientRegistrationStatus|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|ClientRegistrationStatus。 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|OwnerType。 可取值为：`unknown`、`company`、`personal`。|
|managementAgents|[managementAgentType](../resources/intune-shared-managementagenttype.md)|ManagementAgents。 可能的值为：`eas`、、`mdm`、`easMdm``intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`unknown``configurationManagerClientMdmEas`、`jamf`、`googleCloudDevicePolicyController``microsoft365ManagedMdm`、、`msSense`。 `intuneAosp`|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|ManagementState。 可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。|
|referenceId|String|ReferenceId|
|mdmStatus|String|MDMStatus|
|osVersion|String|OSVersion|
|serialNumber|String|序列号|
|manufacturer|String|制造商|
|model|String|模型|
|osDescription|String|OSDescription|
|entitySource|Int32|EntitySource|
|userId|字符串|UserId|
|Upn|字符串|UPN|
|userEmail|String|UserEmail|
|userName|String|UserName|
|status|[comanagementEligibleType](../resources/intune-devices-comanagementeligibletype.md)|ComanagementEligibleStatus。 可取值为：`comanaged`、`eligible`、`eligibleButNotAzureAdJoined`、`needsOsUpdate`、`ineligible`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "String (identifier)",
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
  "status": "String"
}
```




