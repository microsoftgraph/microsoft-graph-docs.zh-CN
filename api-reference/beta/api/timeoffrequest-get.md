---
title: 获取 timeOffRequest
description: 检索 timeoffrequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 187dfaeeb6888c9717f6270166cbee61c6816082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953926"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="5068b-103">获取 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="5068b-103">Get timeOffRequest</span></span>

<span data-ttu-id="5068b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5068b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5068b-105">检索 [timeoffrequest 对象的属性和](../resources/timeoffrequest.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="5068b-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5068b-106">权限</span><span class="sxs-lookup"><span data-stu-id="5068b-106">Permissions</span></span>

<span data-ttu-id="5068b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5068b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5068b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5068b-109">Permission type</span></span>                        | <span data-ttu-id="5068b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5068b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5068b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5068b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5068b-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5068b-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5068b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5068b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5068b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5068b-114">Not supported.</span></span> |
|<span data-ttu-id="5068b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5068b-115">Application</span></span> | <span data-ttu-id="5068b-116">Schedule.Read.All *、Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="5068b-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="5068b-117">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="5068b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="5068b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5068b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5068b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5068b-119">Optional query parameters</span></span>

<span data-ttu-id="5068b-120">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5068b-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5068b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5068b-121">Request headers</span></span>

| <span data-ttu-id="5068b-122">名称</span><span class="sxs-lookup"><span data-stu-id="5068b-122">Name</span></span>      |<span data-ttu-id="5068b-123">说明</span><span class="sxs-lookup"><span data-stu-id="5068b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5068b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5068b-124">Authorization</span></span> | <span data-ttu-id="5068b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5068b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5068b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5068b-127">Request body</span></span>

<span data-ttu-id="5068b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5068b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5068b-129">响应</span><span class="sxs-lookup"><span data-stu-id="5068b-129">Response</span></span>

<span data-ttu-id="5068b-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5068b-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5068b-131">示例</span><span class="sxs-lookup"><span data-stu-id="5068b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5068b-132">请求</span><span class="sxs-lookup"><span data-stu-id="5068b-132">Request</span></span>

<span data-ttu-id="5068b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5068b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5068b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5068b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="5068b-135">C#</span><span class="sxs-lookup"><span data-stu-id="5068b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5068b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5068b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5068b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5068b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5068b-138">Java</span><span class="sxs-lookup"><span data-stu-id="5068b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5068b-139">响应</span><span class="sxs-lookup"><span data-stu-id="5068b-139">Response</span></span>

<span data-ttu-id="5068b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5068b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5068b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5068b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


