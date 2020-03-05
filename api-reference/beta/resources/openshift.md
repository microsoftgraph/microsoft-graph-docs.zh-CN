---
title: openShift 资源类型
description: 代表计划中未分配的打开班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e544f54c7fbf015ed1050ab23d76217b311bdeaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522191"
---
# <a name="openshift-resource-type"></a>openShift 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[计划](../resources/schedule.md)中未分配的打开班次。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Create](../api/openshift-post.md) | [openShift](openshift.md) | 创建**openShift**对象的实例。 |
| [List](../api/openshift-list.md) | [OpenShift](openshift.md)的集合 | 列出团队中的**openShift**对象的属性和关系。|
| [获取](../api/openshift-get.md) | [openShift](openshift.md) | 读取**openShift**对象的属性和关系。 |
| [更新](../api/openshift-update.md) | [openShift](openshift.md) | 更新**openShift**对象。 |
| [删除](../api/openshift-delete.md) | 无 | 删除**openShift**对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
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
