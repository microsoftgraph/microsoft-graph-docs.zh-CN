---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3eff83475c4a36ec1c294c62b9e1b87673926d8d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895626"
---
# <a name="openshift-resource-type"></a>openShift 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[计划](../resources/schedule.md)中未分配的打开班次。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/openshift-get.md) | [openShift](openshift.md) | 读取 openShift 对象的属性和关系。 |
| [更新](../api/openshift-update.md) | [openShift](openshift.md) | 更新 openShift 对象。 |
| [删除](../api/openshift-delete.md) | None | 删除 openShift 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|未发布的打开班次。|
|schedulingGroupId|字符串|打开的班次所属的计划组的 ID。|
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
