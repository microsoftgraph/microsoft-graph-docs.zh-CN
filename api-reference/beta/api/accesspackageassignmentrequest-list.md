---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d97b0f7c3f06652a7d22d0b803d471b95a233e62
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935247"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="634e0-103">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="634e0-103">List accessPackageAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="634e0-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="634e0-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="634e0-105">生成的列表包括在所有目录和访问包中，呼叫者有权读取的所有工作分配请求、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="634e0-105">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="634e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="634e0-106">Permissions</span></span>

<span data-ttu-id="634e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="634e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="634e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="634e0-109">Permission type</span></span>                        | <span data-ttu-id="634e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="634e0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="634e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="634e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="634e0-112">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="634e0-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="634e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="634e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="634e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="634e0-114">Not supported.</span></span> |
| <span data-ttu-id="634e0-115">Application</span><span class="sxs-lookup"><span data-stu-id="634e0-115">Application</span></span>                            | <span data-ttu-id="634e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="634e0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="634e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="634e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="634e0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="634e0-118">Optional query parameters</span></span>

<span data-ttu-id="634e0-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="634e0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="634e0-120">例如，若要检索每个请求的访问包，请`$expand=accessPackage`在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="634e0-120">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="634e0-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="634e0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="634e0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="634e0-122">Request headers</span></span>

| <span data-ttu-id="634e0-123">名称</span><span class="sxs-lookup"><span data-stu-id="634e0-123">Name</span></span>      |<span data-ttu-id="634e0-124">说明</span><span class="sxs-lookup"><span data-stu-id="634e0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="634e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="634e0-125">Authorization</span></span> | <span data-ttu-id="634e0-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="634e0-126">Bearer \{token\}.</span></span> <span data-ttu-id="634e0-127">必填。</span><span class="sxs-lookup"><span data-stu-id="634e0-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="634e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="634e0-128">Request body</span></span>

<span data-ttu-id="634e0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="634e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="634e0-130">响应</span><span class="sxs-lookup"><span data-stu-id="634e0-130">Response</span></span>

<span data-ttu-id="634e0-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="634e0-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="634e0-132">示例</span><span class="sxs-lookup"><span data-stu-id="634e0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="634e0-133">请求</span><span class="sxs-lookup"><span data-stu-id="634e0-133">Request</span></span>

<span data-ttu-id="634e0-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="634e0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

### <a name="response"></a><span data-ttu-id="634e0-135">响应</span><span class="sxs-lookup"><span data-stu-id="634e0-135">Response</span></span>

<span data-ttu-id="634e0-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="634e0-136">The following is an example of the response.</span></span>

> <span data-ttu-id="634e0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="634e0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
