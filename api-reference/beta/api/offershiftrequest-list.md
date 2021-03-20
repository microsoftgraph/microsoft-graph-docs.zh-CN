---
title: 列出 offerShiftRequest
description: 检索团队中所有 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d38b668041bb94c3b61e589307aadfdb46e76de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946019"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="cebfb-103">列出 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="cebfb-103">List offerShiftRequest</span></span>

<span data-ttu-id="cebfb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cebfb-105">检索团队中 [所有 offerShiftRequest](../resources/offershiftrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cebfb-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebfb-106">权限</span><span class="sxs-lookup"><span data-stu-id="cebfb-106">Permissions</span></span>

<span data-ttu-id="cebfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cebfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cebfb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cebfb-109">Permission type</span></span>                        | <span data-ttu-id="cebfb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cebfb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cebfb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cebfb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cebfb-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebfb-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cebfb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cebfb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebfb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cebfb-114">Not supported.</span></span> |
| <span data-ttu-id="cebfb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cebfb-115">Application</span></span>                            | <span data-ttu-id="cebfb-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebfb-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebfb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cebfb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cebfb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cebfb-118">Optional query parameters</span></span>

<span data-ttu-id="cebfb-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cebfb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cebfb-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cebfb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cebfb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cebfb-121">Request headers</span></span>

| <span data-ttu-id="cebfb-122">名称</span><span class="sxs-lookup"><span data-stu-id="cebfb-122">Name</span></span>      |<span data-ttu-id="cebfb-123">说明</span><span class="sxs-lookup"><span data-stu-id="cebfb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cebfb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cebfb-124">Authorization</span></span> | <span data-ttu-id="cebfb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cebfb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cebfb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cebfb-127">Request body</span></span>

<span data-ttu-id="cebfb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cebfb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebfb-129">响应</span><span class="sxs-lookup"><span data-stu-id="cebfb-129">Response</span></span>

<span data-ttu-id="cebfb-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cebfb-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cebfb-131">示例</span><span class="sxs-lookup"><span data-stu-id="cebfb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cebfb-132">请求</span><span class="sxs-lookup"><span data-stu-id="cebfb-132">Request</span></span>

<span data-ttu-id="cebfb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cebfb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cebfb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cebfb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="cebfb-135">C#</span><span class="sxs-lookup"><span data-stu-id="cebfb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cebfb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cebfb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cebfb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cebfb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cebfb-138">Java</span><span class="sxs-lookup"><span data-stu-id="cebfb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cebfb-139">响应</span><span class="sxs-lookup"><span data-stu-id="cebfb-139">Response</span></span>

<span data-ttu-id="cebfb-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cebfb-140">The following is an example of the response.</span></span>

> <span data-ttu-id="cebfb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cebfb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


