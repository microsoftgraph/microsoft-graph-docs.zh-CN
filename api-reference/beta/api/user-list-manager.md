---
title: 列出经理
description: 获取用户的经理。 返回指定为用户经理的用户或联系人。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 32784009419596579551430deee3d8953fc1a139
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086765"
---
# <a name="list-manager"></a><span data-ttu-id="6cee7-104">列出经理</span><span class="sxs-lookup"><span data-stu-id="6cee7-104">List manager</span></span>

<span data-ttu-id="6cee7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cee7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cee7-106">返回指定为用户经理的用户或组织联系人。</span><span class="sxs-lookup"><span data-stu-id="6cee7-106">Returns the user or organizational contact assigned as the user's manager.</span></span> <span data-ttu-id="6cee7-107">（可选）您可以将管理器的链展开到根节点。</span><span class="sxs-lookup"><span data-stu-id="6cee7-107">Optionally, you can expand the manager's chain up to the root node.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cee7-108">权限</span><span class="sxs-lookup"><span data-stu-id="6cee7-108">Permissions</span></span>

<span data-ttu-id="6cee7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cee7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cee7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cee7-111">Permission type</span></span>      | <span data-ttu-id="6cee7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cee7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cee7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cee7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6cee7-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cee7-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6cee7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cee7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cee7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cee7-116">Not supported.</span></span>    |
|<span data-ttu-id="6cee7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cee7-117">Application</span></span> | <span data-ttu-id="6cee7-118">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cee7-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6cee7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cee7-119">HTTP request</span></span>

<span data-ttu-id="6cee7-120">获取经理：</span><span class="sxs-lookup"><span data-stu-id="6cee7-120">Get the manager:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
<span data-ttu-id="6cee7-121">获取管理链：</span><span class="sxs-lookup"><span data-stu-id="6cee7-121">Get the management chain:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=max)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=max)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cee7-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6cee7-122">Optional query parameters</span></span>

<span data-ttu-id="6cee7-123">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6cee7-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>  

<span data-ttu-id="6cee7-124">如果您的请求包含 `$expand=manager($levels=max)` 用于获取经理的链的参数，则还必须包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="6cee7-124">If your request includes the `$expand=manager($levels=max)` parameter to get the manager's chain, you must also include the following:</span></span>

- <span data-ttu-id="6cee7-125">`$count=true` 查询字符串参数</span><span class="sxs-lookup"><span data-stu-id="6cee7-125">`$count=true` query string parameter</span></span>
- <span data-ttu-id="6cee7-126">`ConsistencyLevel=eventual` 请求标头</span><span class="sxs-lookup"><span data-stu-id="6cee7-126">`ConsistencyLevel=eventual` request header</span></span>

><span data-ttu-id="6cee7-127">**注意：** `max` 是允许的唯一值 `$levels` 。</span><span class="sxs-lookup"><span data-stu-id="6cee7-127">**Note:** `max` is the only allowed value for `$levels`.</span></span>
> <span data-ttu-id="6cee7-128">如果 `$level` 未指定此参数，则仅返回直属管理器。</span><span class="sxs-lookup"><span data-stu-id="6cee7-128">When the `$level` parameter is not specified, only the immediate manager is returned.</span></span>  
> <span data-ttu-id="6cee7-129">您可以 `$select` 在内指定 `$expand` ，以选择单个经理的属性： `$expand=manager($levels=max;$select=id,displayName)`</span><span class="sxs-lookup"><span data-stu-id="6cee7-129">You can specify `$select` inside `$expand` to select the individual manager's properties: `$expand=manager($levels=max;$select=id,displayName)`</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cee7-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cee7-130">Request headers</span></span>

| <span data-ttu-id="6cee7-131">标头</span><span class="sxs-lookup"><span data-stu-id="6cee7-131">Header</span></span>       | <span data-ttu-id="6cee7-132">值</span><span class="sxs-lookup"><span data-stu-id="6cee7-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6cee7-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cee7-133">Authorization</span></span>  | <span data-ttu-id="6cee7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cee7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6cee7-136">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6cee7-136">ConsistencyLevel</span></span> | <span data-ttu-id="6cee7-137">最终。</span><span class="sxs-lookup"><span data-stu-id="6cee7-137">eventual.</span></span> <span data-ttu-id="6cee7-138">请求包括参数时必需 `$expand=manager($levels=max)` 。</span><span class="sxs-lookup"><span data-stu-id="6cee7-138">Required when the request includes the `$expand=manager($levels=max)` parameter.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cee7-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cee7-139">Request body</span></span>

<span data-ttu-id="6cee7-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cee7-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cee7-141">响应</span><span class="sxs-lookup"><span data-stu-id="6cee7-141">Response</span></span>

<span data-ttu-id="6cee7-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6cee7-142">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cee7-143">示例</span><span class="sxs-lookup"><span data-stu-id="6cee7-143">Examples</span></span>

### <a name="example-1-get-manager"></a><span data-ttu-id="6cee7-144">示例1：获取管理器</span><span class="sxs-lookup"><span data-stu-id="6cee7-144">Example 1: Get manager</span></span>

<span data-ttu-id="6cee7-145">下面的示例展示了获取经理的请求。</span><span class="sxs-lookup"><span data-stu-id="6cee7-145">The following example shows a request to get the manager.</span></span>

#### <a name="request"></a><span data-ttu-id="6cee7-146">请求</span><span class="sxs-lookup"><span data-stu-id="6cee7-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6cee7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cee7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```

#### <a name="response"></a><span data-ttu-id="6cee7-148">响应</span><span class="sxs-lookup"><span data-stu-id="6cee7-148">Response</span></span>

<span data-ttu-id="6cee7-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cee7-149">The following is an example of the response.</span></span>
><span data-ttu-id="6cee7-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6cee7-150">**Note**: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a><span data-ttu-id="6cee7-151">示例2：获取到根级别的管理器链</span><span class="sxs-lookup"><span data-stu-id="6cee7-151">Example 2: Get manager chain up to the root level</span></span>

<span data-ttu-id="6cee7-152">下面的示例演示将管理器链向上获取到根级别的请求。</span><span class="sxs-lookup"><span data-stu-id="6cee7-152">The following example shows a request to get the manager chain up to the root level.</span></span>

#### <a name="request"></a><span data-ttu-id="6cee7-153">请求</span><span class="sxs-lookup"><span data-stu-id="6cee7-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6cee7-154">响应</span><span class="sxs-lookup"><span data-stu-id="6cee7-154">Response</span></span>

<span data-ttu-id="6cee7-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6cee7-155">The following is an example of the response.</span></span> <span data-ttu-id="6cee7-156">可传递的管理器分层显示。</span><span class="sxs-lookup"><span data-stu-id="6cee7-156">Transitive managers are displayed hierarchically.</span></span>

><span data-ttu-id="6cee7-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6cee7-157">**Note**: The response object shown here might be shortened for readability.</span></span>
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
