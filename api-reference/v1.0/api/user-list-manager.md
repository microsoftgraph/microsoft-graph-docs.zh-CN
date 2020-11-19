---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Priority
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d9df52fa26407cd5b08a3b8cb69ac156bc996925
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086779"
---
# <a name="list-manager"></a><span data-ttu-id="c0486-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="c0486-104">List manager</span></span>

<span data-ttu-id="c0486-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0486-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0486-106">返回指定为用户经理的用户或组织联系人。</span><span class="sxs-lookup"><span data-stu-id="c0486-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="c0486-107">（可选）可将经理链一直展开到根节点。</span><span class="sxs-lookup"><span data-stu-id="c0486-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0486-108">权限</span><span class="sxs-lookup"><span data-stu-id="c0486-108">Permissions</span></span>

<span data-ttu-id="c0486-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0486-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0486-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0486-111">Permission type</span></span>      | <span data-ttu-id="c0486-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0486-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0486-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0486-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0486-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0486-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0486-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0486-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0486-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0486-116">Not supported.</span></span>    |
|<span data-ttu-id="c0486-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0486-117">Application</span></span> | <span data-ttu-id="c0486-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0486-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c0486-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0486-119">HTTP request</span></span>

<span data-ttu-id="c0486-120">获取经理：</span><span class="sxs-lookup"><span data-stu-id="c0486-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="c0486-121">获取管理链：</span><span class="sxs-lookup"><span data-stu-id="c0486-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=max)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=max)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0486-122">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="c0486-122">Optional query parameters</span></span>

<span data-ttu-id="c0486-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0486-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

<span data-ttu-id="c0486-124">如果请求包含用于获取经理链的 `$expand=manager($levels=max)` 参数，则还必须包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="c0486-124">If your request includes the `$expand=manager($levels=max)` parameter to get the manager's chain, you must also include the following:</span></span>

- <span data-ttu-id="c0486-125">`$count=true` 查询字符串参数</span><span class="sxs-lookup"><span data-stu-id="c0486-125">`$count=true` query string parameter</span></span>
- <span data-ttu-id="c0486-126">`ConsistencyLevel=eventual` 请求标头</span><span class="sxs-lookup"><span data-stu-id="c0486-126">`ConsistencyLevel=eventual` request header</span></span>

><span data-ttu-id="c0486-127">**注意：** `max` 是 `$levels` 允许的唯一值。</span><span class="sxs-lookup"><span data-stu-id="c0486-127">**Note:** `max` is the only allowed value for `$levels`.</span></span>
> <span data-ttu-id="c0486-128">如果未指定 `$level` 参数，将仅返回直属经理。</span><span class="sxs-lookup"><span data-stu-id="c0486-128">When `$level` parameter is not specified, only the immediate manager is returned.</span></span>  
> <span data-ttu-id="c0486-129">可在 `$expand` 内指定 `$select` 以选择单独的经理属性：`$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="c0486-129">You can specify `$select` inside `$expand` to select the individual managers' properties: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0486-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0486-130">Request headers</span></span>

| <span data-ttu-id="c0486-131">标头</span><span class="sxs-lookup"><span data-stu-id="c0486-131">Header</span></span>       | <span data-ttu-id="c0486-132">值</span><span class="sxs-lookup"><span data-stu-id="c0486-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c0486-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0486-133">Authorization</span></span>  | <span data-ttu-id="c0486-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0486-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0486-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c0486-136">ConsistencyLevel</span></span> | <span data-ttu-id="c0486-137">最终。</span><span class="sxs-lookup"><span data-stu-id="c0486-137">eventual.</span></span> <span data-ttu-id="c0486-138">请求包括 `$expand=manager($levels=max)` 参数时必需。</span><span class="sxs-lookup"><span data-stu-id="c0486-138">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0486-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0486-139">Request body</span></span>

<span data-ttu-id="c0486-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0486-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0486-141">响应</span><span class="sxs-lookup"><span data-stu-id="c0486-141">Response</span></span>

<span data-ttu-id="c0486-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0486-142">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0486-143">示例</span><span class="sxs-lookup"><span data-stu-id="c0486-143">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="c0486-144">示例 1：获取经理</span><span class="sxs-lookup"><span data-stu-id="c0486-144">Example 1: Get manager</span></span>

<span data-ttu-id="c0486-145">以下示例显示获取经理的请求。</span><span class="sxs-lookup"><span data-stu-id="c0486-145">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="c0486-146">请求</span><span class="sxs-lookup"><span data-stu-id="c0486-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0486-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0486-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
# <a name="c"></a>[<span data-ttu-id="c0486-148">C#</span><span class="sxs-lookup"><span data-stu-id="c0486-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0486-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0486-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0486-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0486-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0486-151">Java</span><span class="sxs-lookup"><span data-stu-id="c0486-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c0486-152">响应</span><span class="sxs-lookup"><span data-stu-id="c0486-152">Response</span></span>

<span data-ttu-id="c0486-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0486-153">The following is an example of the response.</span></span>
><span data-ttu-id="c0486-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0486-154">**Note**: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="c0486-155">示例 2：获取直至根级别的经理链</span><span class="sxs-lookup"><span data-stu-id="c0486-155">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="c0486-156">以下示例显示获取直至根级别的经理链的请求。</span><span class="sxs-lookup"><span data-stu-id="c0486-156">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="c0486-157">请求</span><span class="sxs-lookup"><span data-stu-id="c0486-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c0486-158">响应</span><span class="sxs-lookup"><span data-stu-id="c0486-158">Response</span></span>

<span data-ttu-id="c0486-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0486-159">The following is an example of the response.</span></span> <span data-ttu-id="c0486-160">可传递的经理分层显示。</span><span class="sxs-lookup"><span data-stu-id="c0486-160">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="c0486-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0486-161">**Note**: The response object shown here might be shortened for readability.</span></span>
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
