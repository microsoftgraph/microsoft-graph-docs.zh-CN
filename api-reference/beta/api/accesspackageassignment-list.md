---
title: 列出 accessPackageAssignments
description: 检索 accesspackageassignment 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fa93152cdd390093ceeedb061649af018c28808a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868028"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="64cf3-103">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="64cf3-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64cf3-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignment](../resources/accesspackageassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="64cf3-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="64cf3-105">生成的列表包括呼叫者在所有目录和访问包中具有读取权限的所有工作分配、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="64cf3-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="64cf3-106">权限</span><span class="sxs-lookup"><span data-stu-id="64cf3-106">Permissions</span></span>

<span data-ttu-id="64cf3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64cf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64cf3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64cf3-109">Permission type</span></span>                        | <span data-ttu-id="64cf3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64cf3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="64cf3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64cf3-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="64cf3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cf3-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="64cf3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64cf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64cf3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64cf3-114">Not supported.</span></span> |
| <span data-ttu-id="64cf3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64cf3-115">Application</span></span>                            | <span data-ttu-id="64cf3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64cf3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64cf3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64cf3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64cf3-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="64cf3-118">Optional query parameters</span></span>

<span data-ttu-id="64cf3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64cf3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64cf3-120">例如，若要仅检索已传递的工作分配，可以包含`$filter=assignmentState eq 'Delivered'`查询。</span><span class="sxs-lookup"><span data-stu-id="64cf3-120">For example, to retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="64cf3-121">若要仅检索特定用户的工作分配，可以包含一个查询，该查询具有针对该用户`$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`的对象 ID 的工作分配。</span><span class="sxs-lookup"><span data-stu-id="64cf3-121">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID for of that user `$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>

<span data-ttu-id="64cf3-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="64cf3-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64cf3-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="64cf3-123">Request headers</span></span>

| <span data-ttu-id="64cf3-124">名称</span><span class="sxs-lookup"><span data-stu-id="64cf3-124">Name</span></span>      |<span data-ttu-id="64cf3-125">说明</span><span class="sxs-lookup"><span data-stu-id="64cf3-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64cf3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="64cf3-126">Authorization</span></span> | <span data-ttu-id="64cf3-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="64cf3-127">Bearer \{token\}.</span></span> <span data-ttu-id="64cf3-128">必需。</span><span class="sxs-lookup"><span data-stu-id="64cf3-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64cf3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="64cf3-129">Request body</span></span>

<span data-ttu-id="64cf3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64cf3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64cf3-131">响应</span><span class="sxs-lookup"><span data-stu-id="64cf3-131">Response</span></span>

<span data-ttu-id="64cf3-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignment](../resources/accesspackageassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="64cf3-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64cf3-133">示例</span><span class="sxs-lookup"><span data-stu-id="64cf3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64cf3-134">请求</span><span class="sxs-lookup"><span data-stu-id="64cf3-134">Request</span></span>

<span data-ttu-id="64cf3-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64cf3-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64cf3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cf3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64cf3-137">C#</span><span class="sxs-lookup"><span data-stu-id="64cf3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64cf3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64cf3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64cf3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64cf3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64cf3-140">响应</span><span class="sxs-lookup"><span data-stu-id="64cf3-140">Response</span></span>

<span data-ttu-id="64cf3-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64cf3-141">The following is an example of the response.</span></span>

> <span data-ttu-id="64cf3-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="64cf3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
