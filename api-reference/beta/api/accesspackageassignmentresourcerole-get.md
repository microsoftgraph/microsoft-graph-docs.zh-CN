---
title: 获取 accessPackageAssignmentResourceRole
description: 检索 accessPackageAssignmentResourceRole 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae44a167d7e89ac659e816e5ebe90d1995b5258b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442004"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="cdbaa-103">获取 accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="cdbaa-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="cdbaa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cdbaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdbaa-105">检索[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdbaa-106">权限</span><span class="sxs-lookup"><span data-stu-id="cdbaa-106">Permissions</span></span>

<span data-ttu-id="cdbaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdbaa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdbaa-109">Permission type</span></span>                        | <span data-ttu-id="cdbaa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdbaa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cdbaa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbaa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdbaa-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbaa-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="cdbaa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdbaa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-114">Not supported.</span></span> |
| <span data-ttu-id="cdbaa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdbaa-115">Application</span></span>                            | <span data-ttu-id="cdbaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdbaa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdbaa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdbaa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cdbaa-118">Optional query parameters</span></span>

<span data-ttu-id="cdbaa-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cdbaa-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdbaa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdbaa-121">Request headers</span></span>

| <span data-ttu-id="cdbaa-122">名称</span><span class="sxs-lookup"><span data-stu-id="cdbaa-122">Name</span></span>      |<span data-ttu-id="cdbaa-123">说明</span><span class="sxs-lookup"><span data-stu-id="cdbaa-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cdbaa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdbaa-124">Authorization</span></span> | <span data-ttu-id="cdbaa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdbaa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdbaa-127">Request body</span></span>

<span data-ttu-id="cdbaa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdbaa-129">响应</span><span class="sxs-lookup"><span data-stu-id="cdbaa-129">Response</span></span>

<span data-ttu-id="cdbaa-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdbaa-131">示例</span><span class="sxs-lookup"><span data-stu-id="cdbaa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdbaa-132">请求</span><span class="sxs-lookup"><span data-stu-id="cdbaa-132">Request</span></span>

<span data-ttu-id="cdbaa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdbaa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdbaa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="cdbaa-135">C#</span><span class="sxs-lookup"><span data-stu-id="cdbaa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdbaa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdbaa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdbaa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdbaa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdbaa-138">响应</span><span class="sxs-lookup"><span data-stu-id="cdbaa-138">Response</span></span>

<span data-ttu-id="cdbaa-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-139">The following is an example of the response.</span></span>

> <span data-ttu-id="cdbaa-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdbaa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
  "originId": "originId-value",
  "originSystem": "SharePointOnline",
  "status": "Fulfilled"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentResourceRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
