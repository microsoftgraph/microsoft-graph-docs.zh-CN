---
title: 列出 activityStatistics
description: 获取 activityStatistics 对象的集合。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 97bf2cee1f7297fceef895a9b2df1acb3192a226
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719197"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="487d0-103">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="487d0-103">List activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="487d0-104">在最后一个完整的星期获取用户的[activityStatistics](../resources/activitystatistics.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="487d0-104">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="487d0-105">权限</span><span class="sxs-lookup"><span data-stu-id="487d0-105">Permissions</span></span>

<span data-ttu-id="487d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="487d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="487d0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="487d0-108">Permission type</span></span>                        | <span data-ttu-id="487d0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="487d0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="487d0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="487d0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="487d0-111">分析。读取</span><span class="sxs-lookup"><span data-stu-id="487d0-111">Analytics.Read</span></span> |
| <span data-ttu-id="487d0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="487d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="487d0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="487d0-113">Not supported.</span></span> |
| <span data-ttu-id="487d0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="487d0-114">Application</span></span>                            | <span data-ttu-id="487d0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="487d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="487d0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="487d0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET  https://graph.microsoft.com/beta/me/analytics/activitystatistics 
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="487d0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="487d0-117">Optional query parameters</span></span>

<span data-ttu-id="487d0-118">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="487d0-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="487d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="487d0-119">Request headers</span></span>

| <span data-ttu-id="487d0-120">名称</span><span class="sxs-lookup"><span data-stu-id="487d0-120">Name</span></span>      |<span data-ttu-id="487d0-121">说明</span><span class="sxs-lookup"><span data-stu-id="487d0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="487d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="487d0-122">Authorization</span></span> | <span data-ttu-id="487d0-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="487d0-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="487d0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="487d0-124">Request body</span></span>

<span data-ttu-id="487d0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="487d0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="487d0-126">响应</span><span class="sxs-lookup"><span data-stu-id="487d0-126">Response</span></span>

<span data-ttu-id="487d0-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[activityStatistics](../resources/activitystatistics.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="487d0-127">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="487d0-128">示例</span><span class="sxs-lookup"><span data-stu-id="487d0-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="487d0-129">请求</span><span class="sxs-lookup"><span data-stu-id="487d0-129">Request</span></span>

<span data-ttu-id="487d0-130">以下是已登录用户的所有相关活动统计信息的请求示例。</span><span class="sxs-lookup"><span data-stu-id="487d0-130">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="487d0-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="487d0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="487d0-132">C#</span><span class="sxs-lookup"><span data-stu-id="487d0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="487d0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="487d0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="487d0-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="487d0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="487d0-135">响应</span><span class="sxs-lookup"><span data-stu-id="487d0-135">Response</span></span>

<span data-ttu-id="487d0-136">以下是用户的所有相关活动统计信息响应的示例。</span><span class="sxs-lookup"><span data-stu-id="487d0-136">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="487d0-137">此响应仅显示一周的活动的第一天, 以缩短可读性。</span><span class="sxs-lookup"><span data-stu-id="487d0-137">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="487d0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="487d0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics",
    "value": [
        {
            "@odata.type": "#microsoft.graph.emailActivityStatistics",
            "activity": "Email",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "email_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S",
            "readEmail": "PT0S",
            "sentEmail": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.meetingActivityStatistics",
            "activity": "Meeting",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "meeting_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S",
            "organized": "PT0S",
            "recurring": "PT0S",
            "long": "PT0S",
            "conflicting": "PT0S",
            "multitasking": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.focusActivityStatistics",
            "activity": "Focus",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "focus_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.chatActivityStatistics",
            "activity": "Chat",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "chat_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        },
        {
            "@odata.type": "#microsoft.graph.callActivityStatistics",
            "activity": "Call",
            "startDate": "2019-06-16",
            "endDate": "2019-06-17",
            "id": "call_2019-06-16_2019-06-17",
            "timeZoneUsed": "Pacific Standard Time",
            "duration": "PT0S",
            "afterHours": "PT0S"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List activitystatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
