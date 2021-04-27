---
title: 列出 privilegedRoles
description: 检索 privilegedRole 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e785505a3b6a86b82a1631422e0e8861e68551d0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055258"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="e5626-103">列出 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="e5626-103">List privilegedRoles</span></span>

<span data-ttu-id="e5626-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5626-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5626-105">检索 [privilegedRole 对象](../resources/privilegedrole.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="e5626-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="e5626-106">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="e5626-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5626-107">权限</span><span class="sxs-lookup"><span data-stu-id="e5626-107">Permissions</span></span>
<span data-ttu-id="e5626-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e5626-110">请求程序需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="e5626-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="e5626-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5626-111">Permission type</span></span>      | <span data-ttu-id="e5626-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5626-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5626-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5626-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e5626-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5626-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5626-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5626-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5626-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5626-116">Not supported.</span></span>    |
|<span data-ttu-id="e5626-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5626-117">Application</span></span> | <span data-ttu-id="e5626-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5626-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5626-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5626-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5626-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5626-120">Optional query parameters</span></span>
<span data-ttu-id="e5626-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5626-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5626-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5626-122">Request headers</span></span>
| <span data-ttu-id="e5626-123">名称</span><span class="sxs-lookup"><span data-stu-id="e5626-123">Name</span></span>      |<span data-ttu-id="e5626-124">说明</span><span class="sxs-lookup"><span data-stu-id="e5626-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5626-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5626-125">Authorization</span></span>  | <span data-ttu-id="e5626-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5626-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5626-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5626-128">Request body</span></span>
<span data-ttu-id="e5626-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5626-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5626-130">响应</span><span class="sxs-lookup"><span data-stu-id="e5626-130">Response</span></span>

<span data-ttu-id="e5626-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [privilegedRole](../resources/privilegedrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5626-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="e5626-132">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="e5626-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e5626-133">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="e5626-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e5626-134">示例</span><span class="sxs-lookup"><span data-stu-id="e5626-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5626-135">请求</span><span class="sxs-lookup"><span data-stu-id="e5626-135">Request</span></span>
<span data-ttu-id="e5626-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5626-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5626-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5626-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="e5626-138">C#</span><span class="sxs-lookup"><span data-stu-id="e5626-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5626-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5626-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5626-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5626-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5626-141">Java</span><span class="sxs-lookup"><span data-stu-id="e5626-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5626-142">响应</span><span class="sxs-lookup"><span data-stu-id="e5626-142">Response</span></span>
<span data-ttu-id="e5626-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5626-143">Here is an example of the response.</span></span> <span data-ttu-id="e5626-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5626-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
