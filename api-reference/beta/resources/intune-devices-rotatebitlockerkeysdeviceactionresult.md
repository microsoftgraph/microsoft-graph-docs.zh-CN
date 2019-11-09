---
title: rotateBitLockerKeysDeviceActionResult 资源类型
description: RotateBitLockerKeys 设备操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 46b0f00f38e453edbd2e5214a1fe1e900a418639
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088243"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a>rotateBitLockerKeysDeviceActionResult 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

RotateBitLockerKeys 设备操作结果


继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|actionName|String|操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|startDateTime|DateTimeOffset|操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|errorCode|Int32|RotateBitLockerKeys 操作错误代码|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```



