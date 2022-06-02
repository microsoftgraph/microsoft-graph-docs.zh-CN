---
title: deviceScopeActionResult 资源类型
description: 触发的设备范围操作的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6938869b658edb1d0fddc4dfa753e45cb1fb8eb5
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858547"
---
# <a name="devicescopeactionresult-resource-type"></a>deviceScopeActionResult 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

触发的设备范围操作的结果。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceScopeAction|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|触发的操作名称。 可能的值为： .|
|deviceScopeId|String|触发操作的设备范围的唯一标识符。|
|status|[deviceScopeActionStatus](../resources/intune-devices-devicescopeactionstatus.md)|指示尝试设备作用域操作的状态。 成功后，操作被成功触发，失败时，操作无法触发。 可取值为：`failed`、`succeeded`、`unknownFutureValue`。|
|failedMessage|String|该消息指示设备范围操作无法触发的原因。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceScopeActionResult"
}
-->
``` json
{
  "@odata.type": "microsoft.graph.deviceScopeActionResult",
  "deviceScopeAction": "String",
  "deviceScopeId": "String",
  "status": "String",
  "failedMessage": "String"
}
```




