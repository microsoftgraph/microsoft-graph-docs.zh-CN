---
title: 列出 accessPackageAssignments
description: 检索 accesspackageassignment 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a14bfbdf7785c378a132d308711d4fd21a815413
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108425"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="67335-103">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="67335-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67335-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignment](../resources/accesspackageassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="67335-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="67335-105">生成的列表包括呼叫者在所有目录和访问包中具有读取权限的所有工作分配、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="67335-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="67335-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="67335-106">Permissions</span></span>

<span data-ttu-id="67335-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67335-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67335-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67335-109">Permission type</span></span>                        | <span data-ttu-id="67335-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67335-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="67335-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67335-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="67335-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67335-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="67335-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67335-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67335-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="67335-114">Not supported.</span></span> |
| <span data-ttu-id="67335-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67335-115">Application</span></span>                            | <span data-ttu-id="67335-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67335-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67335-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67335-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67335-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="67335-118">Optional query parameters</span></span>

<span data-ttu-id="67335-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="67335-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="67335-120">例如，若要同时返回目标用户和访问包，请包括`$expand=target,accessPackage`。</span><span class="sxs-lookup"><span data-stu-id="67335-120">For example, to also return the target user and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="67335-121">若要仅检索已传递的工作分配，可以`$filter=assignmentState eq 'Delivered'`包含查询。</span><span class="sxs-lookup"><span data-stu-id="67335-121">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="67335-122">若要仅检索特定用户的工作分配，可以包含一个查询，该查询具有针对该用户`$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`的对象 ID 的工作分配。</span><span class="sxs-lookup"><span data-stu-id="67335-122">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="67335-123">若要仅检索特定用户和特定访问包的工作分配，可以包含具有针对该用户`$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`的访问包和对象 ID 的工作分配的查询。</span><span class="sxs-lookup"><span data-stu-id="67335-123">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>

<span data-ttu-id="67335-124">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="67335-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="67335-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="67335-125">Request headers</span></span>

| <span data-ttu-id="67335-126">名称</span><span class="sxs-lookup"><span data-stu-id="67335-126">Name</span></span>      |<span data-ttu-id="67335-127">说明</span><span class="sxs-lookup"><span data-stu-id="67335-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67335-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="67335-128">Authorization</span></span> | <span data-ttu-id="67335-129">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="67335-129">Bearer \{token\}.</span></span> <span data-ttu-id="67335-130">必填。</span><span class="sxs-lookup"><span data-stu-id="67335-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67335-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="67335-131">Request body</span></span>

<span data-ttu-id="67335-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67335-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67335-133">响应</span><span class="sxs-lookup"><span data-stu-id="67335-133">Response</span></span>

<span data-ttu-id="67335-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignment](../resources/accesspackageassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="67335-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67335-135">示例</span><span class="sxs-lookup"><span data-stu-id="67335-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67335-136">请求</span><span class="sxs-lookup"><span data-stu-id="67335-136">Request</span></span>

<span data-ttu-id="67335-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67335-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67335-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="67335-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="67335-139">C#</span><span class="sxs-lookup"><span data-stu-id="67335-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67335-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67335-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67335-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67335-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67335-142">响应</span><span class="sxs-lookup"><span data-stu-id="67335-142">Response</span></span>

<span data-ttu-id="67335-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67335-143">The following is an example of the response.</span></span>

> <span data-ttu-id="67335-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67335-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
