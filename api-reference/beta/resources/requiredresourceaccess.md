---
title: requiredResourceAccess 资源类型
description: 指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。 指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。 应用程序实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047521"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。 指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。 [应用程序](application.md)实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。


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
|resourceAccess|[ResourceAccess](resourceaccess.md)集合|OAuth2.0 权限范围和应用程序需要从指定的资源的应用程序角色的列表。|
|resourceAppId|字符串|应用程序需要访问资源的唯一标识符。  这应该是等于**appId**上的目标资源应用程序声明。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
