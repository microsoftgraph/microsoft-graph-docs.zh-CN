---
title: openShiftChangeRequest 资源类型
description: 表示请求在日程安排中声明打开的班次。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a6f34e566caa2ff623eb3a66ebf8584b1adeb764dd1e7918bc34f1dbd8455a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229106"
---
# <a name="openshiftchangerequest-resource-type"></a>openShiftChangeRequest 资源类型

命名空间：microsoft.graph

表示在日程安排中 [声明 openShift](../resources/openshift.md) [的请求](../resources/schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/openshiftchangerequest-list.md) | [openShiftChangeRequest 的集合](openshiftchangerequest.md) | 列出团队中 **openShiftChangeRequest** 对象的属性和关系。 |
| [Create](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 创建 **openShiftChangeRequest 对象的实例** 。 |
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

