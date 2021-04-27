---
title: 获取 permissionGrantPolicy
description: 检索单个 permissionGrantPolicy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: f1aa51b9e31924443f6f276333bd9c284185a8c0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052955"
---
# <a name="get-permissiongrantpolicy"></a><span data-ttu-id="f8354-103">获取 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="f8354-103">Get permissionGrantPolicy</span></span>

<span data-ttu-id="f8354-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8354-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8354-105">检索单个 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8354-105">Retrieve a single [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8354-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8354-106">Permissions</span></span>

<span data-ttu-id="f8354-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8354-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8354-109">Permission type</span></span>                        | <span data-ttu-id="f8354-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8354-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8354-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8354-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8354-112">Policy.Read.PermissionGrant、Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f8354-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="f8354-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8354-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8354-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8354-114">Not supported.</span></span> |
| <span data-ttu-id="f8354-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8354-115">Application</span></span>                            | <span data-ttu-id="f8354-116">Policy.Read.PermissionGrant、Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f8354-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8354-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8354-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8354-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8354-118">Optional query parameters</span></span>

<span data-ttu-id="f8354-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8354-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8354-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8354-120">Request headers</span></span>

| <span data-ttu-id="f8354-121">名称</span><span class="sxs-lookup"><span data-stu-id="f8354-121">Name</span></span>           | <span data-ttu-id="f8354-122">说明</span><span class="sxs-lookup"><span data-stu-id="f8354-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f8354-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8354-123">Authorization</span></span>  | <span data-ttu-id="f8354-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8354-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8354-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8354-126">Request body</span></span>

<span data-ttu-id="f8354-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8354-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8354-128">响应</span><span class="sxs-lookup"><span data-stu-id="f8354-128">Response</span></span>

<span data-ttu-id="f8354-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8354-129">If successful, this method returns a `200 OK` response code and the requested [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8354-130">示例</span><span class="sxs-lookup"><span data-stu-id="f8354-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8354-131">请求</span><span class="sxs-lookup"><span data-stu-id="f8354-131">Request</span></span>

<span data-ttu-id="f8354-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8354-132">The following is an example of the request.</span></span> <span data-ttu-id="f8354-133">此示例中，请求的策略是内置权限授予策略，其中包括针对已验证发布者的应用或在此租户中注册的应用分类的低委派 `microsoft-user-default-low` 权限。</span><span class="sxs-lookup"><span data-stu-id="f8354-133">In this example, the requested policy is the built-in permission grant policy `microsoft-user-default-low`, which includes delegated permissions classified low, for apps from verified publishers or apps registered in this tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="f8354-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8354-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-user-default-low
```
# <a name="c"></a>[<span data-ttu-id="f8354-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8354-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8354-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8354-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8354-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8354-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8354-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8354-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8354-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8354-139">Response</span></span>

<span data-ttu-id="f8354-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8354-140">The following is an example of the response.</span></span> <span data-ttu-id="f8354-141">策略有两个条件集，一个条件集与为此租户中注册的客户端应用分类的委派权限匹配，另一个条件集与为来自已验证发布者 (的应用分类的委派权限匹配，而不管该应用程序在 `includes` `low`) 中注册 `low` 哪个租户。</span><span class="sxs-lookup"><span data-stu-id="f8354-141">The policy has two `includes` condition sets, one which matches with delegated permission classified `low` for client apps registered in this tenant, and the other which matches delegated permissions classified `low` for apps from verified publishers (regardless of which tenant the app is registered in).</span></span>

> <span data-ttu-id="f8354-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8354-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "microsoft-user-default-low",
    "displayName": "Default User Low Risk Policy",
    "description": "All low risk permissions are consentable by member type users by default.",
    "includes": [
        {
            "id": "cb0c20dd-919d-40c5-ba6d-7ffb233b4b0b",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "11e37ee2-48fe-42e0-aab9-07d0bb165353" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": false
        },
        {
            "id": "8ce99f96-730c-4ebd-8397-07ee65942b97",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "all" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": true
        }
    ],
    "excludes": []
}
```
