---
title: deviceHealthScriptIntegerParameter 资源类型
description: Integer 脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fda0fe9a937867ea2f61bdd0d0a2bec491ba7515
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58751935"
---
# <a name="devicehealthscriptintegerparameter-resource-type"></a>deviceHealthScriptIntegerParameter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Integer 脚本参数的属性。


继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|参数的名称 继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|String|参数的说明 继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Boolean|参数是否必需 继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|applyDefaultValueWhenNotAssigned|Boolean|未分配时是否应用默认值 继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|defaultValue|Int32|Integer 参数的默认值。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": 1024
}
```



