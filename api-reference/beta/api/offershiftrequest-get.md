---
title: 获取 offerShiftRequest
description: 检索 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1ae04f4e2cd97cca0ad0f7c7719c4f1b6d4b5c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456586"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="02f15-103">获取 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="02f15-103">Get offerShiftRequest</span></span>

<span data-ttu-id="02f15-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="02f15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02f15-105">检索[offerShiftRequest](../resources/offershiftrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02f15-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02f15-106">权限</span><span class="sxs-lookup"><span data-stu-id="02f15-106">Permissions</span></span>

<span data-ttu-id="02f15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02f15-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="02f15-109">Permission type</span></span>                        | <span data-ttu-id="02f15-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02f15-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02f15-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02f15-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="02f15-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f15-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="02f15-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02f15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02f15-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="02f15-114">Not supported.</span></span> |
| <span data-ttu-id="02f15-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="02f15-115">Application</span></span>                            | <span data-ttu-id="02f15-116">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="02f15-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="02f15-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="02f15-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="02f15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02f15-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02f15-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="02f15-119">Optional query parameters</span></span>

<span data-ttu-id="02f15-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="02f15-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="02f15-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="02f15-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02f15-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="02f15-122">Request headers</span></span>

| <span data-ttu-id="02f15-123">名称</span><span class="sxs-lookup"><span data-stu-id="02f15-123">Name</span></span>      |<span data-ttu-id="02f15-124">说明</span><span class="sxs-lookup"><span data-stu-id="02f15-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02f15-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f15-125">Authorization</span></span> | <span data-ttu-id="02f15-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02f15-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02f15-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="02f15-128">Request body</span></span>

<span data-ttu-id="02f15-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02f15-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02f15-130">响应</span><span class="sxs-lookup"><span data-stu-id="02f15-130">Response</span></span>

<span data-ttu-id="02f15-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="02f15-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02f15-132">示例</span><span class="sxs-lookup"><span data-stu-id="02f15-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02f15-133">请求</span><span class="sxs-lookup"><span data-stu-id="02f15-133">Request</span></span>

<span data-ttu-id="02f15-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02f15-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02f15-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="02f15-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="02f15-136">C#</span><span class="sxs-lookup"><span data-stu-id="02f15-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02f15-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02f15-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02f15-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02f15-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02f15-139">响应</span><span class="sxs-lookup"><span data-stu-id="02f15-139">Response</span></span>

<span data-ttu-id="02f15-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02f15-140">The following is an example of the response.</span></span>

> <span data-ttu-id="02f15-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="02f15-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
