---
title: 获取 timeOffRequest
description: 检索 timeoffrequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f80a9d3ad66b7621cd3fecbf9fae6380568fbee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981333"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="bab5e-103">获取 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="bab5e-103">Get timeOffRequest</span></span>

<span data-ttu-id="bab5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab5e-105">检索 [timeoffrequest](../resources/timeoffrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bab5e-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="bab5e-106">Permissions</span></span>

<span data-ttu-id="bab5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bab5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bab5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bab5e-109">Permission type</span></span>                        | <span data-ttu-id="bab5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bab5e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bab5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bab5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bab5e-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab5e-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bab5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bab5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab5e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bab5e-114">Not supported.</span></span> |
|<span data-ttu-id="bab5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bab5e-115">Application</span></span> | <span data-ttu-id="bab5e-116">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="bab5e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="bab5e-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="bab5e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="bab5e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bab5e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab5e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bab5e-119">Optional query parameters</span></span>

<span data-ttu-id="bab5e-120">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bab5e-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab5e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bab5e-121">Request headers</span></span>

| <span data-ttu-id="bab5e-122">名称</span><span class="sxs-lookup"><span data-stu-id="bab5e-122">Name</span></span>      |<span data-ttu-id="bab5e-123">说明</span><span class="sxs-lookup"><span data-stu-id="bab5e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bab5e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab5e-124">Authorization</span></span> | <span data-ttu-id="bab5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bab5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bab5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bab5e-127">Request body</span></span>

<span data-ttu-id="bab5e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bab5e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab5e-129">响应</span><span class="sxs-lookup"><span data-stu-id="bab5e-129">Response</span></span>

<span data-ttu-id="bab5e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bab5e-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bab5e-131">示例</span><span class="sxs-lookup"><span data-stu-id="bab5e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bab5e-132">请求</span><span class="sxs-lookup"><span data-stu-id="bab5e-132">Request</span></span>

<span data-ttu-id="bab5e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bab5e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bab5e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bab5e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="bab5e-135">C#</span><span class="sxs-lookup"><span data-stu-id="bab5e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bab5e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bab5e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bab5e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bab5e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bab5e-138">Java</span><span class="sxs-lookup"><span data-stu-id="bab5e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bab5e-139">响应</span><span class="sxs-lookup"><span data-stu-id="bab5e-139">Response</span></span>

<span data-ttu-id="bab5e-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bab5e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="bab5e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bab5e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


