---
title: List excludes collection of permissionGrantPolicy
description: 检索描述权限授予策略中排除权限授予事件的条件集列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: cdcfef61ef4b0f3bd1a04d2e52409564a74dc253
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448100"
---
# <a name="list-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="c4b1d-103">List excludes collection of permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="c4b1d-103">List excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="c4b1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4b1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4b1d-105">检索在[permissionGrantPolicy](../resources/permissiongrantpolicy.md)中排除的条件集。 </span><span class="sxs-lookup"><span data-stu-id="c4b1d-105">Retrieve the condition sets which are *excluded* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b1d-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4b1d-106">Permissions</span></span>

<span data-ttu-id="c4b1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b1d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4b1d-109">Permission type</span></span>      | <span data-ttu-id="c4b1d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4b1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4b1d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4b1d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4b1d-112">Policy.Read.PermissionGrant、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4b1d-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="c4b1d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4b1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4b1d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-114">Not supported.</span></span>    |
|<span data-ttu-id="c4b1d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4b1d-115">Application</span></span> | <span data-ttu-id="c4b1d-116">Policy.Read.PermissionGrant、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4b1d-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4b1d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4b1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4b1d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4b1d-118">Optional query parameters</span></span>

<span data-ttu-id="c4b1d-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4b1d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4b1d-120">Request headers</span></span>

| <span data-ttu-id="c4b1d-121">名称</span><span class="sxs-lookup"><span data-stu-id="c4b1d-121">Name</span></span>           | <span data-ttu-id="c4b1d-122">说明</span><span class="sxs-lookup"><span data-stu-id="c4b1d-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c4b1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4b1d-123">Authorization</span></span>  | <span data-ttu-id="c4b1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4b1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4b1d-126">Request body</span></span>

<span data-ttu-id="c4b1d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4b1d-128">响应</span><span class="sxs-lookup"><span data-stu-id="c4b1d-128">Response</span></span>

<span data-ttu-id="c4b1d-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b1d-130">示例</span><span class="sxs-lookup"><span data-stu-id="c4b1d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4b1d-131">请求</span><span class="sxs-lookup"><span data-stu-id="c4b1d-131">Request</span></span>

<span data-ttu-id="c4b1d-132">下面是检索内置权限授予策略的排除条件集的请求示例 `microsoft-application-admin` 。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-132">The following is an example of the request to retrieve the **excludes** condition sets of the built-on permission grant policy `microsoft-application-admin`.</span></span> <span data-ttu-id="c4b1d-133">此权限授予策略包括所有委派权限，以及除 Microsoft Graph 的应用程序权限和 Azure AD Graph 的应用程序权限之外的所有应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-133">This permission grant policy includes all delegated permissions, and all application permissions excluding application permissions for Microsoft Graph and application permissions for Azure AD Graph.</span></span>



# <a name="http"></a>[<span data-ttu-id="c4b1d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4b1d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_excludes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/excludes
```
# <a name="c"></a>[<span data-ttu-id="c4b1d-135">C#</span><span class="sxs-lookup"><span data-stu-id="c4b1d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4b1d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4b1d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4b1d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4b1d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4b1d-138">Java</span><span class="sxs-lookup"><span data-stu-id="c4b1d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4b1d-139">响应</span><span class="sxs-lookup"><span data-stu-id="c4b1d-139">Response</span></span>

<span data-ttu-id="c4b1d-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="c4b1d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4b1d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "c85b029f-4abf-47d8-ae61-d2a38299033a",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000003-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "2a1fbb36-9d9a-42d8-8804-de2aa45aca80",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000002-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
