---
title: 配置与目录扩展属性的同步
description: '你可以自定义同步架构以包含 Azure Active Directory (Azure AD) 目录扩展属性。 本文介绍如何使用目录扩展属性 (**extension_9d98asdfl15980a_Nickname**) 填充 Salesforce 中的 CommunityNickname 的值。 在这种情况下, 您已将 Azure AD Connect 设置为设置多个目录扩展属性, 从本地 Windows Server Active Directory 到 Azure AD。 '
localization_priority: Normal
ms.openlocfilehash: b16cf5f73c95c34d624de8c1c7a8330b0ce64f4c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277089"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="051dd-105">配置与目录扩展属性的同步</span><span class="sxs-lookup"><span data-stu-id="051dd-105">Configure synchronization with directory extension attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="051dd-106">你可以自定义同步架构以包含 Azure Active Directory (Azure AD) 目录扩展属性。</span><span class="sxs-lookup"><span data-stu-id="051dd-106">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="051dd-107">本文介绍如何使用目录扩展属性 (**extension_9d98asdfl15980a_Nickname**) 填充 Salesforce 中的 CommunityNickname 的值。</span><span class="sxs-lookup"><span data-stu-id="051dd-107">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="051dd-108">在这种情况下, 您已将 Azure AD Connect 设置为设置多个目录扩展属性, 从本地 Windows Server Active Directory 到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="051dd-108">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="051dd-109">本文假定您已添加了一个应用程序, 该应用程序支持通过[Azure 门户](https://portal.azure.com)同步到您的租户, 您知道应用程序显示名称, 并且您具有 Microsoft Graph 的授权令牌。</span><span class="sxs-lookup"><span data-stu-id="051dd-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="051dd-110">有关如何获取授权令牌的信息, 请参阅[获取访问令牌以调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="051dd-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="051dd-111">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="051dd-111">Find the service principal object by display name</span></span>

<span data-ttu-id="051dd-112">下面的示例演示如何查找显示名称为 "Salesforce 沙盒" 的服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="051dd-112">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="051dd-113">`{servicePrincipalId}`为`60443998-8cf7-4e61-b05c-a53b658cb5e1`。</span><span class="sxs-lookup"><span data-stu-id="051dd-113">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="051dd-114">在服务主体的上下文中列出同步作业</span><span class="sxs-lookup"><span data-stu-id="051dd-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="051dd-115">下面的示例演示如何获取需要使用`jobId`的。</span><span class="sxs-lookup"><span data-stu-id="051dd-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="051dd-116">通常情况下, 响应仅返回一个作业。</span><span class="sxs-lookup"><span data-stu-id="051dd-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="051dd-117">`{jobId}`为`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。</span><span class="sxs-lookup"><span data-stu-id="051dd-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="051dd-118">查找所需的目录扩展属性的名称</span><span class="sxs-lookup"><span data-stu-id="051dd-118">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="051dd-119">您需要扩展属性的完整名称。</span><span class="sxs-lookup"><span data-stu-id="051dd-119">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="051dd-120">如果您不知道完整名称 (应类似于**extension_9d98asdfl15980a_Nickname**), 请参阅以下有关目录扩展属性的信息, 以及如何检查它们:</span><span class="sxs-lookup"><span data-stu-id="051dd-120">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="051dd-121">使用自定义属性扩展 Azure AD directory 架构</span><span class="sxs-lookup"><span data-stu-id="051dd-121">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="051dd-122">目录架构扩展 |图形 API 概念</span><span class="sxs-lookup"><span data-stu-id="051dd-122">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="051dd-123">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="051dd-123">Get the synchronization schema</span></span>
<span data-ttu-id="051dd-124">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="051dd-124">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="051dd-125">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="051dd-125">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="051dd-126">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="051dd-126">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="051dd-127">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="051dd-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="051dd-128">C#</span><span class="sxs-lookup"><span data-stu-id="051dd-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="051dd-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="051dd-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="051dd-130">目标-C</span><span class="sxs-lookup"><span data-stu-id="051dd-130">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="051dd-131">为目录扩展属性添加定义以及属性之间的映射</span><span class="sxs-lookup"><span data-stu-id="051dd-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="051dd-132">使用您选择的纯文本编辑器 (例如,[记事本 + +](https://notepad-plus-plus.org/)或[JSON 编辑器 Online](https://www.jsoneditoronline.org/)) 执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="051dd-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="051dd-133">为`extension_9d98asdfl15980a_Nickname`属性添加[属性定义](synchronization-attributedefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="051dd-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="051dd-134">在 "目录" 下, 查找名称为 "Azure Active Directory" 的目录, 并在对象的阵列中查找名为**User**的一个。</span><span class="sxs-lookup"><span data-stu-id="051dd-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="051dd-135">将新属性添加到列表中, 并指定名称和类型, 如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="051dd-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="051dd-136">在 extension_9d98asdfl15980a_Nickname 和 CommunityNickname 之间添加[属性映射](synchronization-attributemapping.md)。</span><span class="sxs-lookup"><span data-stu-id="051dd-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="051dd-137">在 " [synchronizationRules](synchronization-synchronizationrule.md)" 下, 找到指定 Azure AD 作为 "源目录" 的规则, 将 "Salesforce.com`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`" 指定为目标目录 ()。</span><span class="sxs-lookup"><span data-stu-id="051dd-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="051dd-138">在规则的 " [objectMappings](synchronization-objectmapping.md) " 中, 查找 "用户之间的`"sourceObjectName": "User",   "targetObjectName": "User"`映射" ()。</span><span class="sxs-lookup"><span data-stu-id="051dd-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="051dd-139">在**objectMapping**的[attributeMappings](synchronization-attributemapping.md)数组中, 添加一个新项, 如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="051dd-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="051dd-140">保存修改后的同步架构</span><span class="sxs-lookup"><span data-stu-id="051dd-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="051dd-141">保存更新后的同步架构时, 请确保包含整个架构, 包括未修改的部分。</span><span class="sxs-lookup"><span data-stu-id="051dd-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="051dd-142">此请求将使用您提供的架构替换现有架构。</span><span class="sxs-lookup"><span data-stu-id="051dd-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="051dd-143">如果架构已成功保存, 则在同步作业的下一次迭代中, 它将开始重新处理 Azure AD 中的所有帐户, 并且新的映射将应用于所有已设置的帐户。</span><span class="sxs-lookup"><span data-stu-id="051dd-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
