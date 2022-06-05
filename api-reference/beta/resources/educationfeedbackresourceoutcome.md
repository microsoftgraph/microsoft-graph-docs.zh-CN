---
title: educationFeedbackResourceOutcome 资源类型
description: 以文档的形式表示有关 educationOutcome 对象的反馈。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0cad7a6e8c2f0527dd89ce624fac5652c6ac544b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900545"
---
# <a name="educationfeedbackresourceoutcome-resource-type"></a>educationFeedbackResourceOutcome 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以文档的形式表示有关 [educationOutcome](educationoutcome.md) 对象的反馈。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-post-outcomes.md) | [educationOutcome](educationoutcome.md) | 为提交创建新的 [反馈资源](../resources/educationfeedbackresourceoutcome.md) 。 |
| [删除 educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-delete.md) | 无 | 从提交中删除 [反馈资源](../resources/educationfeedbackresourceoutcome.md) 。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|feedbackResource|[educationResource](educationresource.md)|实际反馈资源。|
|id|String|**educationFeedbackResourceOutcome** 的唯一标识符。|
|resourceStatus|educationFeedbackResourceOutcomeStatus|反馈资源的状态。 可能的值是： `notPublished`、 `pendingPublish`、 `published`、 `failedPublish`和 `unknownFutureValue`。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackResourceOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedbackResource": {"@odata.type": "microsoft.graph.educationResource"},
  "id": "String (identifier)",
  "resourceStatus": {"@odata.type": "microsoft.graph.educationFeedbackResourceOutcomeStatus"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2022-05-05 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackResourceOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
