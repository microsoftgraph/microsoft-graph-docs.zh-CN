---
title: 配置与目录的扩展属性同步
description: '您可以自定义您的同步架构，以包括 Azure Active Directory (Azure AD) 目录扩展属性。 本文介绍如何使用目录扩展特性 (**extension_9d98asdfl15980a_Nickname**) 来填充 User.CommunityNickname 销售队伍中的值。 在此方案中，您必须将设置为设置数从 Windows Server Active Directory 部署到 Azure AD 目录扩展属性的 Azure AD 连接。 '
localization_priority: Normal
ms.openlocfilehash: 093d78b1e47e412a97ac8a4306c432465e24b5e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850097"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>配置与目录的扩展属性同步

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以自定义您的同步架构，以包括 Azure Active Directory (Azure AD) 目录扩展属性。 本文介绍如何使用目录扩展特性 (**extension_9d98asdfl15980a_Nickname**) 来填充 User.CommunityNickname 销售队伍中的值。 在此方案中，您必须将设置为设置数从 Windows Server Active Directory 部署到 Azure AD 目录扩展属性的 Azure AD 连接。 

本文假定您已添加了支持同步到通过[Azure 门户](https://portal.azure.com)，确保您知道应用程序显示名称，租户的应用程序和 Microsoft Graph 具有一个授权令牌。 有关如何获取授权令牌的信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。

## <a name="find-the-service-principal-object-by-display-name"></a>按显示名称查找服务主体对象

下面的示例演示如何查找具有显示名称"销售队伍沙盒"的服务主体对象。

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}
```

```json
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

`{servicePrincipalId}`是`60443998-8cf7-4e61-b05c-a53b658cb5e1`。

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>服务主体的上下文中的列表同步作业 

下面的示例演示如何获取`jobId`，您需要使用。 通常，响应返回只有一个作业。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}
```

```json
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

`{jobId}`是`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>查找所需的目录扩展属性的名称

您将需要扩展特性的完整名称。 如果您不知道的完整名称 （它应类似于**extension_9d98asdfl15980a_Nickname**），请参阅 directory 扩展属性以及如何对其进行检查的以下信息： 

* [扩展 Azure AD 目录架构包含自定义属性](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [Directory 架构扩展 |图形 API 概念](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>获取同步架构
下面的示例演示如何获取同步架构。

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 将返回实际呼叫中的所有属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>添加目录的扩展特性，和属性之间的映射定义

使用纯文本编辑器 （如[记事本 + +](https://notepad-plus-plus.org/)或[JSON 编辑器联机](https://www.jsoneditoronline.org/)） 您选择的：

1. 添加的[属性定义](synchronization-attributedefinition.md)`extension_9d98asdfl15980a_Nickname`属性。 

    - 在目录下找到名称为"Azure Active Directory"、 目录和对象的数组中找到一个指定的**用户**。
    - 将新属性添加到列表中，指定的名称和类型，如下面的示例中所示。

2. 添加 extension_9d98asdfl15980a_Nickname 之间 CommunityNickname[属性映射](synchronization-attributemapping.md)。

    - 下[synchronizationRules](synchronization-synchronizationrule.md)，查找作为源目录，并为目标目录 Salesforce.com 指定 Azure AD 的规则 (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`)。
    - 在规则[objectMappings](synchronization-objectmapping.md) ，找到用户之间的映射 (`"sourceObjectName": "User",   "targetObjectName": "User"`)。
    - 在**objectMapping** [attributeMappings](synchronization-attributemapping.md)数组中，添加一个新项，如下面的示例中所示。

    ```json
    {
        "directories": [
            {
                "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
                "name": "Azure Active Directory",
                "objects": [
                    {
                        "attributes": [
                                ,{
                                "name": "extension_9d98asdfl15980a_Nickname",
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
            "metadata": [..],
            "name": "USER_OUTBOUND_USER",
            "objectMappings": [
                {
                    "attributeMappings": [
                    ,{
                        "source": {
                            "name": "extension_9d98asdfl15980a_Nickname",
                            "type": "Attribute"
                        },
                        "targetAttributeName": "CommunityNickname"
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
            },
        ]
    }
    ```

## <a name="save-the-modified-synchronization-schema"></a>保存修改后的同步架构

保存更新的同步架构时，请确保您包括整个架构，其中包括未修改的部件。 此请求将使用您提供一个替换现有的架构。

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

如果架构已成功保存下, 一步迭代的同步作业，则它将启动重新处理您 Azure AD 中的所有帐户和新的映射将应用于所有已设置的帐户。
