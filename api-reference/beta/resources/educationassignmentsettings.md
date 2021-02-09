---
title: educationAssignmentSettings 资源类型
description: 指定课堂级别作业设置。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5990453eefbe63013ecfa0be03ff5b4d99330fa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153640"
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
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

