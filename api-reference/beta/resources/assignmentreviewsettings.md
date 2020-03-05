---
title: assignmentReviewSettings 资源类型
description: AssignmentReviewSettings type，用于访问包分配策略的 accessReviewSettings 属性，提供了其他设置，以选择必须查看此策略中的访问包分配的用户以及必须检查的频率。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a26728fb39fccd1512a559638c595551a20c0042
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508176"
---
# <a name="assignmentreviewsettings-resource-type"></a>assignmentReviewSettings 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于[访问包分配策略](accesspackageassignmentpolicy.md)的**accessReviewSettings**属性。 提供其他设置，以选择必须查看此策略中的访问包分配的用户以及必须查看的频率。  

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Boolean | 如果为 true，则此策略中的工作分配需要进行访问检查。 |
| recurrenceType | String | 定期的间隔，例如`monthly`或。 `quarterly` |
| reviewerType | String | 应要求谁是`Self`或`Reviewers`，由谁来进行审阅。 |
| startDateTime | DateTimeOffset | 第一次审阅应开始时。 |
| durationInDays | Int32 | 允许来自审阅者的输入的天数。|
| 审批 | [userSet](userset.md)集合 | 如果 reviewerType 是`Reviewers`，则此集合将使用[singleUser](singleuser.md)和[groupMembers](groupmembers.md)的集合指定将成为审阅者的用户（通过 ID 或作为组的成员）。 |

## <a name="json-representation"></a>JSON 表示形式


以下是策略的 "访问评审设置" 属性的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
