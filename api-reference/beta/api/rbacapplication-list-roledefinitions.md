---
title: 列出 unifiedRoleDefinitions
description: 获取 unifiedRoleDefinition 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c858cb438d3e2706d611fef0b4d9b1cc38a2955
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723194"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="20e61-103">列出 unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="20e61-103">List unifiedRoleDefinitions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e61-104">获取提供程序的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="20e61-104">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="20e61-105">权限</span><span class="sxs-lookup"><span data-stu-id="20e61-105">Permissions</span></span>

<span data-ttu-id="20e61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e61-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="20e61-108">Permission type</span></span>      | <span data-ttu-id="20e61-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20e61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e61-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20e61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="20e61-111">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="20e61-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20e61-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20e61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e61-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="20e61-113">Not supported.</span></span>    |
|<span data-ttu-id="20e61-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="20e61-114">Application</span></span> | <span data-ttu-id="20e61-115">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="20e61-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e61-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20e61-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20e61-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20e61-117">Optional query parameters</span></span>
<span data-ttu-id="20e61-118">此方法支持`$filter` on `id`、 `displayName`、和`isBuiltIn`。</span><span class="sxs-lookup"><span data-stu-id="20e61-118">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="20e61-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20e61-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20e61-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20e61-120">Request headers</span></span>

| <span data-ttu-id="20e61-121">名称</span><span class="sxs-lookup"><span data-stu-id="20e61-121">Name</span></span>      |<span data-ttu-id="20e61-122">说明</span><span class="sxs-lookup"><span data-stu-id="20e61-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20e61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20e61-123">Authorization</span></span> | <span data-ttu-id="20e61-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="20e61-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e61-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="20e61-125">Request body</span></span>

<span data-ttu-id="20e61-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20e61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20e61-127">响应</span><span class="sxs-lookup"><span data-stu-id="20e61-127">Response</span></span>

<span data-ttu-id="20e61-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="20e61-128">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20e61-129">示例</span><span class="sxs-lookup"><span data-stu-id="20e61-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="20e61-130">请求</span><span class="sxs-lookup"><span data-stu-id="20e61-130">Request</span></span>

<span data-ttu-id="20e61-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20e61-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20e61-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="20e61-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20e61-133">C#</span><span class="sxs-lookup"><span data-stu-id="20e61-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20e61-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e61-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20e61-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="20e61-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20e61-136">响应</span><span class="sxs-lookup"><span data-stu-id="20e61-136">Response</span></span>

<span data-ttu-id="20e61-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="20e61-137">The following is an example of the response.</span></span>

> <span data-ttu-id="20e61-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20e61-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "resourceScopes": [
                "/"
            ],
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
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
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
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
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
