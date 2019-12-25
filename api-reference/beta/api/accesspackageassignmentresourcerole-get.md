---
title: 获取 accessPackageAssignmentResourceRole
description: 检索 accessPackageAssignmentResourceRole 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a3d7cc1beaaadaf37da83045b9ab270022f8e32e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871751"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="c04f2-103">获取 accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="c04f2-103">Get accessPackageAssignmentResourceRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c04f2-104">检索[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c04f2-104">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c04f2-105">权限</span><span class="sxs-lookup"><span data-stu-id="c04f2-105">Permissions</span></span>

<span data-ttu-id="c04f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c04f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c04f2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c04f2-108">Permission type</span></span>                        | <span data-ttu-id="c04f2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c04f2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c04f2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c04f2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c04f2-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c04f2-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="c04f2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c04f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c04f2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c04f2-113">Not supported.</span></span> |
| <span data-ttu-id="c04f2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c04f2-114">Application</span></span>                            | <span data-ttu-id="c04f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c04f2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c04f2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c04f2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c04f2-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="c04f2-117">Optional query parameters</span></span>

<span data-ttu-id="c04f2-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c04f2-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c04f2-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c04f2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c04f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c04f2-120">Request headers</span></span>

| <span data-ttu-id="c04f2-121">名称</span><span class="sxs-lookup"><span data-stu-id="c04f2-121">Name</span></span>      |<span data-ttu-id="c04f2-122">说明</span><span class="sxs-lookup"><span data-stu-id="c04f2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c04f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c04f2-123">Authorization</span></span> | <span data-ttu-id="c04f2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c04f2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c04f2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c04f2-126">Request body</span></span>

<span data-ttu-id="c04f2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c04f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c04f2-128">响应</span><span class="sxs-lookup"><span data-stu-id="c04f2-128">Response</span></span>

<span data-ttu-id="c04f2-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c04f2-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c04f2-130">示例</span><span class="sxs-lookup"><span data-stu-id="c04f2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c04f2-131">请求</span><span class="sxs-lookup"><span data-stu-id="c04f2-131">Request</span></span>

<span data-ttu-id="c04f2-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c04f2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

### <a name="response"></a><span data-ttu-id="c04f2-133">响应</span><span class="sxs-lookup"><span data-stu-id="c04f2-133">Response</span></span>

<span data-ttu-id="c04f2-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c04f2-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c04f2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c04f2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
