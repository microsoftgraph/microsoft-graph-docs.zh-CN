---
title: " (预览版) 分配、更新或删除自定义安全属性"
description: 了解如何使用 Microsoft 图形 API 为用户和应用程序分配、更新或删除自定义安全属性 (服务主体) 。
author: rolyon
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: directory-management
ms.openlocfilehash: 21db29dc53c3b005dd0fa09c5e13bd7cfa055a1f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442125"
---
# <a name="assign-update-or-remove-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>使用 Microsoft 图形 API (预览) 分配、更新或删除自定义安全属性

> [!IMPORTANT]
> 自定义安全属性功能目前为预览版。 有关适用于 Beta、预览版或尚未发布到正式版的 Azure 功能的法律条款，请参阅 [Microsoft Azure 预览版补充使用条款](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) 。

Azure Active Directory (Azure AD) 中的[自定义安全属性](/azure/active-directory/fundamentals/custom-security-attributes-overview)是特定于企业的属性， (键值对) 可以定义和分配给 Azure AD 对象。

本文提供有关如何为用户和应用程序分配、更新或删除不同类型的自定义安全属性的示例， (服务主体) 。 只能通过`PATCH`[更新用户](/graph/api/user-update)或 [Update servicePrincipal](/graph/api/serviceprincipal-update) 请求中的操作来分配或更新自定义安全属性。

## <a name="permissions"></a>权限

若要管理自定义安全属性，必须为调用主体分配以下 Azure AD 角色。 默认情况下，全局管理员和其他管理员角色无权读取、定义或分配自定义安全属性。

- [属性分配管理员](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

此外，必须向调用主体授予以下权限。

- [CustomSecAttributeAssignment.ReadWrite.All](permissions-reference.md#custom-security-attributes-permissions)
- [User.Read.All](permissions-reference.md#user-permissions)

*自定义SecAttributeAssignment.ReadWrite.All* 授予对应用程序的读取、分配、更新或删除属性的权限。 使用资源对象权限（例如 *User.Read.All*）单独授予读取资源对象的权限（例如用户）。

## <a name="assign-custom-security-attributes"></a>分配自定义安全属性

### <a name="example-1-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>示例 1：为用户分配具有字符串值的自定义安全属性

以下示例演示如何向用户分配具有字符串值的自定义安全属性。

- 属性集：`Engineering`
- 属性：`ProjectDate`
- 属性数据类型：字符串
- 属性值：`"2022-10-01"`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-assign-a-custom-security-attribute-with-a-string-value-to-a-service-principal"></a>示例 2：将具有字符串值的自定义安全属性分配给服务主体

下面的示例演示如何将具有字符串值的自定义安全属性分配给服务主体。

- 属性集： `Engineering`
- 属性：`ProjectDate`
- 属性数据类型：字符串
- 属性值：`"2022-10-01"`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_serviceprincipal_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-3-assign-a-custom-security-attribute-with-a-multi-string-value-to-a-user"></a>示例 3：为用户分配具有多字符串值的自定义安全属性

以下示例演示如何向用户分配具有多字符串值的自定义安全属性。

- 属性集：`Engineering`
- 属性：`Project`
- 属性数据类型：字符串集合
- 属性值：`["Baker","Cascade"]`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multistring"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project@odata.type":"#Collection(String)",
            "Project":["Baker","Cascade"]
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-4-assign-a-custom-security-attribute-with-an-integer-value-to-a-user"></a>示例 4：为用户分配具有整数值的自定义安全属性

以下示例演示如何为用户分配具有整数值的自定义安全属性。

- 属性集：`Engineering`
- 属性：`NumVendors`
- 属性数据类型：整数
- 属性值：`4`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":4
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-5-assign-a-custom-security-attribute-with-a-multi-integer-value-to-a-user"></a>示例 5：为用户分配具有多整数值的自定义安全属性

以下示例演示如何为用户分配具有多整数值的自定义安全属性。

- 属性集：`Engineering`
- 属性：`CostCenter`
- 属性数据类型：整数集合
- 属性值：`[1001,1003]`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multiinteger"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "CostCenter@odata.type":"#Collection(Int32)",
            "CostCenter":[1001,1003]
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-6-assign-a-custom-security-attribute-with-a-boolean-value-to-a-user"></a>示例 6：为用户分配具有布尔值的自定义安全属性

以下示例演示如何为用户分配具有布尔值的自定义安全属性。

- 属性集：`Engineering`
- 属性：`Certification`
- 属性数据类型：布尔
- 属性值：`true`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":true
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="update-custom-security-attribute-assignments"></a>更新自定义安全属性分配

### <a name="example-1-update-a-custom-security-attribute-assignment-with-an-integer-value-for-a-user"></a>示例 1：使用用户的整数值更新自定义安全属性分配

以下示例演示如何使用用户的整数值更新自定义安全属性分配。

- 属性集：`Engineering`
- 属性：`NumVendors`
- 属性数据类型：整数
- 属性值：`8`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":8
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-update-a-custom-security-attribute-assignment-with-a-boolean-value-for-a-user"></a>示例 2：使用用户的布尔值更新自定义安全属性分配

以下示例演示如何使用用户的布尔值更新自定义安全属性分配。

- 属性集：`Engineering`
- 属性：`Certification`
- 属性数据类型：布尔
- 属性值：`false`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":false
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remove-custom-security-attribute-assignments"></a>删除自定义安全属性分配

### <a name="example-1-remove-a-single-valued-custom-security-attribute-assignment-from-a-user"></a>示例 1：从用户中删除单值自定义安全属性分配

以下示例演示如何从用户中删除支持单个值的自定义安全属性分配。

- 属性集：`Engineering`
- 属性：`ProjectDate`
- 属性值：`null`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_singlevalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":null
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-multi-valued-custom-security-attribute-assignment-from-a-user"></a>示例 2：从用户中删除多值自定义安全属性分配

以下示例演示如何从用户中删除支持多个值的自定义安全属性分配。

- 属性集：`Engineering`
- 属性：`Project`
- 属性值：`[]`

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_multivalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project":[]
        }
    }
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 图形 API (预览版) 的自定义安全属性概述](/graph/api/resources/custom-security-attributes-overview)
- [Azure AD 中的自定义安全属性是什么？](/azure/active-directory/fundamentals/custom-security-attributes-overview)
