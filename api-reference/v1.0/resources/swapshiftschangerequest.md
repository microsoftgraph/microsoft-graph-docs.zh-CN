---
title: swapShiftsChangeRequest 资源类型
description: 表示要与团队中的其他用户交换班次的班次请求类型。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 396e4d9dd08044bd726b9e6f85ed808065ec37da
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134449"
---
# <a name="swapshiftschangerequest-resource-type"></a>swapShiftsChangeRequest 资源类型

命名空间：microsoft.graph

表示一种班次请求，用于与 [团队](../resources/shift.md) 中的其他用户交换 [班次](../resources/team.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | [swapShiftsChangeRequest 的集合](swapshiftschangerequest.md) | 列出团队中 **swapShiftsChangeRequest** 对象的属性和关系。 |
| [Create](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | 创建 **swapShiftsChangeRequest 对象** 的实例。 |
| [Get](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | 读取 **swapShiftsChangeRequest** 对象的属性和关系。 |
|[批准](../api/swapshiftschangerequest-approve.md)|无|批准 **swapShiftsChangeRequest**。 |
|[拒绝](../api/swapshiftschangerequest-decline.md)|无|拒绝 **swapShiftsChangeRequest**。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recipientShiftId|String|要与之交换请求的收件人用户的 ShiftId。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
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

