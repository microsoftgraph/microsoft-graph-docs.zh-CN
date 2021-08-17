---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 ID 类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 619e2cd7a933994703f4beee13c6356fc31a5a320d6797455813e7e409f16f1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209923"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a>deliveryOptimizationGroupIdCustom 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义组 ID 类型


继承自 [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupIdCustom|String|指定设备所属的任意组 ID|

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




