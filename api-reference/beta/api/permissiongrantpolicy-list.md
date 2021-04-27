---
title: 列出 permissionGrantPolicies
description: 检索 permissionGrantPolicy 对象列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 7333c765bd556a4c9bbb9de49f2e82519569258b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052962"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="a8759-103">列出 permissionGrantPolicies</span><span class="sxs-lookup"><span data-stu-id="a8759-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="a8759-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8759-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8759-105">检索 [permissionGrantPolicy 对象](../resources/permissiongrantpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="a8759-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8759-106">权限</span><span class="sxs-lookup"><span data-stu-id="a8759-106">Permissions</span></span>

<span data-ttu-id="a8759-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8759-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8759-109">Permission type</span></span>                        | <span data-ttu-id="a8759-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8759-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8759-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8759-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8759-112">Policy.Read.PermissionGrant、Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a8759-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="a8759-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8759-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8759-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8759-114">Not supported.</span></span> |
| <span data-ttu-id="a8759-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8759-115">Application</span></span>                            | <span data-ttu-id="a8759-116">Policy.Read.PermissionGrant、Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a8759-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8759-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8759-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8759-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a8759-118">Optional query parameters</span></span>

<span data-ttu-id="a8759-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a8759-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8759-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8759-120">Request headers</span></span>

| <span data-ttu-id="a8759-121">名称</span><span class="sxs-lookup"><span data-stu-id="a8759-121">Name</span></span>           | <span data-ttu-id="a8759-122">说明</span><span class="sxs-lookup"><span data-stu-id="a8759-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a8759-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8759-123">Authorization</span></span>  | <span data-ttu-id="a8759-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8759-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8759-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8759-126">Request body</span></span>

<span data-ttu-id="a8759-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8759-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8759-128">响应</span><span class="sxs-lookup"><span data-stu-id="a8759-128">Response</span></span>

<span data-ttu-id="a8759-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a8759-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8759-130">示例</span><span class="sxs-lookup"><span data-stu-id="a8759-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8759-131">请求</span><span class="sxs-lookup"><span data-stu-id="a8759-131">Request</span></span>

<span data-ttu-id="a8759-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8759-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8759-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8759-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies
```
# <a name="c"></a>[<span data-ttu-id="a8759-134">C#</span><span class="sxs-lookup"><span data-stu-id="a8759-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permissiongrantpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8759-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8759-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permissiongrantpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8759-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8759-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permissiongrantpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8759-137">Java</span><span class="sxs-lookup"><span data-stu-id="a8759-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permissiongrantpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8759-138">响应</span><span class="sxs-lookup"><span data-stu-id="a8759-138">Response</span></span>

<span data-ttu-id="a8759-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8759-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a8759-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a8759-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "tier-1",
      "displayName": "Tier 1 Help Desk",
      "description": "Custom permission grant policy for tier 1 help desk.",
      "includes": [
        {
          "id": "198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5",
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
    },
    {
      "id": "microsoft-company-admin",
      "displayName": "Company Admin Policy",
      "description": "Permissions consentable by Company Administrators.",
      "includes": [
        {
          "id": "1f06f3a1-42d3-4243-8fbc-5d0c30d4de4c",
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
          "id": "08619a19-ae6f-406c-b9a0-ea6af1f1558d",
          "permissionClassification": "all",
          "permissionType": "delegated",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": false
        }
      ],
      "excludes": []
    }
  ]
}
```
