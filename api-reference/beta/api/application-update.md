---
title: 更新应用程序
description: 更新 application 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2794bdb2c9f86db7565a3d1b9cfcd1411e358e4e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318668"
---
# <a name="update-application"></a>更新应用程序

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 application 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All |

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

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| 指定应用程序是否可以充当公共客户端。 例如, 在移动设备上运行的已安装应用程序。 默认值为 *false*。 |
|api|[apiApplication](../resources/apiapplication.md)| 指定 API 应用程序的设置。 |
|appRoles|[appRole](../resources/approle.md) 集合|应用程序可声明的应用程序角色的集合。 这些角色可以分配给用户、组或服务主体。 不可为 null。|
|重|String 集合| 用于标识应用程序的 URI。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)。 多值属性筛选器表达式需要 *any* 运算符。 不可为 Null。 |
|createdDateTime|DateTimeOffset| 注册应用程序的日期和时间。 |
|deletedDateTime|DateTimeOffset| 删除应用程序的日期和时间。 |
|displayName|String|应用程序的显示名称。 |
|id|String|应用程序的唯一标识符。 继承自 [directoryObject](../resources/directoryobject.md)。 键。 不可为 null。 只读。 |
|info|[informationalUrl](../resources/informationalurl.md)| 应用程序的基本配置文件信息。 | 指定已安装客户端（如台式设备或移动设备）的设置。 |
|keyCredentials|[keyCredential](../resources/keycredential.md) 集合|与应用程序关联的密钥凭据集合，不可为 Null。 |
|logo|Stream|应用程序的主徽标。 不可为 null。 |
|orgRestrictions|String 集合| 应用程序受限制的组织 tenantIds。  如果集合为空, 则应用程序为多租户 (不受限制)。 如果集合包含 tenantIds, 则将应用程序限制为集合中的组织 tenantIds。 如果指定其他租户, 而不是在其中注册应用程序的 tenantId, 则意味着应用程序自身的 tenantId 将被间接包括在内。 |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) 集合|与应用程序关联的密码凭据集合。 不可为 Null。|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md)集合| 列出了应用程序和请求的隐式同意权限。 要求管理员向应用程序提供许可。 preAuthorizedApplications 不要求用户同意请求的权限。 PreAuthorizedApplications 中列出的权限不需要用户同意。 但是, preAuthorizedApplications 中未列出的任何其他请求的权限都需要用户同意。 |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) 集合|指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。 这种预配置的所需资源访问权限可驱动同意体验。 不可为 Null。|
|标记|String collection| 可用于分类和标识应用程序的自定义字符串。 |
|web|[webApplication](../resources/webapplication.md)| 指定 Web 应用程序的设置。 |

## <a name="response"></a>响应

如果成功, 此方法将`204 No Content`返回响应代码, 并且不会在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
注意：为简洁起见，可能会截断此处显示的响应对象。 
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
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
