---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0fbc0f392a6efa1b0a0ba5f1568451a6fe7d1cf
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219753"
---
# <a name="swapshiftschangerequest-resource-type"></a>swapShiftsChangeRequest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | [SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合 | 列出团队中的**swapShiftsChangeRequest**对象的属性和关系。 |
| [创建](../api/swapshiftschangerequest-post.md) | [swapshiftschangerequest](swapshiftschangerequest.md) | 创建 swapshiftschangerequest 对象的实例。 |
| [获取](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | 读取**swapShiftsChangeRequest**对象的属性和关系。 |
|[批准](../api/swapshiftschangerequest-approve.md)|无|批准**swapShiftsChangeRequest**。 |
|[拒绝](../api/swapshiftschangerequest-decline.md)|无|拒绝**swapShiftsChangeRequest**。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recipientShiftId|String|交换请求的收件人的 ID。 这是请求要交换的用户。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
