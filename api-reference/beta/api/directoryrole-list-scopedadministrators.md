---
title: 列出目录角色的 scopedMembers
description: 检索目录角色的 scopedRoleMembership 对象列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: da26f04e40a6e64cc634485da6c6056edd15031b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046816"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="a8ae9-103">列出目录角色的 scopedMembers</span><span class="sxs-lookup"><span data-stu-id="a8ae9-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="a8ae9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8ae9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8ae9-105">检索目录角色 [的 scopedRoleMembership](../resources/scopedrolemembership.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8ae9-106">权限</span><span class="sxs-lookup"><span data-stu-id="a8ae9-106">Permissions</span></span>
<span data-ttu-id="a8ae9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8ae9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8ae9-109">Permission type</span></span>      | <span data-ttu-id="a8ae9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8ae9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8ae9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8ae9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8ae9-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8ae9-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8ae9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8ae9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8ae9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-114">Not supported.</span></span>    |
|<span data-ttu-id="a8ae9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8ae9-115">Application</span></span> | <span data-ttu-id="a8ae9-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8ae9-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8ae9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8ae9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a8ae9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a8ae9-118">Optional query parameters</span></span>
<span data-ttu-id="a8ae9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8ae9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8ae9-120">Request headers</span></span>
| <span data-ttu-id="a8ae9-121">名称</span><span class="sxs-lookup"><span data-stu-id="a8ae9-121">Name</span></span>      |<span data-ttu-id="a8ae9-122">说明</span><span class="sxs-lookup"><span data-stu-id="a8ae9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8ae9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8ae9-123">Authorization</span></span>  | <span data-ttu-id="a8ae9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8ae9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8ae9-126">Request body</span></span>
<span data-ttu-id="a8ae9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8ae9-128">响应</span><span class="sxs-lookup"><span data-stu-id="a8ae9-128">Response</span></span>

<span data-ttu-id="a8ae9-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8ae9-130">示例</span><span class="sxs-lookup"><span data-stu-id="a8ae9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8ae9-131">请求</span><span class="sxs-lookup"><span data-stu-id="a8ae9-131">Request</span></span>
<span data-ttu-id="a8ae9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a8ae9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8ae9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="a8ae9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a8ae9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8ae9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8ae9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8ae9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8ae9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8ae9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a8ae9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a8ae9-138">响应</span><span class="sxs-lookup"><span data-stu-id="a8ae9-138">Response</span></span>
<span data-ttu-id="a8ae9-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-139">Here is an example of the response.</span></span> <span data-ttu-id="a8ae9-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a8ae9-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
