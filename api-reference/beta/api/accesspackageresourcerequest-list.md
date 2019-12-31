---
title: 列出 accessPackageResourceRequests
description: 检索 accessPackageResourceRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5e320cff583c351e824d1ff472ebc5b60daa61a
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911616"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="63520-103">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="63520-103">List accessPackageResourceRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63520-104">检索[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="63520-104">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="63520-105">权限</span><span class="sxs-lookup"><span data-stu-id="63520-105">Permissions</span></span>

<span data-ttu-id="63520-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63520-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63520-108">Permission type</span></span>                        | <span data-ttu-id="63520-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63520-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63520-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63520-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="63520-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63520-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="63520-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63520-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63520-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="63520-113">Not supported.</span></span> |
| <span data-ttu-id="63520-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63520-114">Application</span></span>                            | <span data-ttu-id="63520-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63520-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63520-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63520-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63520-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63520-117">Optional query parameters</span></span>

<span data-ttu-id="63520-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63520-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="63520-119">例如，若要检索请求将资源添加到目录中的谁，请在`$expand=requestor`查询中加入。</span><span class="sxs-lookup"><span data-stu-id="63520-119">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="63520-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="63520-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="63520-121">请求头</span><span class="sxs-lookup"><span data-stu-id="63520-121">Request headers</span></span>

| <span data-ttu-id="63520-122">名称</span><span class="sxs-lookup"><span data-stu-id="63520-122">Name</span></span>      |<span data-ttu-id="63520-123">说明</span><span class="sxs-lookup"><span data-stu-id="63520-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63520-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="63520-124">Authorization</span></span> | <span data-ttu-id="63520-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63520-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63520-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63520-127">Request body</span></span>

<span data-ttu-id="63520-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63520-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63520-129">响应</span><span class="sxs-lookup"><span data-stu-id="63520-129">Response</span></span>

<span data-ttu-id="63520-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="63520-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63520-131">示例</span><span class="sxs-lookup"><span data-stu-id="63520-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63520-132">请求</span><span class="sxs-lookup"><span data-stu-id="63520-132">Request</span></span>

<span data-ttu-id="63520-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63520-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63520-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="63520-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63520-135">C#</span><span class="sxs-lookup"><span data-stu-id="63520-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63520-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63520-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63520-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63520-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63520-138">响应</span><span class="sxs-lookup"><span data-stu-id="63520-138">Response</span></span>

<span data-ttu-id="63520-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63520-139">The following is an example of the response.</span></span>

> <span data-ttu-id="63520-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63520-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
