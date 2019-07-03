---
title: 配置与自定义目标属性的同步
description: 您可以自定义同步架构, 以包括在目标目录中定义的自定义属性。 本文介绍如何通过添加名`officeCode`为的新字段来自定义 Salesforce 订阅。 你将同步从 Azure Active Directory (Azure AD) 设置为 Salesforce, 对于每个用户, 将使用 Azure AD `officeCode`中的`extensionAttribute10`字段的值填充 Salesforce 中的字段。
localization_priority: Normal
ms.openlocfilehash: 772dc8468342c37fa1619758ea681b15f18e7789
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460026"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a>配置与自定义目标属性的同步

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以自定义同步架构, 以包括在目标目录中定义的自定义属性。 本文介绍如何通过添加名`officeCode`为的新字段来自定义 Salesforce 订阅。 你将同步从 Azure Active Directory (Azure AD) 设置为 Salesforce, 对于每个用户, 将使用 Azure AD `officeCode`中的`extensionAttribute10`字段的值填充 Salesforce 中的字段。

本文假定您已添加了一个应用程序, 该应用程序支持通过[Azure 门户](https://portal.azure.com)同步到您的租户, 您知道应用程序显示名称, 并且您具有 Microsoft Graph 的授权令牌。 有关如何获取授权令牌的信息, 请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。

## <a name="find-the-service-principal-object-by-display-name"></a>按显示名称查找服务主体对象

下面的示例演示如何查找显示名称为 Salesforce 的服务主体对象。

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(id,appId,displayName)",
    "value": [
    {
        "id": "167e33e9-f80e-490e-b4d8-698d4a80fb3e",
        "appId": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
        "displayName": "Salesforce"
    },
    {
        "id": "8cbbb70b-7290-42da-83ee-89fa3517a977",
        "appId": "b0f2e3b1-fe31-4658-b216-44dcaeabb63a",
        "displayName": "salesforce 1"
    },
    {
        "id": "60443998-8cf7-4e61-b05c-a53b658cb5e1",
        "appId": "79079396-c301-405d-900f-e2e0c2439a90",
        "displayName": "Salesforce Sandbox"
    }
    ]
}
```

`{servicePrincipalId}`为`167e33e9-f80e-490e-b4d8-698d4a80fb3e`。


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>在服务主体的上下文中列出同步作业 

下面的示例演示如何获取需要使用`jobId`的。 通常情况下, 响应仅返回一个作业。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('60443998-8cf7-4e61-b05c-a53b658cb5e1')/synchronization/jobs",
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {},
            "status": {}
    }
    ]
}
```

`{jobId}`为`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。


## <a name="get-the-synchronization-schema"></a>获取同步架构
下面的示例演示如何获取同步架构。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性将在实际调用中返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "directories": [
        {
              "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
              "name": "Azure Active Directory",
              "objects": [
                {
                    "attributes": [
                        {
                          "anchor": true,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "objectId",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        },
                        {
                          "anchor": false,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "streetAddress",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        }
                    ],
                    "name": "User"
                }
             ]
        },
        {
              "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
              "name": "salesforce.com",
              "objects": []
        }
  ],
 "synchronizationRules": [
        {
          "editable": true,
          "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
          "name": "USER_OUTBOUND_USER",
          "objectMappings": [
                {
                    "attributeMappings": [
                            {
                              "defaultValue": "True",
                              "exportMissingReferences": false,
                              "flowBehavior": "FlowWhenChanged",
                              "flowType": "Always",
                              "matchingPriority": 0,
                              "source": {
                                "expression": "Not([IsSoftDeleted])",
                                "name": "Not",
                                "parameters": [
                                  {
                                    "key": "source",
                                    "value": {
                                      "expression": "[IsSoftDeleted]",
                                      "name": "IsSoftDeleted",
                                      "parameters": [],
                                      "type": "Attribute"
                                    }
                                  }
                                ],
                                "type": "Function"
                              },
                              "targetAttributeName": "IsActive"
                            }
                     ],
                    "enabled": true,
                    "flowTypes": "Add, Update, Delete",
                    "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
            }]
        }]
}
```

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a>为 officeCode 属性添加定义以及属性之间的映射

使用您选择的纯文本编辑器 (例如,[记事本 + +](https://notepad-plus-plus.org/)或[JSON 编辑器 Online](https://www.jsoneditoronline.org/)) 执行以下操作:

1. 为`officeCode`属性添加[属性定义](synchronization-attributedefinition.md)。 

    - 在 "目录" 下, 查找名称为 "salesforce.com" 的目录, 并在对象的数组中查找名为**User**的一个。
    - 将新属性添加到列表中, 并指定名称和类型, 如下面的示例所示。

2. 在和`officeCode` `extensionAttribute10`之间添加[属性映射](synchronization-attributemapping.md)。

    - 在 " [synchronizationRules](synchronization-synchronizationrule.md)" 下, 查找指定 Azure AD 作为源目录的规则, 并将 Salesforce.com 指定为目标`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`目录 ()。
    - 在规则的 " [objectMappings](synchronization-objectmapping.md) " 中, 查找 "用户之间的`"sourceObjectName": "User",   "targetObjectName": "User"`映射" ()。
    - 在**objectMapping**的[attributeMappings](synchronization-attributemapping.md)数组中, 添加一个新项, 如下面的示例所示。

```json
{  
    "directories": [
    {
        "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
            "name": "salesforce.com",
            "objects": [
            {
                "attributes": [
                        {
                            "name": "officeCode",
                            "type": "String"
                        }
                ],
                "name":"User"
            }]
    }
    ],
    "synchronizationRules": [
        {
        "editable": true,
        "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
        "name": "USER_OUTBOUND_USER",
        "objectMappings": [
            {
            "attributeMappings": [
                {
                    "source": {
                            "name": "extensionAttribute10",
                            "type": "Attribute"
                        },
                    "targetAttributeName": "officeCode"
                }
            ],
            "name": "Synchronize Azure Active Directory Users to salesforce.com",
            "scope": null,
            "sourceObjectName": "User",
            "targetObjectName": "User"
            }
        ],
    "priority": 1,
        "sourceDirectoryName": "Azure Active Directory",
        "targetDirectoryName": "salesforce.com"
    }
    ]
}
```

## <a name="save-the-modified-synchronization-schema"></a>保存修改后的同步架构

保存更新后的同步架构时, 请确保包含整个架构, 包括未修改的部分。 此请求将使用您提供的架构替换现有架构。

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

如果架构已成功保存, 则在同步作业的下一次迭代中, 它将开始重新处理 Azure AD 中的所有帐户, 并且新的映射将应用于所有已设置的帐户。
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
