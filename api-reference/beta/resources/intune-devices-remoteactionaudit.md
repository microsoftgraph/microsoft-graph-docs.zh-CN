---
title: remoteActionAudit 资源类型
description: 在属于特定租户的设备上启动的远程操作的报告。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd3e1acabcc5c4e51a4febb307eb0084e1f03292
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081078"
---
# <a name="remoteactionaudit-resource-type"></a>remoteActionAudit 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在属于特定租户的设备上启动的远程操作的报告。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 集合|列出 [remoteActionAudit 对象的属性和](../resources/intune-devices-remoteactionaudit.md) 关系。|
|[获取 remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|读取 [remoteActionAudit 对象的属性和](../resources/intune-devices-remoteactionaudit.md) 关系。|
|[创建 remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|创建新的 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象。|
|[删除 remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|无|删除 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。|
|[更新 remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|更新 [remoteActionAudit 对象](../resources/intune-devices-remoteactionaudit.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|报告 ID。|
|deviceDisplayName|String|Intune 设备名称。|
|userName|String|\[已弃用 \] 请改为使用 InitiatedByUserPrincipalName。|
|initiatedByUserPrincipalName|String|启动设备操作的用户，格式为 UPN。|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|操作名称。 可能的值是 `unknown` `factoryReset` ：、、、、、、、、、、。 `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` `activateDeviceEsim`|
|requestDateTime|DateTimeOffset|发出操作的时间（以 UTC 表示）。|
|deviceOwnerUserPrincipalName|String|设备所有者的 Upn。|
|deviceIMEI|String|设备的 IMEI。|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|操作状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|managedDeviceId|String|操作目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String",
  "managedDeviceId": "String"
}
```



