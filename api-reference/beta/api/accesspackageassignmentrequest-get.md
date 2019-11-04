---
title: 获取 accessPackageAssignmentRequest
description: 检索 accessPackageAssignmentRequest 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5768664edbdce00b8004ee9031520fdcc9331ef3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935248"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="05cbe-103">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="05cbe-103">Get accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05cbe-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="05cbe-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="05cbe-105">权限</span><span class="sxs-lookup"><span data-stu-id="05cbe-105">Permissions</span></span>

<span data-ttu-id="05cbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05cbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05cbe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="05cbe-108">Permission type</span></span>                        | <span data-ttu-id="05cbe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05cbe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05cbe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05cbe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="05cbe-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="05cbe-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="05cbe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05cbe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05cbe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="05cbe-113">Not supported.</span></span> |
| <span data-ttu-id="05cbe-114">Application</span><span class="sxs-lookup"><span data-stu-id="05cbe-114">Application</span></span>                            | <span data-ttu-id="05cbe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="05cbe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05cbe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05cbe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05cbe-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="05cbe-117">Optional query parameters</span></span>

<span data-ttu-id="05cbe-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="05cbe-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="05cbe-119">例如，若要检索请求的访问包，请在查询`$expand=accessPackage`中包含。</span><span class="sxs-lookup"><span data-stu-id="05cbe-119">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="05cbe-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="05cbe-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="05cbe-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="05cbe-121">Request headers</span></span>

| <span data-ttu-id="05cbe-122">名称</span><span class="sxs-lookup"><span data-stu-id="05cbe-122">Name</span></span>      |<span data-ttu-id="05cbe-123">说明</span><span class="sxs-lookup"><span data-stu-id="05cbe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05cbe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05cbe-124">Authorization</span></span> | <span data-ttu-id="05cbe-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="05cbe-125">Bearer \{token\}.</span></span> <span data-ttu-id="05cbe-126">必填。</span><span class="sxs-lookup"><span data-stu-id="05cbe-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05cbe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05cbe-127">Request body</span></span>

<span data-ttu-id="05cbe-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05cbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05cbe-129">响应</span><span class="sxs-lookup"><span data-stu-id="05cbe-129">Response</span></span>

<span data-ttu-id="05cbe-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="05cbe-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05cbe-131">示例</span><span class="sxs-lookup"><span data-stu-id="05cbe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05cbe-132">请求</span><span class="sxs-lookup"><span data-stu-id="05cbe-132">Request</span></span>

<span data-ttu-id="05cbe-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05cbe-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

### <a name="response"></a><span data-ttu-id="05cbe-134">响应</span><span class="sxs-lookup"><span data-stu-id="05cbe-134">Response</span></span>

<span data-ttu-id="05cbe-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05cbe-135">The following is an example of the response.</span></span>

> <span data-ttu-id="05cbe-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05cbe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
