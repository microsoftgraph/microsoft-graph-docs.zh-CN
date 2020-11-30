---
title: cloudPcManagementGroupAssignmentTarget 资源类型
description: 代表工作分配目标组的复杂类型。 基本类型： CloudPcManagementAssignmentTarget
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378326"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>cloudPcManagementGroupAssignmentTarget 资源类型

命名空间：microsoft.graph

代表工作分配目标组的复杂类型。
继承自 [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)。

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
