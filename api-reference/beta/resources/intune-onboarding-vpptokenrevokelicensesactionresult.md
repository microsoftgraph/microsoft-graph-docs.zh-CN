---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 对 Apple Volume Purchase Program 令牌执行的撤销许可证操作的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd08741b48e81afa4a3775fdb3cd4ed160e0e6b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790617"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>vppTokenRevokeLicensesActionResult 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对 Apple Volume Purchase Program 令牌执行的撤销许可证操作的状态。


继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionName|String|操作名称 继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|操作的状态 继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|startDateTime|DateTimeOffset|操作启动时间 继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|上次更新操作状态的时间 继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|totalLicensesCount|Int32|尝试撤销的许可证数量计数。|
|failedLicensesCount|Int32|未能撤销的许可证数量计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|撤销许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|

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



