---
title: appScope 资源类型
description: 应用范围是特定应用程序定义和理解的范围。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 1cb198e26bae9bf41a63bb834564245c77192863
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110490"
---
# <a name="appscope-resource-type"></a>appScope 资源类型

作用域角色分配确定已授予主体访问权限的资源集。 应用程序作用域是由特定应用程序定义和理解的作用域，这与目录作用域不同，目录范围是存储在目录中的共享范围，并且受多个应用程序理解。

这可能同时在下列主体和范围方案中：
+ 单个主体和单个作用域
+ 多个主体和多个作用域。
    
继承自 [实体](entity.md)。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| displayName | string | 提供显示名称范围表示的特定于应用的资源的源。 提供用于显示目的，因为 appScopeId 通常是不可变的、不可读的 ID。只读。 |
| id | string | 表示分配范围的特定于应用的容器或资源的标识符。 通常是资源的不可变 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 此为必需属性。 |
| type | String | 描述应用程序范围表示的特定于应用的资源的类型。 提供用于显示目的，因此用户界面可以向用户传达应用范围表示的应用特定资源类型。 只读。 |

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
