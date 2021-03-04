---
title: 列出 unifiedRoleDefinitions
description: 获取 unifiedRoleDefinition 对象的列表。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b10ed58928ca4b76916f5d24d7211dfd0c839709
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440890"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="8d0ec-103">列出 unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="8d0ec-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="8d0ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d0ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d0ec-105">获取提供程序的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d0ec-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8d0ec-106">Permissions</span></span>

<span data-ttu-id="8d0ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d0ec-109">Permission type</span></span>      | <span data-ttu-id="8d0ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d0ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d0ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d0ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d0ec-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d0ec-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d0ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d0ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d0ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-114">Not supported.</span></span>    |
|<span data-ttu-id="8d0ec-115">Application</span><span class="sxs-lookup"><span data-stu-id="8d0ec-115">Application</span></span> | <span data-ttu-id="8d0ec-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0ec-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d0ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d0ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d0ec-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d0ec-118">Optional query parameters</span></span>
<span data-ttu-id="8d0ec-119">此方法支持 `$filter` 对 `id` 和 `displayName` `isBuiltIn` 。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-119">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="8d0ec-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d0ec-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d0ec-121">Request headers</span></span>

| <span data-ttu-id="8d0ec-122">名称</span><span class="sxs-lookup"><span data-stu-id="8d0ec-122">Name</span></span>      |<span data-ttu-id="8d0ec-123">说明</span><span class="sxs-lookup"><span data-stu-id="8d0ec-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d0ec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0ec-124">Authorization</span></span> | <span data-ttu-id="8d0ec-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8d0ec-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d0ec-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d0ec-126">Request body</span></span>

<span data-ttu-id="8d0ec-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d0ec-128">响应</span><span class="sxs-lookup"><span data-stu-id="8d0ec-128">Response</span></span>

<span data-ttu-id="8d0ec-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-129">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0ec-130">示例</span><span class="sxs-lookup"><span data-stu-id="8d0ec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d0ec-131">请求</span><span class="sxs-lookup"><span data-stu-id="8d0ec-131">Request</span></span>

<span data-ttu-id="8d0ec-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d0ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d0ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="8d0ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="8d0ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d0ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d0ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d0ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d0ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d0ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="8d0ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d0ec-138">响应</span><span class="sxs-lookup"><span data-stu-id="8d0ec-138">Response</span></span>

<span data-ttu-id="8d0ec-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8d0ec-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d0ec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


