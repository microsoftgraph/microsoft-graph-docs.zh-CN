---
title: 配置与自定义目标属性同步
description: 您可以自定义您的同步架构，以包括目标目录中定义的自定义属性。 本文介绍如何通过添加名的新字段的自定义的销售队伍订阅`officeCode`。 您设置同步从 Azure Active Directory (Azure AD) 到销售队伍，并为每个用户，您将填充`officeCode`字段中销售队伍的值与`extensionAttribute10`字段中 Azure AD。
localization_priority: Normal
ms.openlocfilehash: 1b0a19bab796f7bd8261ebf898450c07bf1415e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508879"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="ef260-105">配置与自定义目标属性同步</span><span class="sxs-lookup"><span data-stu-id="ef260-105">Configure synchronization with custom target attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef260-106">您可以自定义您的同步架构，以包括目标目录中定义的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="ef260-106">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="ef260-107">本文介绍如何通过添加名的新字段的自定义的销售队伍订阅`officeCode`。</span><span class="sxs-lookup"><span data-stu-id="ef260-107">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="ef260-108">您设置同步从 Azure Active Directory (Azure AD) 到销售队伍，并为每个用户，您将填充`officeCode`字段中销售队伍的值与`extensionAttribute10`字段中 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="ef260-108">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="ef260-109">本文假定您已添加了支持同步到通过[Azure 门户](https://portal.azure.com)，确保您知道应用程序显示名称，租户的应用程序和 Microsoft Graph 具有一个授权令牌。</span><span class="sxs-lookup"><span data-stu-id="ef260-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="ef260-110">有关如何获取授权令牌的信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="ef260-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="ef260-111">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="ef260-111">Find the service principal object by display name</span></span>

<span data-ttu-id="ef260-112">下面的示例演示如何查找与销售队伍的显示名称的服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="ef260-112">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="ef260-113">`{servicePrincipalId}`是`167e33e9-f80e-490e-b4d8-698d4a80fb3e`。</span><span class="sxs-lookup"><span data-stu-id="ef260-113">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="ef260-114">服务主体的上下文中的列表同步作业</span><span class="sxs-lookup"><span data-stu-id="ef260-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="ef260-115">下面的示例演示如何获取`jobId`，您需要使用。</span><span class="sxs-lookup"><span data-stu-id="ef260-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="ef260-116">通常，响应返回只有一个作业。</span><span class="sxs-lookup"><span data-stu-id="ef260-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="ef260-117">`{jobId}`是`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。</span><span class="sxs-lookup"><span data-stu-id="ef260-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="ef260-118">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="ef260-118">Get the synchronization schema</span></span>
<span data-ttu-id="ef260-119">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="ef260-119">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="ef260-120">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ef260-120">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef260-121">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef260-121">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="ef260-122">添加 officeCode 属性和属性之间的映射定义</span><span class="sxs-lookup"><span data-stu-id="ef260-122">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="ef260-123">使用纯文本编辑器 （如[记事本 + +](https://notepad-plus-plus.org/)或[JSON 编辑器联机](https://www.jsoneditoronline.org/)） 您选择的：</span><span class="sxs-lookup"><span data-stu-id="ef260-123">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="ef260-124">添加的[属性定义](synchronization-attributedefinition.md)`officeCode`属性。</span><span class="sxs-lookup"><span data-stu-id="ef260-124">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="ef260-125">在目录中，查找与名称 salesforce.com，和对象的数组中的目录下，找到一个指定的**用户**。</span><span class="sxs-lookup"><span data-stu-id="ef260-125">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="ef260-126">将新属性添加到列表中，指定的名称和类型，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="ef260-126">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="ef260-127">添加[属性映射](synchronization-attributemapping.md)之间`officeCode`和`extensionAttribute10`。</span><span class="sxs-lookup"><span data-stu-id="ef260-127">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="ef260-128">下[synchronizationRules](synchronization-synchronizationrule.md)，查找作为源目录，并为目标目录 Salesforce.com 指定 Azure AD 的规则 (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`)。</span><span class="sxs-lookup"><span data-stu-id="ef260-128">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="ef260-129">在规则[objectMappings](synchronization-objectmapping.md) ，找到用户之间的映射 (`"sourceObjectName": "User",   "targetObjectName": "User"`)。</span><span class="sxs-lookup"><span data-stu-id="ef260-129">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="ef260-130">在**objectMapping** [attributeMappings](synchronization-attributemapping.md)数组中，添加一个新项，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="ef260-130">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="ef260-131">保存修改后的同步架构</span><span class="sxs-lookup"><span data-stu-id="ef260-131">Save the modified synchronization schema</span></span>

<span data-ttu-id="ef260-132">保存更新的同步架构时，请确保您包括整个架构，其中包括未修改的部件。</span><span class="sxs-lookup"><span data-stu-id="ef260-132">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="ef260-133">此请求将使用您提供一个替换现有的架构。</span><span class="sxs-lookup"><span data-stu-id="ef260-133">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="ef260-134">如果架构已成功保存下, 一步迭代的同步作业，则它将启动重新处理您 Azure AD 中的所有帐户和新的映射将应用于所有已设置的帐户。</span><span class="sxs-lookup"><span data-stu-id="ef260-134">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
