---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 在 Apple 卷购买计划令牌上执行吊销许可证操作的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418223"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在 Apple 卷购买计划令牌上执行吊销许可证操作的状态。


继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionName|String|操作名称继承[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|初始化的操作的时间从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承|
|lastUpdatedDateTime|DateTimeOffset|上次使用的操作状态的时间从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)更新继承|
|totalLicensesCount|Int32|已尝试撤消的许可证数的计数。|
|failedLicensesCount|Int32|无法撤消的许可证数的计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Revoke 许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




