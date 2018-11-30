---
title: deviceActionResult 资源类型
description: 设备操作结果
ms.openlocfilehash: ac37cdff8ec323dfb8a2019b383d506c1b7e1076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042739"
---
# <a name="deviceactionresult-resource-type"></a>deviceActionResult 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

设备操作结果
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
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
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





