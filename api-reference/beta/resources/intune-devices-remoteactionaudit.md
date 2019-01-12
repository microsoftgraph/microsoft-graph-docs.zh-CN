---
title: remoteActionAudit 资源类型
description: 属于某些租户的设备上启动远程操作的报告。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad583f13311e5baece70c5ec28ca8f7c73f5349e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972591"
---
# <a name="remoteactionaudit-resource-type"></a>remoteActionAudit 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

属于某些租户的设备上启动远程操作的报告。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合|列出属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象之间的关系。|
|[获取 remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|读取属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的关系。|
|[创建 remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。|
|[删除 remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|无|删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。|
|[更新 remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|报告 id。|
|deviceDisplayName|String|Intune 设备名称。|
|userName|String|\[弃用的\]请改用 InitiatedByUserPrincipalName。|
|initiatedByUserPrincipalName|字符串|用户启动的设备操作，格式为 UPN。|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|操作名称。 可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.|
|requestDateTime|DateTimeOffset|发布该操作时，给定采用 UTC 时间。|
|deviceOwnerUserPrincipalName|字符串|设备所有者的 Upn。|
|deviceIMEI|字符串|设备的 IMEI。|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|操作状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|

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
  "actionState": "String"
}
```





