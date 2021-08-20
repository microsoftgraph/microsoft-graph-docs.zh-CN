---
title: accessPackageAssignmentRequestRequirements 资源类型
description: 标识请求指定访问包所需的要求。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: febe429bb3c29da1a58454bb2758ee0fae16735b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259264"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>accessPackageAssignmentRequestRequirements 资源类型

命名空间：microsoft.graph

表示调用方必须满足的要求，才能成功为指定为 URL 一部分的 **accessPackage** 创建 **accessPackageAssignmentRequest。** 要求通过评估与 **accessPackage** 关联的策略来确定。 

## <a name="properties"></a>属性
| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| existingAnswers | [accessPackageAnswer](../resources/accesspackageanswer.md) 集合  | 已提供的答案。 |
| isApprovalRequired | 布尔值 | 指示请求是否必须由审批者批准。 |
| isApprovalRequiredForExtension  | 布尔值 | 指示用户尝试扩展其访问权限时是否需要审批。 |
| isCustomAssignmentScheduleAllowed | 布尔值 | 指示是否允许请求者设置自定义计划。 |
| isRequestorJustificationRequired | 布尔值 | 指示请求者在提交分配请求时是否必须提供理由。 |
| policyDescription | String | 用户尝试使用请求访问的策略的说明。  |
| policyDisplayName | String | 用户显示名称请求访问权限的策略的一部分。 |
| policyId | String | 与这些要求关联的策略的标识符。 创建新分配请求时，可以使用此标识符。 |
| 问题 | [accessPackageQuestion](../resources/accesspackagequestion.md) 集合 | 在策略上配置的问题。 问题可以是必需问题，也可以是可选的;调用方可以基于 **accessPackageQuestion** 的 **isRequired** 属性来确定问题是必需还是可选。 |
| schedule | [requestSchedule](../resources/requestschedule.md) | 强制执行计划限制（如果有）。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements" 
}-->

``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequired": false,
  "isApprovalRequiredForExtension": false,
  "isCustomAssignmentScheduleAllowed": false,
  "isRequestorJustificationRequired": false,
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "questions": [
    {
      "@odata.type": "microsoft.graph.accessPackageQuestion"
    }
  ],
  "existingAnswers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ]
}
```
