---
title: assignmentReviewSettings 资源类型
description: 用于访问包分配策略的 accessReviewSettings 属性的 assignmentReviewSettings 类型提供了其他设置，用于选择必须从此策略查看访问包分配以及必须查看访问包分配多久查看一次。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bde8c6d330eda7e100071edbf2190e170ca913ea
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131320"
---
# <a name="assignmentreviewsettings-resource-type"></a>assignmentReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 **访问包分配策略的 accessReviewSettings** [属性](accesspackageassignmentpolicy.md)。 提供其他设置，以选择必须从此策略查看访问包分配的人，以及必须查看访问包分配频繁。  

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Boolean | 如果为 true，则此策略中的分配需要访问评审。 |
| recurrenceType | 字符串 | 定期的间隔，例如或 `monthly` `quarterly` 。 |
| reviewerType | 字符串 | 应要求谁执行审阅，或者 `Self` `Reviewers` 。 |
| startDateTime | DateTimeOffset | 第一次审阅应何时开始。 |
| durationInDays | Int32 | 允许审阅者输入的天数。|
| 审阅者 | [userSet](userset.md) 集合 | 如果 reviewerType 为，则此集合使用 `Reviewers` [singleUser](singleuser.md) 和 [groupMembers](groupmembers.md)集合指定将按 ID 或作为组的成员成为审阅者的用户。 |

## <a name="json-representation"></a>JSON 表示形式


以下是策略的访问评审设置属性的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
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


