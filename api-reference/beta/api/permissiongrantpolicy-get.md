---
title: 获取 permissionGrantPolicy
description: 检索单个 permissionGrantPolicy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8bfef7bdb0c3965aed1a9362fed81008f4925519
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460226"
---
# <a name="get-permissiongrantpolicy"></a><span data-ttu-id="d6e69-103">获取 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="d6e69-103">Get permissionGrantPolicy</span></span>

<span data-ttu-id="d6e69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e69-105">检索单个 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6e69-105">Retrieve a single [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6e69-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6e69-106">Permissions</span></span>

<span data-ttu-id="d6e69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6e69-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6e69-109">Permission type</span></span>                        | <span data-ttu-id="d6e69-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6e69-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6e69-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e69-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6e69-112">PermissionGrant （PermissionGrant）。</span><span class="sxs-lookup"><span data-stu-id="d6e69-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="d6e69-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6e69-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6e69-114">Not supported.</span></span> |
| <span data-ttu-id="d6e69-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6e69-115">Application</span></span>                            | <span data-ttu-id="d6e69-116">PermissionGrant （PermissionGrant）。</span><span class="sxs-lookup"><span data-stu-id="d6e69-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6e69-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6e69-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6e69-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6e69-118">Optional query parameters</span></span>

<span data-ttu-id="d6e69-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6e69-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6e69-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6e69-120">Request headers</span></span>

| <span data-ttu-id="d6e69-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6e69-121">Name</span></span>           | <span data-ttu-id="d6e69-122">说明</span><span class="sxs-lookup"><span data-stu-id="d6e69-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d6e69-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6e69-123">Authorization</span></span>  | <span data-ttu-id="d6e69-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6e69-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6e69-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6e69-126">Request body</span></span>

<span data-ttu-id="d6e69-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6e69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6e69-128">响应</span><span class="sxs-lookup"><span data-stu-id="d6e69-128">Response</span></span>

<span data-ttu-id="d6e69-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6e69-129">If successful, this method returns a `200 OK` response code and the requested [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6e69-130">示例</span><span class="sxs-lookup"><span data-stu-id="d6e69-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6e69-131">请求</span><span class="sxs-lookup"><span data-stu-id="d6e69-131">Request</span></span>

<span data-ttu-id="d6e69-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6e69-132">The following is an example of the request.</span></span> <span data-ttu-id="d6e69-133">在此示例中，请求的策略是内置权限授予策略 `microsoft-user-default-low` ，其中包括从已验证的发布者或在此租户中注册的应用程序中的应用程序分类较低的代理权限。</span><span class="sxs-lookup"><span data-stu-id="d6e69-133">In this example, the requested policy is the built-in permission grant policy `microsoft-user-default-low`, which includes delegated permissions classified low, for apps from verified publishers or apps registered in this tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6e69-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6e69-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-user-default-low
```
# <a name="c"></a>[<span data-ttu-id="d6e69-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6e69-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6e69-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6e69-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6e69-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6e69-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6e69-138">响应</span><span class="sxs-lookup"><span data-stu-id="d6e69-138">Response</span></span>

<span data-ttu-id="d6e69-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d6e69-139">The following is an example of the response.</span></span> <span data-ttu-id="d6e69-140">策略有两个 `includes` 条件集，其中一个与 `low` 为在此租户中注册的客户端应用程序分类的委派权限相匹配，另一个与从已验证的发布者的应用程序分类的委派权限相匹配 `low` (无论在) 中注册了应用程序的是哪个租户。</span><span class="sxs-lookup"><span data-stu-id="d6e69-140">The policy has two `includes` condition sets, one which matches with delegated permission classified `low` for client apps registered in this tenant, and the other which matches delegated permissions classified `low` for apps from verified publishers (regardless of which tenant the app is registered in).</span></span>

> <span data-ttu-id="d6e69-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d6e69-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
