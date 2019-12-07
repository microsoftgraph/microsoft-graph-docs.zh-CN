---
title: openShiftChangeRequest 资源类型
description: 表示在计划中声明打开的班次的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 400444ccccc13d103420cc95c522a6ed0aa1afa6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895625"
---
# <a name="openshiftchangerequest-resource-type"></a>openShiftChangeRequest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在[计划](../resources/schedule.md)中对[openshift](../resources/openshift.md)进行声明的班次请求的类型。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 读取**openShiftChangeRequest**对象的属性和关系。 |
| [更新](../api/openshiftchangerequest-update.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 更新**openShiftChangeRequest**对象。 |
| [删除](../api/openshiftchangerequest-delete.md) | None | 删除**openShiftChangeRequest**对象。 |
|[批准](../api/openshiftchangerequest-approve.md)|None|批准打开的班次更改请求。|
|[拒绝](../api/openshiftchangerequest-decline.md)|None| 拒绝打开的班次更改请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|openShiftId|字符串| 打开的班次的 ID。|

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
