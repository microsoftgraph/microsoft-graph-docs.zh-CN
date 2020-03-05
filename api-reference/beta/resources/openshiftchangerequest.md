---
title: openShiftChangeRequest 资源类型
description: 表示在计划中声明打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b4ca3b0904ffa0ec5bf06c36e710abdf3ba2a1dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522177"
---
# <a name="openshiftchangerequest-resource-type"></a>openShiftChangeRequest 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在[计划](../resources/schedule.md)中对[openshift](../resources/openshift.md)进行声明的班次请求的类型。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Create](../api/openshiftchangerequest-post.md) | [openshiftchangerequest](openshiftchangerequest.md) | 创建 openshiftchangerequest 对象的实例。 |
| [List](../api/openshiftchangerequest-list.md) | [Openshiftchangerequest](openshiftchangerequest.md)的集合 | 列出团队中的**openShiftChangeRequest**对象的属性和关系。 |
| [获取](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 读取**openShiftChangeRequest**对象的属性和关系。 |
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
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
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
