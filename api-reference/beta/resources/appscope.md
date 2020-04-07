---
title: appScope 资源类型
description: '角色分配的范围决定了主体已被授予访问权限的资源集。 应用程序范围是由特定应用程序定义和理解的范围。 另一种类型的作用域是目录作用域。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a996b219df124ac0c287ed4ed32658584acb6ac
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160380"
---
# <a name="appscope-resource-type"></a>appScope 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

角色分配的范围决定了主体已被授予访问权限的资源集。 应用程序范围是由特定应用程序定义和理解的范围。 另一种类型的作用域是目录作用域。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 

这在单个主体、单作用域实体和多个主体中均采用了多个作用域实体。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| id | string | 表示工作分配范围的特定于应用程序的容器或资源的 Id。 通常是资源的不可变 id。 工作分配的范围决定了主体已被授予访问权限的一组资源。 此属性是必需的。 |
| type | String | 描述应用程序范围所表示的应用程序特定资源的类型。 出于显示目的而提供，因此用户界面可以向用户传达应用程序范围所表示的应用程序特定资源的类型。 此属性是只读的。 |
| displayName | string | 提供应用程序范围所表示的应用程序特定资源的显示名称。 出于显示目的而提供，因为 appScopeId 通常是不可变且不可读的可读 id。此属性是只读的。 |

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