---
title: deviceManagementEnumConstraint 资源类型
description: 强制实施设置值的约束来自允许的一组字符串
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2979f189921c0c9e7240cc5287a072b27e12b96e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943429"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>deviceManagementEnumConstraint 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

强制实施设置值的约束来自允许的一组字符串


继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)集合|此字符串的有效值列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```




