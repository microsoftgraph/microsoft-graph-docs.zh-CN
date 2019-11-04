---
title: 列出 accessPackageAssignmentResourceRoles
description: 检索 accessPackageAssignmentResourceRrole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16d2e91b00832b4745682861573985cc5bde27fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935240"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="54a11-103">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="54a11-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54a11-104">检索[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="54a11-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="54a11-105">生成的列表包含呼叫者有权读取的所有目录和访问包中的所有工作分配的所有资源角色。</span><span class="sxs-lookup"><span data-stu-id="54a11-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="54a11-106">权限</span><span class="sxs-lookup"><span data-stu-id="54a11-106">Permissions</span></span>

<span data-ttu-id="54a11-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54a11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54a11-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54a11-109">Permission type</span></span>                        | <span data-ttu-id="54a11-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54a11-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54a11-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54a11-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="54a11-112">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="54a11-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="54a11-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54a11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54a11-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="54a11-114">Not supported.</span></span> |
| <span data-ttu-id="54a11-115">Application</span><span class="sxs-lookup"><span data-stu-id="54a11-115">Application</span></span>                            | <span data-ttu-id="54a11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="54a11-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54a11-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54a11-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54a11-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54a11-118">Optional query parameters</span></span>

<span data-ttu-id="54a11-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54a11-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="54a11-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="54a11-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="54a11-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54a11-121">Request headers</span></span>

| <span data-ttu-id="54a11-122">名称</span><span class="sxs-lookup"><span data-stu-id="54a11-122">Name</span></span>      |<span data-ttu-id="54a11-123">说明</span><span class="sxs-lookup"><span data-stu-id="54a11-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54a11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54a11-124">Authorization</span></span> | <span data-ttu-id="54a11-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="54a11-125">Bearer \{token\}.</span></span> <span data-ttu-id="54a11-126">必填。</span><span class="sxs-lookup"><span data-stu-id="54a11-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54a11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54a11-127">Request body</span></span>

<span data-ttu-id="54a11-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54a11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54a11-129">响应</span><span class="sxs-lookup"><span data-stu-id="54a11-129">Response</span></span>

<span data-ttu-id="54a11-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="54a11-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54a11-131">示例</span><span class="sxs-lookup"><span data-stu-id="54a11-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54a11-132">请求</span><span class="sxs-lookup"><span data-stu-id="54a11-132">Request</span></span>

<span data-ttu-id="54a11-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="54a11-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

### <a name="response"></a><span data-ttu-id="54a11-134">响应</span><span class="sxs-lookup"><span data-stu-id="54a11-134">Response</span></span>

<span data-ttu-id="54a11-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="54a11-135">The following is an example of the response.</span></span>

> <span data-ttu-id="54a11-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="54a11-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
