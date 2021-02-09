---
title: openShiftChangeRequest 资源类型
description: 表示用于声明计划中打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161416"
---
# <a name="openshiftchangerequest-resource-type"></a>openShiftChangeRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一种班次请求，以声明 [在](../resources/openshift.md) 计划中的开放 [临时](../resources/schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/openshiftchangerequest-post.md) | [openshiftchangerequest](openshiftchangerequest.md) | 创建 openshiftchangerequest 对象的实例。 |
| [列表](../api/openshiftchangerequest-list.md) | [openshiftchangerequest 的集合](openshiftchangerequest.md) | 列出团队 **中 openShiftChangeRequest** 对象的属性和关系。 |
| [Get](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 读取 **openShiftChangeRequest** 对象的属性和关系。 |
|[批准](../api/openshiftchangerequest-approve.md)|无|批准打开的班次更改请求。|
|[拒绝](../api/openshiftchangerequest-decline.md)|无| 拒绝打开的班次更改请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|openShiftId|String| 打开的班次的 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


