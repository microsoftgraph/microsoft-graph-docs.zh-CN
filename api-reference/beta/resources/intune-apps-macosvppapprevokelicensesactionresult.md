---
title: macOsVppAppRevokeLicensesActionResult 资源类型
description: 定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b87808428b53e61cd4f13d6686ea94719ce44313
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797991"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>macOsVppAppRevokeLicensesActionResult 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userId|String|与操作关联的用户 Id。|
|managedDeviceId|String|与操作相关联的 DeviceId。|
|totalLicensesCount|Int32|尝试吊销的许可证数量的计数。|
|failedLicensesCount|Int32|吊销失败的许可证数的计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|吊销许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|
|actionName|String|操作名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|startDateTime|DateTimeOffset|初始化操作的时间|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



