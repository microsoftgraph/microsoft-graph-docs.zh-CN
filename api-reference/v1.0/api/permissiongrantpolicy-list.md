---
title: 列出 permissionGrantPolicies
description: 检索 permissionGrantPolicy 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 755d2146907c77baa342a0f1b8abd4ea32b87df4
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524269"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="a49b8-103">列出 permissionGrantPolicies</span><span class="sxs-lookup"><span data-stu-id="a49b8-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="a49b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a49b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a49b8-105">检索 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a49b8-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a49b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="a49b8-106">Permissions</span></span>

<span data-ttu-id="a49b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a49b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a49b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a49b8-109">Permission type</span></span>                        | <span data-ttu-id="a49b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a49b8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a49b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a49b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a49b8-112">PermissionGrant （PermissionGrant）。</span><span class="sxs-lookup"><span data-stu-id="a49b8-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="a49b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a49b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a49b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a49b8-114">Not supported.</span></span> |
| <span data-ttu-id="a49b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a49b8-115">Application</span></span>                            | <span data-ttu-id="a49b8-116">PermissionGrant （PermissionGrant）。</span><span class="sxs-lookup"><span data-stu-id="a49b8-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="a49b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a49b8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a49b8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a49b8-118">Optional query parameters</span></span>

<span data-ttu-id="a49b8-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a49b8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a49b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a49b8-120">Request headers</span></span>

| <span data-ttu-id="a49b8-121">名称</span><span class="sxs-lookup"><span data-stu-id="a49b8-121">Name</span></span>           | <span data-ttu-id="a49b8-122">说明</span><span class="sxs-lookup"><span data-stu-id="a49b8-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a49b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a49b8-123">Authorization</span></span>  | <span data-ttu-id="a49b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a49b8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a49b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a49b8-126">Request body</span></span>

<span data-ttu-id="a49b8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a49b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a49b8-128">响应</span><span class="sxs-lookup"><span data-stu-id="a49b8-128">Response</span></span>

<span data-ttu-id="a49b8-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a49b8-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a49b8-130">示例</span><span class="sxs-lookup"><span data-stu-id="a49b8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a49b8-131">请求</span><span class="sxs-lookup"><span data-stu-id="a49b8-131">Request</span></span>

<span data-ttu-id="a49b8-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a49b8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a49b8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a49b8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
```
# <a name="c"></a>[<span data-ttu-id="a49b8-134">C#</span><span class="sxs-lookup"><span data-stu-id="a49b8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permissiongrantpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a49b8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a49b8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permissiongrantpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a49b8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a49b8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permissiongrantpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a49b8-137">Java</span><span class="sxs-lookup"><span data-stu-id="a49b8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permissiongrantpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a49b8-138">响应</span><span class="sxs-lookup"><span data-stu-id="a49b8-138">Response</span></span>

<span data-ttu-id="a49b8-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a49b8-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a49b8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a49b8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
