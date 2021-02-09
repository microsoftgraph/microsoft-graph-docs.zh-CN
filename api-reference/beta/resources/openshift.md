---
title: openShift 资源类型
description: 表示计划中的未分配开放班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a272d985a4aa71e1c1fdfc83baed51379010d7dc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159463"
---
# <a name="openshift-resource-type"></a>openShift 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示计划的未分配、打开的 [班次](../resources/schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/openshift-post.md) | [openShift](openshift.md) | 创建 **openShift 对象** 的实例。 |
| [列表](../api/openshift-list.md) | [openShift 集合](openshift.md) | 列出团队 **中 openShift** 对象的属性和关系。|
| [Get](../api/openshift-get.md) | [openShift](openshift.md) | 读取 **openShift 对象的属性和** 关系。 |
| [更新](../api/openshift-update.md) | [openShift](openshift.md) | 更新 **openShift** 对象。 |
| [删除](../api/openshift-delete.md) | 无 | 删除 **openShift** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|未发布的开放班次。|
|schedulingGroupId|String|开放班次所属的计划组的 ID。|
|sharedOpenShift|[openShiftItem](openshiftitem.md)|已发布的打开班次。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift"
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


