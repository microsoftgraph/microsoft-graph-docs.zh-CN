---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 33865876b1750c13c6f2eec77aa09f4fa57191d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957106"
---
# <a name="list-manager"></a><span data-ttu-id="63e31-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="63e31-104">List manager</span></span>

<span data-ttu-id="63e31-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63e31-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63e31-106">返回指定为用户经理的用户或组织联系人。</span><span class="sxs-lookup"><span data-stu-id="63e31-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="63e31-107">（可选）可将经理链一直展开到根节点。</span><span class="sxs-lookup"><span data-stu-id="63e31-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="63e31-108">权限</span><span class="sxs-lookup"><span data-stu-id="63e31-108">Permissions</span></span>

<span data-ttu-id="63e31-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63e31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63e31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63e31-111">Permission type</span></span>      | <span data-ttu-id="63e31-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63e31-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63e31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63e31-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63e31-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63e31-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63e31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63e31-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63e31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e31-116">Not supported.</span></span>    |
|<span data-ttu-id="63e31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63e31-117">Application</span></span> | <span data-ttu-id="63e31-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e31-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="63e31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63e31-119">HTTP request</span></span>

<span data-ttu-id="63e31-120">获取经理：</span><span class="sxs-lookup"><span data-stu-id="63e31-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="63e31-121">获取管理链：</span><span class="sxs-lookup"><span data-stu-id="63e31-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63e31-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63e31-122">Optional query parameters</span></span>

<span data-ttu-id="63e31-123">此方法支持`$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63e31-123">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

><span data-ttu-id="63e31-124">**注意：**</span><span class="sxs-lookup"><span data-stu-id="63e31-124">**Note:**</span></span> 
> + <span data-ttu-id="63e31-125">可以使用 `n` 的值 `$levels` 返回 (`max` 1 到 1000 之间的) 或数字。</span><span class="sxs-lookup"><span data-stu-id="63e31-125">The `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> + <span data-ttu-id="63e31-126">如果未指定 `$levels` 参数，将仅返回直属经理。</span><span class="sxs-lookup"><span data-stu-id="63e31-126">When the `$levels` parameter is not specified, only the immediate manager is returned.</span></span>  
> + <span data-ttu-id="63e31-127">您可以在内部 `$select` 指定 `$expand` 以选择单个经理的属性。</span><span class="sxs-lookup"><span data-stu-id="63e31-127">You can specify `$select` inside `$expand` to select the individual manager's properties.</span></span> <span data-ttu-id="63e31-128">`$levels`参数是必需的：`$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="63e31-128">The `$levels` parameter is required: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="63e31-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="63e31-129">Request headers</span></span>

| <span data-ttu-id="63e31-130">标头</span><span class="sxs-lookup"><span data-stu-id="63e31-130">Header</span></span>       | <span data-ttu-id="63e31-131">值</span><span class="sxs-lookup"><span data-stu-id="63e31-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="63e31-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e31-132">Authorization</span></span>  | <span data-ttu-id="63e31-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63e31-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63e31-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="63e31-135">ConsistencyLevel</span></span> | <span data-ttu-id="63e31-136">最终。</span><span class="sxs-lookup"><span data-stu-id="63e31-136">eventual.</span></span> <span data-ttu-id="63e31-137">请求包括 `$expand=manager($levels=max)` 参数时必需。</span><span class="sxs-lookup"><span data-stu-id="63e31-137">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63e31-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="63e31-138">Request body</span></span>

<span data-ttu-id="63e31-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63e31-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63e31-140">响应</span><span class="sxs-lookup"><span data-stu-id="63e31-140">Response</span></span>

<span data-ttu-id="63e31-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63e31-141">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63e31-142">示例</span><span class="sxs-lookup"><span data-stu-id="63e31-142">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="63e31-143">示例 1：获取经理</span><span class="sxs-lookup"><span data-stu-id="63e31-143">Example 1: Get manager</span></span>

<span data-ttu-id="63e31-144">以下示例显示获取经理的请求。</span><span class="sxs-lookup"><span data-stu-id="63e31-144">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="63e31-145">请求</span><span class="sxs-lookup"><span data-stu-id="63e31-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="63e31-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="63e31-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="63e31-147">C#</span><span class="sxs-lookup"><span data-stu-id="63e31-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63e31-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63e31-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63e31-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63e31-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63e31-150">Java</span><span class="sxs-lookup"><span data-stu-id="63e31-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63e31-151">响应</span><span class="sxs-lookup"><span data-stu-id="63e31-151">Response</span></span>

<span data-ttu-id="63e31-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63e31-152">The following is an example of the response.</span></span>
><span data-ttu-id="63e31-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63e31-153">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "<user-id>",
  "displayName": "Sara Davis",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="63e31-154">示例 2：获取直至根级别的经理链</span><span class="sxs-lookup"><span data-stu-id="63e31-154">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="63e31-155">以下示例显示获取直至根级别的经理链的请求。</span><span class="sxs-lookup"><span data-stu-id="63e31-155">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="63e31-156">请求</span><span class="sxs-lookup"><span data-stu-id="63e31-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="63e31-157">响应</span><span class="sxs-lookup"><span data-stu-id="63e31-157">Response</span></span>

<span data-ttu-id="63e31-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63e31-158">The following is an example of the response.</span></span> <span data-ttu-id="63e31-159">可传递的经理分层显示。</span><span class="sxs-lookup"><span data-stu-id="63e31-159">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="63e31-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63e31-160">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "<user1-id>",
    "displayName": "Individual Contributor",
    "manager": {
        "id": "<manager1-id>",
        "displayName": "Manager 1",
        "manager": {
            "id": "<manager2-id>",
            "displayName": "Manager 2",
            "manager": {
                "id": "<manager3-id>",
                "displayName": "Manager 3"
            }
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
