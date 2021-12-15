---
title: bookingQuestionAnswer 资源类型
description: 包含自定义问题、客户为自定义问题给出的答案，以及创建约会时自定义问题的属性。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1b62344b936c0c95b4e831c48c7b2d921c3033a0
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526640"
---
# <a name="bookingquestionanswer-resource-type"></a>bookingQuestionAnswer 资源类型

命名空间：microsoft.graph

包含自定义问题、客户为自定义问题给出的答案，以及创建约会时自定义问题的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|answer|String|如果 **answerInputType** 为 ，则用户给出的答案 `text` 为 。|
|answerInputType|answerInputType|预期的答案类型。 可能的值包括 `text`、`radioButton`、`unknownFutureValue`。|
|answerOptions|String collection|如果 **answerInputType** 为 `radioButton` ，这由可能的答案值列表组成。|
|isRequired|Boolean|指示是否必须回答自定义问题。|
|question|String|问题。|
|questionId|String|自定义问题的 ID。|
|selectedOptions|String collection|用户选择的答案。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAnswer",
  "questionId": "String",
  "question": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": [
    "String"
  ],
  "isRequired": "Boolean",
  "answer": "String",
  "selectedOptions": [
    "String"
  ]
}
```

