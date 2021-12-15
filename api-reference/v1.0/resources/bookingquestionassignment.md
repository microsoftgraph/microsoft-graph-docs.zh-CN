---
title: bookingQuestionAssignment 资源类型
description: 包含与特定服务关联的一组自定义问题。
ms.localizationpriority: medium
author: razortbone
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: dca8d753b2f2787be2d8dee3fc02b89398608a40
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525024"
---
# <a name="bookingquestionassignment-resource-type"></a>bookingQuestionAssignment 资源类型

命名空间：microsoft.graph

包含与特定服务关联的一组自定义问题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isRequired|Boolean|自定义问题的 ID。|
|questionId|String|指示是否必须回答自定义问题。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAssignment",
  "questionId": "String",
  "isRequired": "Boolean"
}
```

