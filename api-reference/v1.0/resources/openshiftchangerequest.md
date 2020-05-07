---
title: openShiftChangeRequest 资源类型
description: 代表在计划中声明打开的班次的请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 47a2aa9eddc4e45d88c3768ded2b44e9d5952178
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154982"
---
# <a name="openshiftchangerequest-resource-type"></a>openShiftChangeRequest 资源类型

命名空间：microsoft.graph

表示在[计划](../resources/schedule.md)中声明[openShift](../resources/openshift.md)的请求。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/openshiftchangerequest-list.md) | [OpenShiftChangeRequest](openshiftchangerequest.md)的集合 | 列出团队中的**openShiftChangeRequest**对象的属性和关系。 |
| [创建](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 创建**openShiftChangeRequest**对象的实例。 |
| [获取](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | 读取**openShiftChangeRequest**对象的属性和关系。 |
|[批准](../api/openshiftchangerequest-approve.md)|None|批准打开的班次更改请求。|
|[拒绝](../api/openshiftchangerequest-decline.md)|None| 拒绝打开的班次更改请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
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
