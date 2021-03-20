---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1b51b94b03f18647e8d3cf88036ecee22ab4de3a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943352"
---
# <a name="list-manager"></a><span data-ttu-id="f7964-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="f7964-104">List manager</span></span>

<span data-ttu-id="f7964-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7964-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7964-106">返回指定为用户经理的用户或组织联系人。</span><span class="sxs-lookup"><span data-stu-id="f7964-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="f7964-107">（可选）可将经理链一直展开到根节点。</span><span class="sxs-lookup"><span data-stu-id="f7964-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7964-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7964-108">Permissions</span></span>

<span data-ttu-id="f7964-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7964-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7964-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7964-111">Permission type</span></span>      | <span data-ttu-id="f7964-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7964-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7964-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7964-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7964-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7964-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7964-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7964-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7964-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7964-116">Not supported.</span></span>    |
|<span data-ttu-id="f7964-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7964-117">Application</span></span> | <span data-ttu-id="f7964-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7964-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f7964-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7964-119">HTTP request</span></span>

<span data-ttu-id="f7964-120">获取经理：</span><span class="sxs-lookup"><span data-stu-id="f7964-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="f7964-121">获取管理链：</span><span class="sxs-lookup"><span data-stu-id="f7964-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=n)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=n)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7964-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7964-122">Optional query parameters</span></span>

<span data-ttu-id="f7964-123">此方法支持`$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7964-123">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

><span data-ttu-id="f7964-124">**注意：**</span><span class="sxs-lookup"><span data-stu-id="f7964-124">**Note:**</span></span> 
> + <span data-ttu-id="f7964-125">值 `n` 为 `$levels` （以 `max` 返回所有经理）或 1 到 1000 之间的数字。</span><span class="sxs-lookup"><span data-stu-id="f7964-125">The `n` value of `$levels` can be `max` (to return all managers) or a number between 1 and 1000.</span></span>  
> + <span data-ttu-id="f7964-126">如果未指定 `$levels` 参数，将仅返回直属经理。</span><span class="sxs-lookup"><span data-stu-id="f7964-126">When the `$levels` parameter is not specified, only the immediate manager is returned.</span></span>  
> + <span data-ttu-id="f7964-127">您可以指定 `$select` 内部 `$expand` 单个经理的属性。</span><span class="sxs-lookup"><span data-stu-id="f7964-127">You can specify `$select` inside `$expand` to select the individual manager's properties.</span></span> <span data-ttu-id="f7964-128">参数 `$levels` 必需： `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="f7964-128">The `$levels` parameter is required: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7964-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7964-129">Request headers</span></span>

| <span data-ttu-id="f7964-130">标头</span><span class="sxs-lookup"><span data-stu-id="f7964-130">Header</span></span>       | <span data-ttu-id="f7964-131">值</span><span class="sxs-lookup"><span data-stu-id="f7964-131">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f7964-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7964-132">Authorization</span></span>  | <span data-ttu-id="f7964-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7964-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7964-135">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f7964-135">ConsistencyLevel</span></span> | <span data-ttu-id="f7964-136">最终。</span><span class="sxs-lookup"><span data-stu-id="f7964-136">eventual.</span></span> <span data-ttu-id="f7964-137">请求包括 `$expand=manager($levels=max)` 参数时必需。</span><span class="sxs-lookup"><span data-stu-id="f7964-137">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7964-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7964-138">Request body</span></span>

<span data-ttu-id="f7964-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7964-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7964-140">响应</span><span class="sxs-lookup"><span data-stu-id="f7964-140">Response</span></span>

<span data-ttu-id="f7964-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7964-141">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7964-142">示例</span><span class="sxs-lookup"><span data-stu-id="f7964-142">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="f7964-143">示例 1：获取经理</span><span class="sxs-lookup"><span data-stu-id="f7964-143">Example 1: Get manager</span></span>

<span data-ttu-id="f7964-144">以下示例显示获取经理的请求。</span><span class="sxs-lookup"><span data-stu-id="f7964-144">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="f7964-145">请求</span><span class="sxs-lookup"><span data-stu-id="f7964-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f7964-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7964-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="f7964-147">C#</span><span class="sxs-lookup"><span data-stu-id="f7964-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7964-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7964-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7964-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7964-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7964-150">Java</span><span class="sxs-lookup"><span data-stu-id="f7964-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f7964-151">响应</span><span class="sxs-lookup"><span data-stu-id="f7964-151">Response</span></span>

<span data-ttu-id="f7964-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7964-152">The following is an example of the response.</span></span>
><span data-ttu-id="f7964-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7964-153">**Note**: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="f7964-154">示例 2：获取直至根级别的经理链</span><span class="sxs-lookup"><span data-stu-id="f7964-154">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="f7964-155">以下示例显示获取直至根级别的经理链的请求。</span><span class="sxs-lookup"><span data-stu-id="f7964-155">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="f7964-156">请求</span><span class="sxs-lookup"><span data-stu-id="f7964-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f7964-157">响应</span><span class="sxs-lookup"><span data-stu-id="f7964-157">Response</span></span>

<span data-ttu-id="f7964-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7964-158">The following is an example of the response.</span></span> <span data-ttu-id="f7964-159">可传递的经理分层显示。</span><span class="sxs-lookup"><span data-stu-id="f7964-159">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="f7964-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7964-160">**Note**: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
