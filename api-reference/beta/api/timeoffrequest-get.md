---
title: 获取 timeOffRequest
description: 检索 timeoffrequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2f8cfce33bd0945cd06c573d9182ed49b943640a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863556"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="33996-103">获取 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="33996-103">Get timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33996-104">检索[timeoffrequest](../resources/timeoffrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33996-104">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33996-105">权限</span><span class="sxs-lookup"><span data-stu-id="33996-105">Permissions</span></span>

<span data-ttu-id="33996-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33996-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="33996-108">Permission type</span></span>                        | <span data-ttu-id="33996-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33996-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="33996-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33996-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="33996-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33996-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="33996-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33996-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33996-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="33996-113">Not supported.</span></span> |
|<span data-ttu-id="33996-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="33996-114">Application</span></span> | <span data-ttu-id="33996-115">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="33996-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="33996-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="33996-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="33996-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33996-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33996-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="33996-118">Optional query parameters</span></span>

<span data-ttu-id="33996-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="33996-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="33996-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="33996-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="33996-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="33996-121">Request headers</span></span>

| <span data-ttu-id="33996-122">名称</span><span class="sxs-lookup"><span data-stu-id="33996-122">Name</span></span>      |<span data-ttu-id="33996-123">说明</span><span class="sxs-lookup"><span data-stu-id="33996-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33996-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33996-124">Authorization</span></span> | <span data-ttu-id="33996-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33996-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33996-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="33996-127">Request body</span></span>

<span data-ttu-id="33996-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33996-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33996-129">响应</span><span class="sxs-lookup"><span data-stu-id="33996-129">Response</span></span>

<span data-ttu-id="33996-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="33996-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33996-131">示例</span><span class="sxs-lookup"><span data-stu-id="33996-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33996-132">请求</span><span class="sxs-lookup"><span data-stu-id="33996-132">Request</span></span>

<span data-ttu-id="33996-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33996-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33996-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="33996-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33996-135">C#</span><span class="sxs-lookup"><span data-stu-id="33996-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33996-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33996-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33996-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33996-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="33996-138">响应</span><span class="sxs-lookup"><span data-stu-id="33996-138">Response</span></span>

<span data-ttu-id="33996-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="33996-139">The following is an example of the response.</span></span>

> <span data-ttu-id="33996-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33996-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
