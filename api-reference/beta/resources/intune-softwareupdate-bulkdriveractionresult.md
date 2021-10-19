---
title: bulkDriverActionResult 资源类型
description: 表示批量驱动程序操作结果的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3332c2856968aa5ddcc7841a555f37ae9638496
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494947"
---
# <a name="bulkdriveractionresult-resource-type"></a>bulkDriverActionResult 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示批量驱动程序操作结果的复杂类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|successfulDriverIds|String 集合|操作成功的驱动程序 ID 列表。|
|failedDriverIds|String 集合|操作失败位置的驱动程序 ID 列表。|
|notFoundDriverIds|String collection|未找到的驱动程序 ID 列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkDriverActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkDriverActionResult",
  "successfulDriverIds": [
    "String"
  ],
  "failedDriverIds": [
    "String"
  ],
  "notFoundDriverIds": [
    "String"
  ]
}
```



