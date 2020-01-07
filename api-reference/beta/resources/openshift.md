---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f3ce94c12328e9c05f899c5d2176339bbed93432
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951935"
---
# <a name="openshift-resource-type"></a>openShift 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[计划](../resources/schedule.md)中未分配的打开班次。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Create](../api/openshift-post.md) | [openShift](openshift.md) | 创建**openShift**对象的实例。 |
| [List](../api/openshift-list.md) | [OpenShift](openshift.md)的集合 | 列出团队中的**openShift**对象的属性和关系。|
| [Get](../api/openshift-get.md) | [openShift](openshift.md) | 读取**openShift**对象的属性和关系。 |
| [更新](../api/openshift-update.md) | [openShift](openshift.md) | 更新**openShift**对象。 |
| [删除](../api/openshift-delete.md) | 无 | 删除**openShift**对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|未发布的打开班次。|
|schedulingGroupId|String|打开的班次所属的计划组的 ID。|
|sharedOpenShift|[openShiftItem](openshiftitem.md)|已发布的打开班次。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
