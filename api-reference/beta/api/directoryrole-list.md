---
title: 列出 directoryRoles
description: 列出租户中激活的目录角色。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b34011e1ed208405f40e4a5a5be6af20e1f217fe
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334421"
---
# <a name="list-directoryroles"></a><span data-ttu-id="1709c-103">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="1709c-103">List directoryRoles</span></span>

<span data-ttu-id="1709c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1709c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1709c-105">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="1709c-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="1709c-106">此操作仅返回已激活的角色。</span><span class="sxs-lookup"><span data-stu-id="1709c-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="1709c-107">当管理员使用 [Activate directoryRole](directoryrole-post-directoryroles.md) API 激活角色时，角色将变为激活状态。</span><span class="sxs-lookup"><span data-stu-id="1709c-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="1709c-108">并非所有内置角色最初都是激活的。</span><span class="sxs-lookup"><span data-stu-id="1709c-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="1709c-109">使用 Azure 门户分配角色时，角色激活步骤将代表管理员隐式完成。</span><span class="sxs-lookup"><span data-stu-id="1709c-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="1709c-110">若要获取 Azure AD 中提供的角色的完整列表，请使用 [List directoryRoleTemplates](directoryroletemplate-list.md)。</span><span class="sxs-lookup"><span data-stu-id="1709c-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1709c-111">权限</span><span class="sxs-lookup"><span data-stu-id="1709c-111">Permissions</span></span>
<span data-ttu-id="1709c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1709c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1709c-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="1709c-114">Permission type</span></span>      | <span data-ttu-id="1709c-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1709c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1709c-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1709c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1709c-117">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1709c-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1709c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1709c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1709c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1709c-119">Not supported.</span></span>    |
|<span data-ttu-id="1709c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="1709c-120">Application</span></span> | <span data-ttu-id="1709c-121">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1709c-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1709c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1709c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1709c-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1709c-123">Optional query parameters</span></span>
<span data-ttu-id="1709c-124">此方法 **不** 支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="1709c-124">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1709c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1709c-125">Request headers</span></span>
| <span data-ttu-id="1709c-126">名称</span><span class="sxs-lookup"><span data-stu-id="1709c-126">Name</span></span>       | <span data-ttu-id="1709c-127">类型</span><span class="sxs-lookup"><span data-stu-id="1709c-127">Type</span></span> | <span data-ttu-id="1709c-128">说明</span><span class="sxs-lookup"><span data-stu-id="1709c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1709c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1709c-129">Authorization</span></span>  | <span data-ttu-id="1709c-130">string</span><span class="sxs-lookup"><span data-stu-id="1709c-130">string</span></span>  | <span data-ttu-id="1709c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1709c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1709c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="1709c-133">Request body</span></span>
<span data-ttu-id="1709c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1709c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1709c-135">响应</span><span class="sxs-lookup"><span data-stu-id="1709c-135">Response</span></span>

<span data-ttu-id="1709c-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1709c-136">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1709c-137">示例</span><span class="sxs-lookup"><span data-stu-id="1709c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1709c-138">请求</span><span class="sxs-lookup"><span data-stu-id="1709c-138">Request</span></span>
<span data-ttu-id="1709c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1709c-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1709c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1709c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="1709c-141">C#</span><span class="sxs-lookup"><span data-stu-id="1709c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1709c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1709c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1709c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1709c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1709c-144">Java</span><span class="sxs-lookup"><span data-stu-id="1709c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1709c-145">响应</span><span class="sxs-lookup"><span data-stu-id="1709c-145">Response</span></span>
<span data-ttu-id="1709c-p105">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1709c-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "value": [
    {
      "id": "9ed3a0c4-53e1-498c-ab4d-2473476fde14",
      "deletedDateTime": null,
      "description": "Can manage all aspects of Azure AD and Microsoft services that use Azure AD identities.",
      "displayName": "Global Administrator",
      "roleTemplateId": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "deletedDateTime": null,
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8"
    },
    {
      "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
      "deletedDateTime": null,
      "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
      "displayName": "Directory Readers",
      "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
