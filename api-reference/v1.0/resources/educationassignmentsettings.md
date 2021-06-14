---
title: educationAssignmentSettings 资源类型
description: 指定课堂级别的作业设置。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ccaa51c84e50e2f9c5302836ffd9b92754f517fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912353"
---
# <a name="educationassignmentsettings-resource-type"></a>educationAssignmentSettings 资源类型

命名空间：microsoft.graph

指定课堂级别的作业设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentSettings](../api/educationassignmentsettings-get.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|读取 [educationAssignmentSettings 对象的属性和](../resources/educationassignmentsettings.md) 关系。|
|[更新 educationAssignmentSettings](../api/educationassignmentsettings-update.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|submissionAnimationDisabled|Boolean|指示是否显示打开的庆祝动画。 的值 `true` 指示不会显示动画。 默认值为 `false`。|

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

