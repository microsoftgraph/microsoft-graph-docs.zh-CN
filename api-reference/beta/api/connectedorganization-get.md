---
title: 获取 connectedOrganization
description: 检索 connectedorganization 对象的属性和关系。
author: markwahl-msft
ms.prod: governance
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: ec4bfa06754f9381c19154e886691f7657e0ab18
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437483"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="fe6e7-103">获取 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="fe6e7-103">Get connectedOrganization</span></span>

<span data-ttu-id="fe6e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe6e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe6e7-105">检索 [connectedOrganization](../resources/connectedorganization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe6e7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fe6e7-106">Permissions</span></span>

<span data-ttu-id="fe6e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe6e7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe6e7-109">Permission type</span></span>|<span data-ttu-id="fe6e7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe6e7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="fe6e7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe6e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe6e7-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe6e7-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="fe6e7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe6e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe6e7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-114">Not supported.</span></span> |
| <span data-ttu-id="fe6e7-115">Application</span><span class="sxs-lookup"><span data-stu-id="fe6e7-115">Application</span></span>                            | <span data-ttu-id="fe6e7-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe6e7-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe6e7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe6e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe6e7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe6e7-118">Optional query parameters</span></span>

<span data-ttu-id="fe6e7-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fe6e7-120">例如，若要仅检索标识源，请添加 `$select=identitySources` 。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="fe6e7-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe6e7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe6e7-122">Request headers</span></span>

|<span data-ttu-id="fe6e7-123">名称</span><span class="sxs-lookup"><span data-stu-id="fe6e7-123">Name</span></span>|<span data-ttu-id="fe6e7-124">说明</span><span class="sxs-lookup"><span data-stu-id="fe6e7-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fe6e7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe6e7-125">Authorization</span></span>|<span data-ttu-id="fe6e7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe6e7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe6e7-128">Request body</span></span>

<span data-ttu-id="fe6e7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe6e7-130">响应</span><span class="sxs-lookup"><span data-stu-id="fe6e7-130">Response</span></span>

<span data-ttu-id="fe6e7-131">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe6e7-132">示例</span><span class="sxs-lookup"><span data-stu-id="fe6e7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe6e7-133">请求</span><span class="sxs-lookup"><span data-stu-id="fe6e7-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fe6e7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe6e7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="fe6e7-135">C#</span><span class="sxs-lookup"><span data-stu-id="fe6e7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe6e7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe6e7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe6e7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe6e7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe6e7-138">Java</span><span class="sxs-lookup"><span data-stu-id="fe6e7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe6e7-139">响应</span><span class="sxs-lookup"><span data-stu-id="fe6e7-139">Response</span></span>

<span data-ttu-id="fe6e7-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe6e7-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
  "displayName": "Wingtip Toys",
  "description": "Wingtip Toys",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-05-13T15:18:04.81Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-05-13T15:18:04.81Z",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
      "displayName": "Wingtip Toys Co"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


