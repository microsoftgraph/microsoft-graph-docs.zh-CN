---
title: educationAssignmentSettings 资源类型
description: 指定课堂级别作业设置。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c670cb2bbef0b82ff80996e4acb52c2826ec118f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034333"
---
# <a name="educationassignmentsettings-resource-type"></a>educationAssignmentSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定课堂级别作业设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|读取 [educationAssignmentSettings 对象的属性和](../resources/educationassignmentsettings.md) 关系。|
|[更新 educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|submissionAnimationDisabled|布尔|指示是否显示打开的庆祝动画。 值 `true` 指示不会显示动画。 默认值为 `false`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

