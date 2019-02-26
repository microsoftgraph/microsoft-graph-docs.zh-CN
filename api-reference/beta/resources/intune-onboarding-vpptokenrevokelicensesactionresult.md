---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 在 Apple volume purchase program 令牌上执行的吊销许可证操作的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3ccf2bfd72ae9f6aeb85e3a7228faac09a8b2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158168"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在 Apple volume purchase program 令牌上执行的吊销许可证操作的状态。


继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionName|String|从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作名称|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)的操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。|
|startDateTime|DateTimeOffset|从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作的开始时间|
|lastUpdatedDateTime|DateTimeOffset|上次更新操作状态的时间从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承|
|totalLicensesCount|Int32|试图吊销的许可证数量的计数。|
|failedLicensesCount|Int32|无法撤消的许可证数量的计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|吊销许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|

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




