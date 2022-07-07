---
title: assignmentFilterEvaluateRequest 资源类型
description: 请求设备的分配筛选器评估。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a3dde68384dcf9813167544a8d2b56c8db7a98e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666856"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>assignmentFilterEvaluateRequest 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求设备的分配筛选器评估。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|平台|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|工作分配筛选器将适用的设备的平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|规则|String|工作分配筛选器的规则定义。|
|top|Int32|每个请求的记录限制。 如果提供的值小于 0 或大于 100，则默认值为 100|
|skip|Int32|要跳过的记录数。 默认值为 0|
|orderBy|字符串集合|对设备进行排序。 默认值在设备名称上升序。|
|search|String|应用于已找到的范围设备的搜索关键字。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluateRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluateRequest",
  "platform": "String",
  "rule": "String",
  "top": 1024,
  "skip": 1024,
  "orderBy": [
    "String"
  ],
  "search": "String"
}
```




