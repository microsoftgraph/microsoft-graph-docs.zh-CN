---
title: assignmentFilterEvaluationSummary 资源类型
description: 表示工作分配筛选器评估的结果摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f2e93f481f0b21689b1a83d63f4540c22f50cb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160287"
---
# <a name="assignmentfilterevaluationsummary-resource-type"></a>assignmentFilterEvaluationSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示工作分配筛选器评估的结果摘要

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignmentFilterId|String|分配筛选器对象的唯一标识符|
|assignmentFilterLastModifiedDateTime|DateTimeOffset|上次修改工作分配筛选器的时间。|
|assignmentFilterDisplayName|String|管理员为分配筛选器定义的名称。|
|assignmentFilterPlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|创建此分配筛选器的平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|evaluationResult|[assignmentFilterEvaluationResult](../resources/intune-policyset-assignmentfilterevaluationresult.md)|工作分配筛选器评估结果。 可取值为：`unknown`、`match`、`notMatch`、`inconclusive`、`failure`、`notEvaluated`。|
|evaluationDateTime|DateTimeOffset|已评估时间分配筛选器。|
|assignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|指示包含或排除的筛选器类型。 可取值为：`none`、`include`、`exclude`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationSummary",
  "assignmentFilterId": "String",
  "assignmentFilterLastModifiedDateTime": "String (timestamp)",
  "assignmentFilterDisplayName": "String",
  "assignmentFilterPlatform": "String",
  "evaluationResult": "String",
  "evaluationDateTime": "String (timestamp)",
  "assignmentFilterType": "String"
}
```




