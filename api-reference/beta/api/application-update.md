---
title: 更新应用程序
description: 更新应用程序对象的属性。
ms.openlocfilehash: eaf3eaaab7e14407c6c778e4e38711b2842ed46c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041451"
---
# <a name="update-application"></a>更新应用程序

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新应用程序对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowPublicClient|布尔值| 指定应用程序可用作公共客户端。 例如，移动设备上运行安装的应用程序。 默认值为 *false*。 |
|api|[api](../resources/api.md)| 指定 API 应用程序的设置。 |
|appRoles|[appRole](../resources/approle.md)集合|声明应用程序可能的应用程序角色的集合。 这些角色可以分配给用户、 组或服务主体。 不可为 null。|
|applicationAliases|String 集合| 标识应用程序的 Uri。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。 *Any*运算符，则需要为多值属性的筛选器表达式。 不可为 null。 |
|createdDateTime|DateTimeOffset| 日期和时间注册应用程序。 |
|deletedDateTime|DateTimeOffset| 日期和时间的应用程序已删除。 |
|displayName|字符串|应用程序的显示名称。 |
|id|字符串|应用程序的唯一标识符。 继承自 [directoryObject](../resources/directoryobject.md)。 键。 不可为 null。 只读。 |
|信息|[informationalUrl](../resources/informationalurl.md)| 应用程序的基本配置文件信息。 | 指定安装客户端，如桌面或移动设备的设置。 |
|keyCredentials|[keyCredential](../resources/keycredential.md)集合|不应用程序关联的关键凭据集合可以为 null。 |
|logo|Stream|主应用程序徽标。 不可为 null。 |
|orgRestrictions|String 集合| 应用程序所使用的受限组织 tenantIds。  如果集合为空，该应用程序是多租户 （不受限制）。 如果集合包含 tenantIds，应用程序仅限于组织 tenantIds 集合中。 指定其他租户但未注册应用程序其中 tenantId 意味着应用程序自身的 tenantId 为间接包含。 |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md)集合|应用程序关联的密码凭据的集合。 不可为 null。|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md)集合| 列出应用程序和隐式同意请求的权限。 需要管理员可以提供了到应用程序的许可。 preAuthorizedApplications 不需要用户同意所请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是，preAuthorizedApplications 中未列出任何其他请求的权限要求用户同意。 |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md)集合|指定此应用程序需要访问和一组的 OAuth 权限范围和应用程序角色它需要在每个这些资源的资源。 此预配置完所需的资源访问驱动器的同意体验。 不可为 null。|
|标记前添加的标记|String 集合| 用于分类和确定应用程序的自定义字符串。 |
|web|[web](../resources/web.md)| 指定 web 应用程序的设置。 |

## <a name="response"></a>响应

如果成功，此方法返回`204 No Content`响应代码和不响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a>响应
注意：为简洁起见，可能会截断此处展示的响应对象。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->