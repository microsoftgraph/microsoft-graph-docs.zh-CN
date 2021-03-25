---
title: assignmentFilterState 资源类型
description: 表示 GetState API 的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 969d902635962a9ff89bb197f32e7d995dd9b35f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159376"
---
# <a name="assignmentfilterstate-resource-type"></a>assignmentFilterState 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 GetState API 的结果。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|已启用|Boolean|指示 AssignmentFilter 是启用还是禁用的指示器。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterState",
  "enabled": true
}
```




