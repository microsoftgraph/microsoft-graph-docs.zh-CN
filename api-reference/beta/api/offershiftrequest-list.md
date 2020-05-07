---
title: 列出 offerShiftRequest
description: 检索团队中所有 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 411363d06a677c6b211d85e058766923a136a505
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44153539"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="72bc6-103">列出 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="72bc6-103">List offerShiftRequest</span></span>

<span data-ttu-id="72bc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72bc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72bc6-105">检索团队中所有[offerShiftRequest](../resources/offershiftrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72bc6-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="72bc6-106">权限</span><span class="sxs-lookup"><span data-stu-id="72bc6-106">Permissions</span></span>

<span data-ttu-id="72bc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72bc6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72bc6-109">Permission type</span></span>                        | <span data-ttu-id="72bc6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72bc6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72bc6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72bc6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72bc6-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bc6-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="72bc6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72bc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bc6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72bc6-114">Not supported.</span></span> |
| <span data-ttu-id="72bc6-115">Application</span><span class="sxs-lookup"><span data-stu-id="72bc6-115">Application</span></span>                            | <span data-ttu-id="72bc6-116">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="72bc6-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="72bc6-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="72bc6-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="72bc6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72bc6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72bc6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72bc6-119">Optional query parameters</span></span>

<span data-ttu-id="72bc6-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72bc6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="72bc6-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="72bc6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72bc6-122">请求头</span><span class="sxs-lookup"><span data-stu-id="72bc6-122">Request headers</span></span>

| <span data-ttu-id="72bc6-123">名称</span><span class="sxs-lookup"><span data-stu-id="72bc6-123">Name</span></span>      |<span data-ttu-id="72bc6-124">说明</span><span class="sxs-lookup"><span data-stu-id="72bc6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72bc6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72bc6-125">Authorization</span></span> | <span data-ttu-id="72bc6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72bc6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72bc6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="72bc6-128">Request body</span></span>

<span data-ttu-id="72bc6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72bc6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72bc6-130">响应</span><span class="sxs-lookup"><span data-stu-id="72bc6-130">Response</span></span>

<span data-ttu-id="72bc6-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="72bc6-131">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72bc6-132">示例</span><span class="sxs-lookup"><span data-stu-id="72bc6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72bc6-133">请求</span><span class="sxs-lookup"><span data-stu-id="72bc6-133">Request</span></span>

<span data-ttu-id="72bc6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72bc6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72bc6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bc6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="72bc6-136">C#</span><span class="sxs-lookup"><span data-stu-id="72bc6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72bc6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bc6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72bc6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bc6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72bc6-139">响应</span><span class="sxs-lookup"><span data-stu-id="72bc6-139">Response</span></span>

<span data-ttu-id="72bc6-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72bc6-140">The following is an example of the response.</span></span>

> <span data-ttu-id="72bc6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72bc6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
