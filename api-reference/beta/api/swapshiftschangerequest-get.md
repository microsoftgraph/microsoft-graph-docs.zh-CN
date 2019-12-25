---
title: 获取 swapShiftsChangeRequest
description: 检索 swapShiftsChangeRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e229fa0d85ab876a61cfff2958d3961f4b42637c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865047"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="457ea-103">获取 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="457ea-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="457ea-104">检索[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="457ea-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="457ea-105">权限</span><span class="sxs-lookup"><span data-stu-id="457ea-105">Permissions</span></span>

<span data-ttu-id="457ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="457ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="457ea-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="457ea-108">Permission type</span></span>                        | <span data-ttu-id="457ea-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="457ea-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="457ea-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="457ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="457ea-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="457ea-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="457ea-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="457ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="457ea-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="457ea-113">Not supported.</span></span> |
| <span data-ttu-id="457ea-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="457ea-114">Application</span></span>                            | <span data-ttu-id="457ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="457ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="457ea-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="457ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="457ea-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="457ea-117">Optional query parameters</span></span>

<span data-ttu-id="457ea-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="457ea-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="457ea-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="457ea-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="457ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="457ea-120">Request headers</span></span>

| <span data-ttu-id="457ea-121">名称</span><span class="sxs-lookup"><span data-stu-id="457ea-121">Name</span></span>      |<span data-ttu-id="457ea-122">说明</span><span class="sxs-lookup"><span data-stu-id="457ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="457ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="457ea-123">Authorization</span></span> | <span data-ttu-id="457ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="457ea-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="457ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="457ea-126">Request body</span></span>

<span data-ttu-id="457ea-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="457ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="457ea-128">响应</span><span class="sxs-lookup"><span data-stu-id="457ea-128">Response</span></span>

<span data-ttu-id="457ea-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="457ea-129">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="457ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="457ea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="457ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="457ea-131">Request</span></span>

<span data-ttu-id="457ea-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="457ea-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="457ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="457ea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="457ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="457ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="457ea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="457ea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="457ea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="457ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="457ea-137">响应</span><span class="sxs-lookup"><span data-stu-id="457ea-137">Response</span></span>

<span data-ttu-id="457ea-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="457ea-138">The following is an example of the response.</span></span>

> <span data-ttu-id="457ea-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="457ea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
