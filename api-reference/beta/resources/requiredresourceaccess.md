---
title: requiredResourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围和应用程序角色的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 3c2251f5a5b4655a73747490f5052661c3b4a6eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521108"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess 资源类型

命名空间： microsoft. graph

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
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md)集合|应用程序需要指定资源中的 OAuth 2.0 权限范围和应用程序角色的列表。|
|resourceAppId|String|应用程序需要访问的资源的唯一标识符。  此值应等于在目标资源应用程序上声明的**appId** 。|

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
