---
title: '使用 Microsoft Graph API (预览版分配、更新) '
description: 了解如何使用 Microsoft Graph API 为用户和应用程序分配、更新 (服务主体) 自定义安全属性。
author: rolyon
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: directory-management
ms.openlocfilehash: 74603d7d39203134151928243de98624fc7a0dad
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077662"
---
# <a name="assign-update-or-remove-custom-security-attributes-using-the-microsoft-graph-api-preview"></a>使用 Microsoft Graph API (预览版分配、更新) 

> [!IMPORTANT]
> 自定义安全属性功能当前处于预览阶段。 有关适用于 Beta 版、预览[版](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)或尚未正式发布的 Azure 功能的法律条款，请参阅 Microsoft Azure 预览版补充使用条款。

[Azure Active Directory (Azure AD) 中的](/azure/active-directory/fundamentals/custom-security-attributes-overview)自定义安全属性是特定于业务 (属性，) 定义和分配给 Azure AD 对象。

本文提供了如何为用户和应用程序分配、更新或删除不同类型的自定义安全属性的示例， (服务主体) 。 自定义安全属性只能通过 Update 用户或 Update `PATCH` [servicePrincipal](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)请求中的操作分配或更新。 [](/graph/api/user-update?view=graph-rest-beta&preserve-view=true)

## <a name="permissions"></a>权限

若要管理自定义安全属性，必须为调用主体分配以下Azure AD角色。 默认情况下，全局管理员和其他管理员角色没有读取、定义或分配自定义安全属性的权限。

- [属性分配管理员](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

此外，还必须向调用主体授予以下权限。

- [CustomSecAttributeAssignment.ReadWrite.All](permissions-reference.md#custom-security-attributes-permissions)

## <a name="assign-custom-security-attributes"></a>分配自定义安全属性

### <a name="example-1-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>示例 1：向用户分配具有字符串值的自定义安全属性

以下示例演示如何向用户分配具有字符串值的自定义安全属性。

- 属性集： `Engineering`
- 属性： `ProjectDate`
- 属性数据类型：String
- 属性值： `"2022-10-01"`

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

以下示例演示如何将具有字符串值的自定义安全属性分配给服务主体。

- 属性集： `Engineering`
- 属性： `ProjectDate`
- 属性数据类型：String
- 属性值： `"2022-10-01"`

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

### <a name="example-3-assign-a-custom-security-attribute-with-a-multi-string-value-to-a-user"></a>示例 3：向用户分配具有多字符串值的自定义安全属性

以下示例演示如何向用户分配具有多字符串值的自定义安全属性。

- 属性集： `Engineering`
- 属性： `Project`
- 属性数据类型：字符串集合
- 属性值： `["Baker","Cascade"]`

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

### <a name="example-4-assign-a-custom-security-attribute-with-an-integer-value-to-a-user"></a>示例 4：向用户分配具有整数值的自定义安全属性

以下示例演示如何向用户分配具有整数值的自定义安全属性。

- 属性集： `Engineering`
- 属性： `NumVendors`
- 属性数据类型：Integer
- 属性值： `4`

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

### <a name="example-5-assign-a-custom-security-attribute-with-a-multi-integer-value-to-a-user"></a>示例 5：向用户分配具有多整数值的自定义安全属性

以下示例演示如何向用户分配具有多整数值的自定义安全属性。

- 属性集： `Engineering`
- 属性： `CostCenter`
- 属性数据类型：Integers 集合
- 属性值： `[1001,1003]`

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

### <a name="example-6-assign-a-custom-security-attribute-with-a-boolean-value-to-a-user"></a>示例 6：向用户分配具有布尔值的自定义安全属性

以下示例演示如何向用户分配具有布尔值的自定义安全属性。

- 属性集： `Engineering`
- 属性： `Certification`
- 属性数据类型：Boolean
- 属性值： `true`

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

### <a name="example-1-update-a-custom-security-attribute-assignment-with-an-integer-value-for-a-user"></a>示例 1：使用用户整数值更新自定义安全属性分配

以下示例演示如何使用用户整数值更新自定义安全属性分配。

- 属性集： `Engineering`
- 属性： `NumVendors`
- 属性数据类型：Integer
- 属性值： `8`

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

- 属性集： `Engineering`
- 属性： `Certification`
- 属性数据类型：Boolean
- 属性值： `false`

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

以下示例演示如何删除支持用户单个值的自定义安全属性分配。

- 属性集： `Engineering`
- 属性： `ProjectDate`
- 属性值： `null`

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

以下示例演示如何删除支持来自用户的多个值的自定义安全属性分配。

- 属性集： `Engineering`
- 属性： `Project`
- 属性值： `[]`

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

- [使用 Microsoft Graph API 的自定义安全属性概述](/graph/api/resources/custom-security-attributes-overview)
- [什么是自定义安全Azure AD？](/azure/active-directory/fundamentals/custom-security-attributes-overview)
- [Update user](/graph/api/user-update?view=graph-rest-beta&preserve-view=true)
- [更新 servicePrincipal](/graph/api/serviceprincipal-update?view=graph-rest-beta&preserve-view=true)
