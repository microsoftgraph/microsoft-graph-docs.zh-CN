---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f64f2df709d5332be46dd76216b1a1457d27a61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418902"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>iosVppAppRevokeLicensesActionResult 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userId|String|与操作关联的用户 Id。|
|managedDeviceId|String|DeviceId 与操作关联。|
|totalLicensesCount|Int32|Revoke 尝试建立为其许可证数的计数。|
|failedLicensesCount|Int32|失败的吊销许可证数的计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Revoke 许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|
|actionName|String|操作名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|初始化操作的时间|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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




