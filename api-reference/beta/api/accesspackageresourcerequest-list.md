---
title: 列出 accessPackageResourceRequests
description: 检索 accessPackageResourceRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb9110815baf6290de2e2abd897dd193a1d93f66
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345175"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="35ce5-103">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="35ce5-103">List accessPackageResourceRequests</span></span>

<span data-ttu-id="35ce5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35ce5-105">检索[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="35ce5-105">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="35ce5-106">权限</span><span class="sxs-lookup"><span data-stu-id="35ce5-106">Permissions</span></span>

<span data-ttu-id="35ce5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35ce5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35ce5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="35ce5-109">Permission type</span></span>                        | <span data-ttu-id="35ce5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35ce5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35ce5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35ce5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35ce5-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="35ce5-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="35ce5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35ce5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35ce5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="35ce5-114">Not supported.</span></span> |
| <span data-ttu-id="35ce5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="35ce5-115">Application</span></span>                            | <span data-ttu-id="35ce5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35ce5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35ce5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35ce5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35ce5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35ce5-118">Optional query parameters</span></span>

<span data-ttu-id="35ce5-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35ce5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="35ce5-120">例如，若要检索请求将资源添加到目录中的谁，请 `$expand=requestor` 在查询中加入。</span><span class="sxs-lookup"><span data-stu-id="35ce5-120">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="35ce5-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="35ce5-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="35ce5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="35ce5-122">Request headers</span></span>

| <span data-ttu-id="35ce5-123">名称</span><span class="sxs-lookup"><span data-stu-id="35ce5-123">Name</span></span>      |<span data-ttu-id="35ce5-124">说明</span><span class="sxs-lookup"><span data-stu-id="35ce5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35ce5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="35ce5-125">Authorization</span></span> | <span data-ttu-id="35ce5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35ce5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35ce5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="35ce5-128">Request body</span></span>

<span data-ttu-id="35ce5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35ce5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35ce5-130">响应</span><span class="sxs-lookup"><span data-stu-id="35ce5-130">Response</span></span>

<span data-ttu-id="35ce5-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="35ce5-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35ce5-132">示例</span><span class="sxs-lookup"><span data-stu-id="35ce5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35ce5-133">请求</span><span class="sxs-lookup"><span data-stu-id="35ce5-133">Request</span></span>

<span data-ttu-id="35ce5-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="35ce5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35ce5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="35ce5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="c"></a>[<span data-ttu-id="35ce5-136">C#</span><span class="sxs-lookup"><span data-stu-id="35ce5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35ce5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35ce5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35ce5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35ce5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35ce5-139">响应</span><span class="sxs-lookup"><span data-stu-id="35ce5-139">Response</span></span>

<span data-ttu-id="35ce5-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="35ce5-140">The following is an example of the response.</span></span>

> <span data-ttu-id="35ce5-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="35ce5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
