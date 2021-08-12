---
title: requiredResourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围的应用程序角色集。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 24d4e48fb6a15fabb61552d1ee2f2d884f276e6a862706b290fb97c1a2a78096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184492"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess 资源类型

命名空间：microsoft.graph

指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色集。 指定的 OAuth 2.0 权限范围可能由客户端应用程序 (调用资源应用程序时) **requiredResourceAccess** 集合请求。 **application 实体的 requiredResourceAccess** 属性是 **Re一redResourceAccess 的集合**。 [](application.md)


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resourceAccess|[resourceAccess](resourceaccess.md) 集合|应用程序从指定资源请求的 OAuth2.0 权限范围和应用角色列表。|
|resourceAppId|String|应用程序需要访问的资源的唯一标识符。  这应该等于在目标资源应用程序上声明的 **appId。**|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

