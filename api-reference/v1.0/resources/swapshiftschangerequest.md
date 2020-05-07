---
title: swapShiftsChangeRequest 资源类型
description: 表示向团队中的其他用户交换班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a3902669028a26abdb8d88e09334ccefe414d42
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154968"
---
# <a name="swapshiftschangerequest-resource-type"></a>swapShiftsChangeRequest 资源类型

命名空间：microsoft.graph

表示将[班次](../resources/shift.md)与[团队](../resources/team.md)中的其他用户交换的班次请求类型。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | [SwapShiftsChangeRequest](swapshiftschangerequest.md)的集合 | 列出团队中的**swapShiftsChangeRequest**对象的属性和关系。 |
| [创建](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | 创建**swapShiftsChangeRequest**对象的实例。 |
| [获取](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | 读取**swapShiftsChangeRequest**对象的属性和关系。 |
|[批准](../api/swapshiftschangerequest-approve.md)|None|批准**swapShiftsChangeRequest**。 |
|[拒绝](../api/swapshiftschangerequest-decline.md)|None|拒绝**swapShiftsChangeRequest**。|

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|recipientShiftId|字符串|ShiftId 要与之交换请求的收件人用户。|

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
