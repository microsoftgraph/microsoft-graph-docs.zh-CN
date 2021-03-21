---
title: 配置与目录扩展属性的同步
description: 自定义同步架构，以将 Azure Active Directory (Azure AD) 扩展属性。
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: db5e2ba4bc715f608d17b8e11067df71141a6142
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956974"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="3d7de-103">配置与目录扩展属性的同步</span><span class="sxs-lookup"><span data-stu-id="3d7de-103">Configure synchronization with directory extension attributes</span></span>

<span data-ttu-id="3d7de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d7de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d7de-105">你可以自定义同步架构，以将 Azure Active Directory (Azure AD) 扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3d7de-105">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="3d7de-106">本文介绍如何使用目录扩展属性 (extension_9d98asdfl15980a_Nickname) Salesforce 中User.CommunityNickname 的值。</span><span class="sxs-lookup"><span data-stu-id="3d7de-106">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="3d7de-107">在此方案中，你已设置 Azure AD Connect 以预配从本地 Windows Server Active Directory 到 Azure AD 的一些目录扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3d7de-107">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="3d7de-108">本文假定你已添加支持通过 [Azure](https://portal.azure.com)门户与租户同步的应用程序，你知道应用程序显示名称，并且你具有 Microsoft Graph 的授权令牌。</span><span class="sxs-lookup"><span data-stu-id="3d7de-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="3d7de-109">若要了解如何获取授权令牌，请参阅[获取访问令牌以调用 Microsoft Graph。](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="3d7de-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="3d7de-110">按以下方法查找服务主体显示名称</span><span class="sxs-lookup"><span data-stu-id="3d7de-110">Find the service principal object by display name</span></span>

<span data-ttu-id="3d7de-111">以下示例演示如何查找具有"Salesforce 沙盒"显示名称服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="3d7de-111">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="3d7de-112">`{servicePrincipalId}`为 `60443998-8cf7-4e61-b05c-a53b658cb5e1` 。</span><span class="sxs-lookup"><span data-stu-id="3d7de-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="3d7de-113">在服务主体上下文中列出同步作业</span><span class="sxs-lookup"><span data-stu-id="3d7de-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="3d7de-114">以下示例演示如何获取 `jobId` 您需要的 。</span><span class="sxs-lookup"><span data-stu-id="3d7de-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="3d7de-115">通常，响应仅返回一个作业。</span><span class="sxs-lookup"><span data-stu-id="3d7de-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="3d7de-116">`{jobId}`为 `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` 。</span><span class="sxs-lookup"><span data-stu-id="3d7de-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="3d7de-117">查找所需的目录扩展属性的名称</span><span class="sxs-lookup"><span data-stu-id="3d7de-117">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="3d7de-118">你将需要扩展属性的完整名称。</span><span class="sxs-lookup"><span data-stu-id="3d7de-118">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="3d7de-119">如果不知道完整名称 (其外观应类似于 extension_9d98asdfl15980a_Nickname **) ，** 请参阅以下有关目录扩展属性以及如何检查它们的信息：</span><span class="sxs-lookup"><span data-stu-id="3d7de-119">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="3d7de-120">使用自定义属性扩展 Azure AD 目录架构</span><span class="sxs-lookup"><span data-stu-id="3d7de-120">Extending the Azure AD directory schema with custom properties</span></span>](/graph/extensibility-overview)
* [<span data-ttu-id="3d7de-121">目录架构扩展|Graph API 概念</span><span class="sxs-lookup"><span data-stu-id="3d7de-121">Directory schema extensions | Graph API concepts</span></span>](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="3d7de-122">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="3d7de-122">Get the synchronization schema</span></span>
<span data-ttu-id="3d7de-123">以下示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="3d7de-123">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d7de-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d7de-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="3d7de-125">C#</span><span class="sxs-lookup"><span data-stu-id="3d7de-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d7de-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d7de-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d7de-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d7de-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d7de-128">Java</span><span class="sxs-lookup"><span data-stu-id="3d7de-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="3d7de-129">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3d7de-129">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d7de-130">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d7de-130">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="3d7de-131">为目录扩展属性添加定义，以及属性之间的映射</span><span class="sxs-lookup"><span data-stu-id="3d7de-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="3d7de-132">使用你选择的纯文本编辑器 (例如，记事本 [++](https://notepad-plus-plus.org/) 或 [JSON 编辑器 Online](https://www.jsoneditoronline.org/)) ：</span><span class="sxs-lookup"><span data-stu-id="3d7de-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="3d7de-133">为 [属性添加属性](synchronization-attributedefinition.md) `extension_9d98asdfl15980a_Nickname` 定义。</span><span class="sxs-lookup"><span data-stu-id="3d7de-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="3d7de-134">在目录下，查找名为"Azure Active Directory"的目录，在对象的数组中查找名为 **User 的目录**。</span><span class="sxs-lookup"><span data-stu-id="3d7de-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="3d7de-135">将新属性添加到列表中，并指定名称和类型，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="3d7de-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="3d7de-136">在 [Extension_9d98asdfl15980a_Nickname](synchronization-attributemapping.md) 和 CommunityNickname 之间添加属性映射。</span><span class="sxs-lookup"><span data-stu-id="3d7de-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="3d7de-137">在 [synchronizationRules](synchronization-synchronizationrule.md)下，查找将 Azure AD 指定为源目录的规则，Salesforce.com 指定为目标 `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` () 。</span><span class="sxs-lookup"><span data-stu-id="3d7de-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="3d7de-138">在 [规则的 objectMappings](synchronization-objectmapping.md) 中，查找用户与 `"sourceObjectName": "User",   "targetObjectName": "User"` () 。</span><span class="sxs-lookup"><span data-stu-id="3d7de-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="3d7de-139">在 **objectMapping** 的 [attributeMappings](synchronization-attributemapping.md)数组中，添加新条目，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="3d7de-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="3d7de-140">保存修改后的同步架构</span><span class="sxs-lookup"><span data-stu-id="3d7de-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="3d7de-141">保存更新的同步架构时，请确保包括整个架构，包括未修改的部分。</span><span class="sxs-lookup"><span data-stu-id="3d7de-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="3d7de-142">此请求将用您提供的架构替换现有架构。</span><span class="sxs-lookup"><span data-stu-id="3d7de-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="3d7de-143">如果架构已成功保存，则下次迭代同步作业时，它将开始重新处理 Azure AD 中所有帐户，并且新映射将应用于所有预配的帐户。</span><span class="sxs-lookup"><span data-stu-id="3d7de-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
