---
title: 列出 scopedAdministratorOf
description: 检索用户的 scopedRoleMembership 列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0686e0a6b8ac6bec26a2f30d8e52e59b52f3a192
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051702"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="cfb2b-103">列出 scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="cfb2b-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="cfb2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfb2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfb2b-105">检索用户的 [scopedRoleMembership](../resources/scopedrolemembership.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfb2b-106">权限</span><span class="sxs-lookup"><span data-stu-id="cfb2b-106">Permissions</span></span>
<span data-ttu-id="cfb2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cfb2b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfb2b-109">Permission type</span></span>      | <span data-ttu-id="cfb2b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfb2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfb2b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfb2b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfb2b-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfb2b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfb2b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfb2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb2b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-114">Not supported.</span></span>    |
|<span data-ttu-id="cfb2b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfb2b-115">Application</span></span> | <span data-ttu-id="cfb2b-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfb2b-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfb2b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfb2b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedRoleMemberOf 
GET /users/{id}/scopedRoleMemberOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="cfb2b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cfb2b-118">Optional query parameters</span></span>
<span data-ttu-id="cfb2b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfb2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfb2b-120">Request headers</span></span>
| <span data-ttu-id="cfb2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="cfb2b-121">Header</span></span>       | <span data-ttu-id="cfb2b-122">值</span><span class="sxs-lookup"><span data-stu-id="cfb2b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfb2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfb2b-123">Authorization</span></span>  | <span data-ttu-id="cfb2b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfb2b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfb2b-126">Request body</span></span>
<span data-ttu-id="cfb2b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfb2b-128">响应</span><span class="sxs-lookup"><span data-stu-id="cfb2b-128">Response</span></span>

<span data-ttu-id="cfb2b-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cfb2b-130">示例</span><span class="sxs-lookup"><span data-stu-id="cfb2b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfb2b-131">请求</span><span class="sxs-lookup"><span data-stu-id="cfb2b-131">Request</span></span>
<span data-ttu-id="cfb2b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfb2b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb2b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf
```
# <a name="c"></a>[<span data-ttu-id="cfb2b-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfb2b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfb2b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfb2b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfb2b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfb2b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfb2b-137">Java</span><span class="sxs-lookup"><span data-stu-id="cfb2b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedadministratorof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cfb2b-138">响应</span><span class="sxs-lookup"><span data-stu-id="cfb2b-138">Response</span></span>
<span data-ttu-id="cfb2b-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-139">Here is an example of the response.</span></span> <span data-ttu-id="cfb2b-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cfb2b-140">Note: The response object shown here might be shortened for readability.</span></span>
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
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
