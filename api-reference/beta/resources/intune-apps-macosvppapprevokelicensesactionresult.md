---
title: macOsVppAppRevokeLicensesActionResult 资源类型
description: 定义对 MacOS Vpp 应用的操作的结果，包含 ActionResult 的继承属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8044581eaf8ae41e7b3353f599c5f2a68c50964a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129129"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>macOsVppAppRevokeLicensesActionResult 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

定义对 MacOS Vpp 应用的操作的结果，包含 ActionResult 的继承属性。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|userId|String|与操作关联的 UserId。|
|managedDeviceId|String|与操作关联的 DeviceId。|
|totalLicensesCount|Int32|已尝试撤销的许可证数量计数。|
|failedLicensesCount|Int32|撤销失败的许可证数量计数。|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|撤销许可证操作失败的原因。 可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。|
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



