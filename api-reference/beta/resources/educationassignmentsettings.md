---
title: educationAssignmentSettings 资源类型
description: 指定类级分配设置。
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fe1a8cf70f717df396bf8b336f3a543770a4da71
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684877"
---
# <a name="educationassignmentsettings-resource-type"></a>educationAssignmentSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定类级分配设置。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|读取 [educationAssignmentSettings 对象的](../resources/educationassignmentsettings.md) 属性和关系。|
|[更新 educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|更新 [educationAssignmentSettings 对象的](../resources/educationassignmentsettings.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|educationAssignmentSettings 的唯一标识符。|
|submissionAnimationDisabled|Boolean|指示是否将显示入场庆祝动画。 指示不会显示动画的 `true` 值。 默认值为 `false`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "submissionAnimationDisabled": false
}
```

