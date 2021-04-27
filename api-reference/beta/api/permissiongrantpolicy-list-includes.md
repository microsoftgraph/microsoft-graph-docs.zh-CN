---
title: 列表包括 permissionGrantPolicy 的集合
description: 检索条件集的列表，这些条件集描述权限授予策略中包括权限授予事件的条件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: c1fc71f56c662b1558d11fe10404a67395fb4813
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055412"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="db20e-103">列表包括 permissionGrantPolicy 的集合</span><span class="sxs-lookup"><span data-stu-id="db20e-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="db20e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db20e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db20e-105">检索包含在[permissionGrantPolicy 中的条件集](../resources/permissiongrantpolicy.md)。 </span><span class="sxs-lookup"><span data-stu-id="db20e-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db20e-106">权限</span><span class="sxs-lookup"><span data-stu-id="db20e-106">Permissions</span></span>

<span data-ttu-id="db20e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db20e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db20e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db20e-109">Permission type</span></span>      | <span data-ttu-id="db20e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db20e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db20e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db20e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db20e-112">Policy.Read.PermissionGrant、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="db20e-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="db20e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db20e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db20e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db20e-114">Not supported.</span></span>    |
|<span data-ttu-id="db20e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db20e-115">Application</span></span> | <span data-ttu-id="db20e-116">Policy.Read.PermissionGrant、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="db20e-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db20e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db20e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db20e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db20e-118">Optional query parameters</span></span>

<span data-ttu-id="db20e-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="db20e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db20e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db20e-120">Request headers</span></span>

| <span data-ttu-id="db20e-121">名称</span><span class="sxs-lookup"><span data-stu-id="db20e-121">Name</span></span>           | <span data-ttu-id="db20e-122">说明</span><span class="sxs-lookup"><span data-stu-id="db20e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="db20e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db20e-123">Authorization</span></span>  | <span data-ttu-id="db20e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db20e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db20e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db20e-126">Request body</span></span>

<span data-ttu-id="db20e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db20e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db20e-128">响应</span><span class="sxs-lookup"><span data-stu-id="db20e-128">Response</span></span>

<span data-ttu-id="db20e-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db20e-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db20e-130">示例</span><span class="sxs-lookup"><span data-stu-id="db20e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db20e-131">请求</span><span class="sxs-lookup"><span data-stu-id="db20e-131">Request</span></span>

<span data-ttu-id="db20e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db20e-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="db20e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db20e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-application-admin/includes
```
# <a name="c"></a>[<span data-ttu-id="db20e-134">C#</span><span class="sxs-lookup"><span data-stu-id="db20e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db20e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db20e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db20e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db20e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db20e-137">Java</span><span class="sxs-lookup"><span data-stu-id="db20e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db20e-138">响应</span><span class="sxs-lookup"><span data-stu-id="db20e-138">Response</span></span>

<span data-ttu-id="db20e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db20e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="db20e-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db20e-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
