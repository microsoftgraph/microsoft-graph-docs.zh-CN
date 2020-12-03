---
title: cloudPcManagementGroupAssignmentTarget 资源类型
description: 代表工作分配目标组的复杂类型。 基本类型： CloudPcManagementAssignmentTarget
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563843"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>cloudPcManagementGroupAssignmentTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表工作分配目标组的复杂类型。
继承自 [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|groupId|String|工作分配的目标组的 id|

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
