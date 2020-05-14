---
title: 获取 offerShiftRequest
description: 检索 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ffef189622621322fee15cdfc651531bd6a6d0c0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218227"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="9f9ab-103">获取 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="9f9ab-103">Get offerShiftRequest</span></span>

<span data-ttu-id="9f9ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f9ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f9ab-105">检索[offerShiftRequest](../resources/offershiftrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f9ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="9f9ab-106">Permissions</span></span>

<span data-ttu-id="9f9ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f9ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f9ab-109">Permission type</span></span>                        | <span data-ttu-id="9f9ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f9ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f9ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f9ab-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="9f9ab-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9f9ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f9ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-114">Not supported.</span></span> |
| <span data-ttu-id="9f9ab-115">Application</span><span class="sxs-lookup"><span data-stu-id="9f9ab-115">Application</span></span>                            | <span data-ttu-id="9f9ab-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="9f9ab-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="9f9ab-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9f9ab-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f9ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f9ab-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f9ab-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9f9ab-120">Optional query parameters</span></span>

<span data-ttu-id="9f9ab-121">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f9ab-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f9ab-122">Request headers</span></span>

| <span data-ttu-id="9f9ab-123">名称</span><span class="sxs-lookup"><span data-stu-id="9f9ab-123">Name</span></span>      |<span data-ttu-id="9f9ab-124">说明</span><span class="sxs-lookup"><span data-stu-id="9f9ab-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f9ab-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f9ab-125">Authorization</span></span> | <span data-ttu-id="9f9ab-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f9ab-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f9ab-128">Request body</span></span>

<span data-ttu-id="9f9ab-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f9ab-130">响应</span><span class="sxs-lookup"><span data-stu-id="9f9ab-130">Response</span></span>

<span data-ttu-id="9f9ab-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f9ab-132">示例</span><span class="sxs-lookup"><span data-stu-id="9f9ab-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f9ab-133">请求</span><span class="sxs-lookup"><span data-stu-id="9f9ab-133">Request</span></span>

<span data-ttu-id="9f9ab-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9f9ab-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f9ab-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="9f9ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="9f9ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f9ab-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f9ab-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f9ab-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f9ab-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f9ab-139">Java</span><span class="sxs-lookup"><span data-stu-id="9f9ab-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="9f9ab-140">响应</span><span class="sxs-lookup"><span data-stu-id="9f9ab-140">Response</span></span>

<span data-ttu-id="9f9ab-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-141">The following is an example of the response.</span></span>

> <span data-ttu-id="9f9ab-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9f9ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
