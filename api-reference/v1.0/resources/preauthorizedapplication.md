---
title: preAuthorizedApplication 资源类型
description: 列出预先授权的客户端应用程序
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 25632d22161a5fb422cb67786f26fdc7c645bd4f
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118422"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

命名空间：microsoft.graph

列出具有访问此应用程序 API 的指定权限预先授权的客户端应用程序。 用户不需要同意任何预先授权的应用程序 (指定) 权限。 但是，在 preAuthorizedApplications 中未列出的任何其他权限 (通过增量许可请求，例如) 将需要用户同意。

在某些极少数情况下，属性中`delegatedPermissionIds`列出的标识符实际上可能标识服务主体`appRoles`属性)  (的[应用角色](approle.md)，指示该`appId`属性标识的客户端应用程序已预先授权该应用角色。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|delegatedPermissionIds|字符串集合| 应用程序所需的 [oauth2PermissionScopes](permissionscope.md) 的唯一标识符。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "delegatedPermissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

