---
title: 配置与目录的扩展属性同步
description: '您可以自定义您的同步架构，以包括 Azure Active Directory (Azure AD) 目录扩展属性。 本文介绍如何使用目录扩展特性 (**extension_9d98asdfl15980a_Nickname**) 来填充 User.CommunityNickname 销售队伍中的值。 在此方案中，您必须将设置为设置数从 Windows Server Active Directory 部署到 Azure AD 目录扩展属性的 Azure AD 连接。 '
ms.openlocfilehash: fa29e405b235107cd6773444085e7b409441c90e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048118"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="69382-105">配置与目录的扩展属性同步</span><span class="sxs-lookup"><span data-stu-id="69382-105">Configure synchronization with directory extension attributes</span></span>

> <span data-ttu-id="69382-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69382-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69382-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69382-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69382-108">您可以自定义您的同步架构，以包括 Azure Active Directory (Azure AD) 目录扩展属性。</span><span class="sxs-lookup"><span data-stu-id="69382-108">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="69382-109">本文介绍如何使用目录扩展特性 (**extension_9d98asdfl15980a_Nickname**) 来填充 User.CommunityNickname 销售队伍中的值。</span><span class="sxs-lookup"><span data-stu-id="69382-109">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="69382-110">在此方案中，您必须将设置为设置数从 Windows Server Active Directory 部署到 Azure AD 目录扩展属性的 Azure AD 连接。</span><span class="sxs-lookup"><span data-stu-id="69382-110">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="69382-111">本文假定您已添加了支持同步到通过[Azure 门户](https://portal.azure.com)，确保您知道应用程序显示名称，租户的应用程序和 Microsoft Graph 具有一个授权令牌。</span><span class="sxs-lookup"><span data-stu-id="69382-111">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="69382-112">有关如何获取授权令牌的信息，请参阅[获取访问令牌调用 Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview)。</span><span class="sxs-lookup"><span data-stu-id="69382-112">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="69382-113">按显示名称查找服务主体对象</span><span class="sxs-lookup"><span data-stu-id="69382-113">Find the service principal object by display name</span></span>

<span data-ttu-id="69382-114">下面的示例演示如何查找具有显示名称"销售队伍沙盒"的服务主体对象。</span><span class="sxs-lookup"><span data-stu-id="69382-114">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="69382-115">`{servicePrincipalId}`是`60443998-8cf7-4e61-b05c-a53b658cb5e1`。</span><span class="sxs-lookup"><span data-stu-id="69382-115">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="69382-116">服务主体的上下文中的列表同步作业</span><span class="sxs-lookup"><span data-stu-id="69382-116">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="69382-117">下面的示例演示如何获取`jobId`，您需要使用。</span><span class="sxs-lookup"><span data-stu-id="69382-117">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="69382-118">通常，响应返回只有一个作业。</span><span class="sxs-lookup"><span data-stu-id="69382-118">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="69382-119">`{jobId}`是`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。</span><span class="sxs-lookup"><span data-stu-id="69382-119">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="69382-120">查找所需的目录扩展属性的名称</span><span class="sxs-lookup"><span data-stu-id="69382-120">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="69382-121">您将需要扩展特性的完整名称。</span><span class="sxs-lookup"><span data-stu-id="69382-121">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="69382-122">如果您不知道的完整名称 （它应类似于**extension_9d98asdfl15980a_Nickname**），请参阅 directory 扩展属性以及如何对其进行检查的以下信息：</span><span class="sxs-lookup"><span data-stu-id="69382-122">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="69382-123">扩展 Azure AD 目录架构包含自定义属性</span><span class="sxs-lookup"><span data-stu-id="69382-123">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="69382-124">Directory 架构扩展 |图形 API 概念</span><span class="sxs-lookup"><span data-stu-id="69382-124">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="69382-125">获取同步架构</span><span class="sxs-lookup"><span data-stu-id="69382-125">Get the synchronization schema</span></span>
<span data-ttu-id="69382-126">下面的示例演示如何获取同步架构。</span><span class="sxs-lookup"><span data-stu-id="69382-126">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="69382-127">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="69382-127">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69382-128">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="69382-128">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="69382-129">添加目录的扩展特性，和属性之间的映射定义</span><span class="sxs-lookup"><span data-stu-id="69382-129">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="69382-130">使用纯文本编辑器 （如[记事本 + +](https://notepad-plus-plus.org/)或[JSON 编辑器联机](https://www.jsoneditoronline.org/)） 您选择的：</span><span class="sxs-lookup"><span data-stu-id="69382-130">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="69382-131">添加的[属性定义](synchronization-attributedefinition.md)`extension_9d98asdfl15980a_Nickname`属性。</span><span class="sxs-lookup"><span data-stu-id="69382-131">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="69382-132">在目录下找到名称为"Azure Active Directory"、 目录和对象的数组中找到一个指定的**用户**。</span><span class="sxs-lookup"><span data-stu-id="69382-132">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="69382-133">将新属性添加到列表中，指定的名称和类型，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="69382-133">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="69382-134">添加 extension_9d98asdfl15980a_Nickname 之间 CommunityNickname[属性映射](synchronization-attributemapping.md)。</span><span class="sxs-lookup"><span data-stu-id="69382-134">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="69382-135">下[synchronizationRules](synchronization-synchronizationrule.md)，查找作为源目录，并为目标目录 Salesforce.com 指定 Azure AD 的规则 (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`)。</span><span class="sxs-lookup"><span data-stu-id="69382-135">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="69382-136">在规则[objectMappings](synchronization-objectmapping.md) ，找到用户之间的映射 (`"sourceObjectName": "User",   "targetObjectName": "User"`)。</span><span class="sxs-lookup"><span data-stu-id="69382-136">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="69382-137">在**objectMapping** [attributeMappings](synchronization-attributemapping.md)数组中，添加一个新项，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="69382-137">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="69382-138">保存修改后的同步架构</span><span class="sxs-lookup"><span data-stu-id="69382-138">Save the modified synchronization schema</span></span>

<span data-ttu-id="69382-139">保存更新的同步架构时，请确保您包括整个架构，其中包括未修改的部件。</span><span class="sxs-lookup"><span data-stu-id="69382-139">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="69382-140">此请求将使用您提供一个替换现有的架构。</span><span class="sxs-lookup"><span data-stu-id="69382-140">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="69382-141">如果架构已成功保存下, 一步迭代的同步作业，则它将启动重新处理您 Azure AD 中的所有帐户和新的映射将应用于所有已设置的帐户。</span><span class="sxs-lookup"><span data-stu-id="69382-141">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>