---
title: cloudPcBulkRemoteActionResult 资源类型
description: 表示云电脑指定的批量远程操作结果。
author: rongting
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 46f1336ec8f8cfa53813a73ac1230767f3a2e937
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338837"
---
# <a name="cloudpcbulkremoteactionresult-resource-type"></a>cloudPcBulkRemoteActionResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑指定的批量远程操作结果。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|failedDeviceIds|字符串集合|完成批量操作但失败的所有 Intune 托管设备 ID 的列表。|
|notFoundDeviceIds|字符串集合|尝试批量操作时找不到的所有 Intune 托管设备 ID 的列表。|
|notSupportedDeviceIds|String collection|标识为不支持批量操作的所有 Intune 托管设备标识的列表。|
|successfulDeviceIds|字符串集合|成功完成批量操作的所有 Intune 托管设备 ID 的列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcBulkRemoteActionResult",
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ],
  "successfulDeviceIds": [
    "String"
  ]
}
```

