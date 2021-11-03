---
title: assignmentFilterEvaluateRequest 资源类型
description: 请求评估设备的分配筛选器。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7a3af607c2d809f32e064b45bfaef9d6057f241f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697223"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>assignmentFilterEvaluateRequest 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求评估设备的分配筛选器。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|平台|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|工作分配筛选器适用的设备的平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|rule|String|工作分配筛选器的规则定义。|
|top|Int32|每个请求的记录限制。 如果提供小于 0 或大于 100，则默认值为 100|
|skip|Int32|要跳过的记录数。 默认值为 0|

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
  "skip": 1024
}
```



