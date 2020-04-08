---
title: 列出 unifiedRoleDefinitions
description: 获取 unifiedRoleDefinition 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9402d4543cecf51a1c689c6f47ee9f7358fd0800
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181194"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="c7b0d-103">列出 unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c7b0d-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="c7b0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7b0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7b0d-105">获取提供程序的[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7b0d-106">权限</span><span class="sxs-lookup"><span data-stu-id="c7b0d-106">Permissions</span></span>

<span data-ttu-id="c7b0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7b0d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7b0d-109">Permission type</span></span>      | <span data-ttu-id="c7b0d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7b0d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7b0d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b0d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7b0d-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7b0d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7b0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7b0d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-114">Not supported.</span></span>    |
|<span data-ttu-id="c7b0d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7b0d-115">Application</span></span> | <span data-ttu-id="c7b0d-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="c7b0d-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7b0d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7b0d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7b0d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7b0d-118">Optional query parameters</span></span>
<span data-ttu-id="c7b0d-119">此方法支持`$filter` on `id`、 `displayName`、和`isBuiltIn`。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-119">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="c7b0d-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7b0d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7b0d-121">Request headers</span></span>

| <span data-ttu-id="c7b0d-122">名称</span><span class="sxs-lookup"><span data-stu-id="c7b0d-122">Name</span></span>      |<span data-ttu-id="c7b0d-123">说明</span><span class="sxs-lookup"><span data-stu-id="c7b0d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7b0d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7b0d-124">Authorization</span></span> | <span data-ttu-id="c7b0d-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c7b0d-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7b0d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7b0d-126">Request body</span></span>

<span data-ttu-id="c7b0d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7b0d-128">响应</span><span class="sxs-lookup"><span data-stu-id="c7b0d-128">Response</span></span>

<span data-ttu-id="c7b0d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[unifiedRoleDefinition](../resources/unifiedroledefinition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-129">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7b0d-130">示例</span><span class="sxs-lookup"><span data-stu-id="c7b0d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7b0d-131">请求</span><span class="sxs-lookup"><span data-stu-id="c7b0d-131">Request</span></span>

<span data-ttu-id="c7b0d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7b0d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7b0d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="c7b0d-134">C#</span><span class="sxs-lookup"><span data-stu-id="c7b0d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7b0d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7b0d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7b0d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7b0d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7b0d-137">响应</span><span class="sxs-lookup"><span data-stu-id="c7b0d-137">Response</span></span>

<span data-ttu-id="c7b0d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-138">The following is an example of the response.</span></span>

> <span data-ttu-id="c7b0d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7b0d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
