---
title: 获取 offerShiftRequest
description: 检索 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8b02d3bb5a9a228c2fa6f53c3243fc5bcc7de5a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050414"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="d59f6-103">获取 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="d59f6-103">Get offerShiftRequest</span></span>

<span data-ttu-id="d59f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d59f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d59f6-105">检索 [offerShiftRequest 对象的属性和](../resources/offershiftrequest.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d59f6-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d59f6-106">权限</span><span class="sxs-lookup"><span data-stu-id="d59f6-106">Permissions</span></span>

<span data-ttu-id="d59f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d59f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d59f6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d59f6-109">Permission type</span></span>                        | <span data-ttu-id="d59f6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d59f6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d59f6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d59f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d59f6-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d59f6-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d59f6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d59f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d59f6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d59f6-114">Not supported.</span></span> |
| <span data-ttu-id="d59f6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d59f6-115">Application</span></span>                            | <span data-ttu-id="d59f6-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d59f6-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d59f6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d59f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d59f6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d59f6-118">Optional query parameters</span></span>

<span data-ttu-id="d59f6-119">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d59f6-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d59f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d59f6-120">Request headers</span></span>

| <span data-ttu-id="d59f6-121">名称</span><span class="sxs-lookup"><span data-stu-id="d59f6-121">Name</span></span>      |<span data-ttu-id="d59f6-122">说明</span><span class="sxs-lookup"><span data-stu-id="d59f6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d59f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d59f6-123">Authorization</span></span> | <span data-ttu-id="d59f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d59f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d59f6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d59f6-126">Request body</span></span>

<span data-ttu-id="d59f6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d59f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d59f6-128">响应</span><span class="sxs-lookup"><span data-stu-id="d59f6-128">Response</span></span>

<span data-ttu-id="d59f6-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d59f6-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d59f6-130">示例</span><span class="sxs-lookup"><span data-stu-id="d59f6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d59f6-131">请求</span><span class="sxs-lookup"><span data-stu-id="d59f6-131">Request</span></span>

<span data-ttu-id="d59f6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d59f6-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d59f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d59f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="d59f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="d59f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d59f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d59f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d59f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d59f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d59f6-137">Java</span><span class="sxs-lookup"><span data-stu-id="d59f6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d59f6-138">响应</span><span class="sxs-lookup"><span data-stu-id="d59f6-138">Response</span></span>

<span data-ttu-id="d59f6-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d59f6-139">The following is an example of the response.</span></span>

> <span data-ttu-id="d59f6-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d59f6-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

