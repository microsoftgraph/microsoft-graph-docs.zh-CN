---
title: 列出 activityStatistics
description: 获取 activityStatistics 对象的集合。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0b6c499bf86041e3f071977370e898b1471c3755
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441786"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="86f6b-103">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="86f6b-103">List activityStatistics</span></span>

<span data-ttu-id="86f6b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="86f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86f6b-105">在最后一个完整的星期获取用户的[activityStatistics](../resources/activitystatistics.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="86f6b-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="86f6b-106">权限</span><span class="sxs-lookup"><span data-stu-id="86f6b-106">Permissions</span></span>

<span data-ttu-id="86f6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86f6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86f6b-109">Permission type</span></span>                        | <span data-ttu-id="86f6b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86f6b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86f6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86f6b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86f6b-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="86f6b-112">Analytics.Read</span></span> |
| <span data-ttu-id="86f6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86f6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86f6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86f6b-114">Not supported.</span></span> |
| <span data-ttu-id="86f6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86f6b-115">Application</span></span>                            | <span data-ttu-id="86f6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86f6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86f6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86f6b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86f6b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86f6b-118">Optional query parameters</span></span>

<span data-ttu-id="86f6b-119">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="86f6b-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86f6b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86f6b-120">Request headers</span></span>

| <span data-ttu-id="86f6b-121">名称</span><span class="sxs-lookup"><span data-stu-id="86f6b-121">Name</span></span>      |<span data-ttu-id="86f6b-122">说明</span><span class="sxs-lookup"><span data-stu-id="86f6b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86f6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86f6b-123">Authorization</span></span> | <span data-ttu-id="86f6b-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="86f6b-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86f6b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="86f6b-125">Request body</span></span>

<span data-ttu-id="86f6b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86f6b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86f6b-127">响应</span><span class="sxs-lookup"><span data-stu-id="86f6b-127">Response</span></span>

<span data-ttu-id="86f6b-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[activityStatistics](../resources/activitystatistics.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="86f6b-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86f6b-129">示例</span><span class="sxs-lookup"><span data-stu-id="86f6b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="86f6b-130">请求</span><span class="sxs-lookup"><span data-stu-id="86f6b-130">Request</span></span>

<span data-ttu-id="86f6b-131">以下是已登录用户的所有相关活动统计信息的请求示例。</span><span class="sxs-lookup"><span data-stu-id="86f6b-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="86f6b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="86f6b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="86f6b-133">C#</span><span class="sxs-lookup"><span data-stu-id="86f6b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86f6b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86f6b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86f6b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86f6b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86f6b-136">响应</span><span class="sxs-lookup"><span data-stu-id="86f6b-136">Response</span></span>

<span data-ttu-id="86f6b-137">以下是用户的所有相关活动统计信息响应的示例。</span><span class="sxs-lookup"><span data-stu-id="86f6b-137">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="86f6b-138">此响应仅显示一周的活动的第一天，以缩短可读性。</span><span class="sxs-lookup"><span data-stu-id="86f6b-138">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="86f6b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86f6b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
