---
title: 使用自定义目标属性配置同步
description: 自定义同步架构以包括目标目录中定义的自定义属性。
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 865cde06cded24f9f2920e63535e037a2b477330
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956890"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="53bb7-103">使用自定义目标属性配置同步</span><span class="sxs-lookup"><span data-stu-id="53bb7-103">Configure synchronization with custom target attributes</span></span>

<span data-ttu-id="53bb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53bb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53bb7-105">您可以自定义同步架构以包括目标目录中定义的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="53bb7-105">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="53bb7-106">本文介绍如何通过添加名为 的新字段来自定义 Salesforce 订阅 `officeCode` 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-106">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="53bb7-107">设置从 Azure Active Directory (Azure AD) 到 Salesforce 的同步，并且对于每个用户，你将使用 Azure AD 中的字段中的值填充 `officeCode` Salesforce 中的 `extensionAttribute10` 字段。</span><span class="sxs-lookup"><span data-stu-id="53bb7-107">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="53bb7-108">本文假定你已添加支持通过 [Azure](https://portal.azure.com)门户与租户同步的应用程序，你知道应用程序显示名称，并且你具有 Microsoft Graph 的授权令牌。</span><span class="sxs-lookup"><span data-stu-id="53bb7-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="53bb7-109">若要了解如何获取授权令牌，请参阅[获取访问令牌以调用 Microsoft Graph。](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="53bb7-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="53bb7-110">按以下方法查找服务主体显示名称</span><span class="sxs-lookup"><span data-stu-id="53bb7-110">Find the service principal object by display name</span></span>

<span data-ttu-id="53bb7-111">以下示例演示如何查找 Salesforce 显示名称对象。</span><span class="sxs-lookup"><span data-stu-id="53bb7-111">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="53bb7-112">`{servicePrincipalId}`为 `167e33e9-f80e-490e-b4d8-698d4a80fb3e` 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-112">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="53bb7-113">在服务主体上下文中列出同步作业</span><span class="sxs-lookup"><span data-stu-id="53bb7-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="53bb7-114">以下示例演示如何获取 `jobId` 您需要的 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="53bb7-115">通常，响应仅返回一个作业。</span><span class="sxs-lookup"><span data-stu-id="53bb7-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="53bb7-116">`{jobId}`为 `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="53bb7-117">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="53bb7-117">Get the synchronization schema</span></span>
<span data-ttu-id="53bb7-118">以下示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="53bb7-118">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="53bb7-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="53bb7-119">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="53bb7-120">C#</span><span class="sxs-lookup"><span data-stu-id="53bb7-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53bb7-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53bb7-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53bb7-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53bb7-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53bb7-123">Java</span><span class="sxs-lookup"><span data-stu-id="53bb7-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="53bb7-124">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53bb7-124">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="53bb7-125">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53bb7-125">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="53bb7-126">添加 officeCode 属性的定义和属性之间的映射</span><span class="sxs-lookup"><span data-stu-id="53bb7-126">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="53bb7-127">使用你选择的纯文本编辑器 (例如，记事本 [++](https://notepad-plus-plus.org/) 或 [JSON 编辑器 Online](https://www.jsoneditoronline.org/)) ：</span><span class="sxs-lookup"><span data-stu-id="53bb7-127">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="53bb7-128">为 [属性添加属性](synchronization-attributedefinition.md) `officeCode` 定义。</span><span class="sxs-lookup"><span data-stu-id="53bb7-128">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="53bb7-129">在目录下，查找名称为 salesforce.com 的目录，在对象的数组中查找名为 **User 的目录**。</span><span class="sxs-lookup"><span data-stu-id="53bb7-129">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="53bb7-130">将新属性添加到列表中，并指定名称和类型，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="53bb7-130">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="53bb7-131">在 和 [之间添加](synchronization-attributemapping.md) 属性 `officeCode` 映射 `extensionAttribute10` 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-131">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="53bb7-132">在 [synchronizationRules](synchronization-synchronizationrule.md)下，查找将 Azure AD 指定为源目录的规则，Salesforce.com 指定为目标 `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` () 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-132">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="53bb7-133">在 [规则的 objectMappings](synchronization-objectmapping.md) 中，查找用户与 `"sourceObjectName": "User",   "targetObjectName": "User"` () 。</span><span class="sxs-lookup"><span data-stu-id="53bb7-133">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="53bb7-134">在 **objectMapping** 的 [attributeMappings](synchronization-attributemapping.md)数组中，添加新条目，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="53bb7-134">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="53bb7-135">保存修改后的同步架构</span><span class="sxs-lookup"><span data-stu-id="53bb7-135">Save the modified synchronization schema</span></span>

<span data-ttu-id="53bb7-136">保存更新的同步架构时，请确保包括整个架构，包括未修改的部分。</span><span class="sxs-lookup"><span data-stu-id="53bb7-136">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="53bb7-137">此请求将用您提供的架构替换现有架构。</span><span class="sxs-lookup"><span data-stu-id="53bb7-137">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="53bb7-138">如果架构已成功保存，则下次迭代同步作业时，它将开始重新处理 Azure AD 中所有帐户，并且新映射将应用于所有预配的帐户。</span><span class="sxs-lookup"><span data-stu-id="53bb7-138">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
