---
title: cloudPcManagementGroupAssignmentTarget 资源类型
description: 表示工作分配目标组的复杂类型。 基本类型：CloudPcManagementAssignmentTarget
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a3841cc775b1b0ed9221d193a5ca5d44c61bc6f0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765660"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>cloudPcManagementGroupAssignmentTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作分配目标组的复杂类型。
继承自 [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|groupId|String|工作分配的目标组的 ID|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
