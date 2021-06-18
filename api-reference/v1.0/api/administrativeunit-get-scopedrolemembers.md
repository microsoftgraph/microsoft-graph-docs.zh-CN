---
title: 获取 scopedRoleMember
description: 检索特定的 scopedRoleMembership 资源。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c6e0e3de92ee350a17b1821e7c567dbaa1792f9d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991533"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="1e6df-103">获取 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="1e6df-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="1e6df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e6df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e6df-105">检索特定的 [scopedRoleMembership](../resources/scopedrolemembership.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="1e6df-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e6df-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e6df-106">Permissions</span></span>
<span data-ttu-id="1e6df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e6df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e6df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e6df-109">Permission type</span></span>      | <span data-ttu-id="1e6df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e6df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e6df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e6df-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e6df-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e6df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e6df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e6df-114">Not supported.</span></span>    |
|<span data-ttu-id="1e6df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e6df-115">Application</span></span> | <span data-ttu-id="1e6df-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e6df-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e6df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e6df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e6df-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e6df-118">Optional query parameters</span></span>
<span data-ttu-id="1e6df-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e6df-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e6df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e6df-120">Request headers</span></span>
| <span data-ttu-id="1e6df-121">名称</span><span class="sxs-lookup"><span data-stu-id="1e6df-121">Name</span></span>      |<span data-ttu-id="1e6df-122">说明</span><span class="sxs-lookup"><span data-stu-id="1e6df-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e6df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e6df-123">Authorization</span></span>  | <span data-ttu-id="1e6df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e6df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e6df-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e6df-126">Request body</span></span>
<span data-ttu-id="1e6df-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e6df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e6df-128">响应</span><span class="sxs-lookup"><span data-stu-id="1e6df-128">Response</span></span>

<span data-ttu-id="1e6df-129">如果成功，此方法在响应正文中返回 响应代码和请求 `200 OK` [的 scopedRoleMembership](../resources/scopedrolemembership.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e6df-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e6df-130">示例</span><span class="sxs-lookup"><span data-stu-id="1e6df-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e6df-131">请求</span><span class="sxs-lookup"><span data-stu-id="1e6df-131">Request</span></span>
<span data-ttu-id="1e6df-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e6df-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1e6df-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e6df-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="1e6df-134">C#</span><span class="sxs-lookup"><span data-stu-id="1e6df-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e6df-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e6df-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e6df-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e6df-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e6df-137">Java</span><span class="sxs-lookup"><span data-stu-id="1e6df-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="1e6df-138">响应</span><span class="sxs-lookup"><span data-stu-id="1e6df-138">Response</span></span>
<span data-ttu-id="1e6df-p103">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e6df-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
