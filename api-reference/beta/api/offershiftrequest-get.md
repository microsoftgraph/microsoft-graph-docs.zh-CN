---
title: 获取 offerShiftRequest
description: 检索 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 89b4c6db5c1898b64d72f7ba9cdaeb45ea3b10ef
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313749"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="22a63-103">获取 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="22a63-103">Get offerShiftRequest</span></span>

<span data-ttu-id="22a63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a63-105">检索 [offerShiftRequest](../resources/offershiftrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22a63-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22a63-106">权限</span><span class="sxs-lookup"><span data-stu-id="22a63-106">Permissions</span></span>

<span data-ttu-id="22a63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22a63-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22a63-109">Permission type</span></span>                        | <span data-ttu-id="22a63-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22a63-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22a63-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22a63-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22a63-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="22a63-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="22a63-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22a63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22a63-114">Not supported.</span></span> |
| <span data-ttu-id="22a63-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22a63-115">Application</span></span>                            | <span data-ttu-id="22a63-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="22a63-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22a63-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22a63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22a63-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22a63-118">Optional query parameters</span></span>

<span data-ttu-id="22a63-119">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22a63-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22a63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22a63-120">Request headers</span></span>

| <span data-ttu-id="22a63-121">名称</span><span class="sxs-lookup"><span data-stu-id="22a63-121">Name</span></span>      |<span data-ttu-id="22a63-122">说明</span><span class="sxs-lookup"><span data-stu-id="22a63-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22a63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a63-123">Authorization</span></span> | <span data-ttu-id="22a63-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22a63-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22a63-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="22a63-126">Request body</span></span>

<span data-ttu-id="22a63-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22a63-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a63-128">响应</span><span class="sxs-lookup"><span data-stu-id="22a63-128">Response</span></span>

<span data-ttu-id="22a63-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22a63-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22a63-130">示例</span><span class="sxs-lookup"><span data-stu-id="22a63-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22a63-131">请求</span><span class="sxs-lookup"><span data-stu-id="22a63-131">Request</span></span>

<span data-ttu-id="22a63-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22a63-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22a63-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22a63-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="22a63-134">C#</span><span class="sxs-lookup"><span data-stu-id="22a63-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22a63-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22a63-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22a63-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22a63-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22a63-137">响应</span><span class="sxs-lookup"><span data-stu-id="22a63-137">Response</span></span>

<span data-ttu-id="22a63-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22a63-138">The following is an example of the response.</span></span>

> <span data-ttu-id="22a63-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22a63-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


