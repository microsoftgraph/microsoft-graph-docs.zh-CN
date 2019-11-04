---
title: requiredResourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围和应用程序角色的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a2104052f4c70a988d1154bb08db025e740246fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938819"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色的集合。 调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 权限范围（通过**requiredResourceAccess**集合）。 [Application](application.md)实体的**RequiredResourceAccess**属性是**ReqiredResourceAccess**的集合。


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
| 属性     | 类型   |描述|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md)集合|应用程序需要指定资源中的 OAuth 2.0 权限范围和应用程序角色的列表。|
|resourceAppId|字符串|应用程序需要访问的资源的唯一标识符。  此值应等于在目标资源应用程序上声明的**appId** 。|

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
