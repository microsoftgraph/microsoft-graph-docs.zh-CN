---
title: appScope 资源类型
description: 应用范围是由特定应用程序定义和理解的范围。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: de49425bddc5905d1b1bf17afeb5fb7c5363038c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136008"
---
# <a name="appscope-resource-type"></a>appScope 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作用域角色分配确定主体已被授予访问权限的资源集。 应用范围是由特定应用程序定义和理解的范围。 另一种类型的作用域是目录范围。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 

这同时在单个主体、单个范围实体和多个主体、多个范围实体中采用。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| id | string | 表示分配范围的特定于应用的容器或资源的 ID。 通常是资源的不可变 ID。 工作分配的范围决定了主体已被授予访问权限的资源集。 此属性是必需的。 |
| type | 字符串 | 描述应用范围所代表的特定于应用的资源的类型。 提供用于显示目的，以便用户界面可以向用户传达应用范围表示的应用特定资源类型。 此属性为只读。 |
| displayName | string | 提供显示名称范围表示的特定于应用的资源的源。 提供用于显示目的，因为 appScopeId 通常是不可变的不可读 ID。此属性为只读。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope"
}-->

```json
{
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

