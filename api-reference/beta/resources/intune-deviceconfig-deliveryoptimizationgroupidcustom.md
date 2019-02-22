---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 id 类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177971"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a>deliveryOptimizationGroupIdCustom 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义组 id 类型


继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupIdCustom|字符串|指定设备所属的任意组 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




