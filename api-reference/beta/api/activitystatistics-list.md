---
title: 列出 activityStatistics
description: 获取 activityStatistics 对象的集合。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 422d6b3d03129d2e1c7169f3131c46fadc457e35
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048307"
---
# <a name="list-activitystatistics"></a><span data-ttu-id="34037-103">列出 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="34037-103">List activityStatistics</span></span>

<span data-ttu-id="34037-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34037-105">获取用户 [最近一整周的 activityStatistics](../resources/activitystatistics.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="34037-105">Get a collection of [activityStatistics](../resources/activitystatistics.md) for a user, for the last complete week.</span></span>

## <a name="permissions"></a><span data-ttu-id="34037-106">权限</span><span class="sxs-lookup"><span data-stu-id="34037-106">Permissions</span></span>

<span data-ttu-id="34037-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34037-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="34037-109">Permission type</span></span>                        | <span data-ttu-id="34037-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="34037-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34037-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34037-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34037-112">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="34037-112">Analytics.Read</span></span> |
| <span data-ttu-id="34037-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34037-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34037-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="34037-114">Not supported.</span></span> |
| <span data-ttu-id="34037-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="34037-115">Application</span></span>                            | <span data-ttu-id="34037-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34037-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34037-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34037-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/analytics/activitystatistics
GET /users/{id|userPrincipalName}/analytics/activitystatistics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34037-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="34037-118">Optional query parameters</span></span>

<span data-ttu-id="34037-119">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="34037-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34037-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="34037-120">Request headers</span></span>

| <span data-ttu-id="34037-121">名称</span><span class="sxs-lookup"><span data-stu-id="34037-121">Name</span></span>      |<span data-ttu-id="34037-122">说明</span><span class="sxs-lookup"><span data-stu-id="34037-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34037-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34037-123">Authorization</span></span> | <span data-ttu-id="34037-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="34037-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="34037-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="34037-125">Request body</span></span>

<span data-ttu-id="34037-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="34037-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34037-127">响应</span><span class="sxs-lookup"><span data-stu-id="34037-127">Response</span></span>

<span data-ttu-id="34037-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [activityStatistics](../resources/activitystatistics.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="34037-128">If successful, this method returns a `200 OK` response code and a collection of [activityStatistics](../resources/activitystatistics.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34037-129">示例</span><span class="sxs-lookup"><span data-stu-id="34037-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="34037-130">请求</span><span class="sxs-lookup"><span data-stu-id="34037-130">Request</span></span>

<span data-ttu-id="34037-131">下面是一个请求已登录用户的所有相关活动统计信息的示例。</span><span class="sxs-lookup"><span data-stu-id="34037-131">The following is an example of a request of all related activity statistics for the signed-in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="34037-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="34037-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics

```
# <a name="c"></a>[<span data-ttu-id="34037-133">C#</span><span class="sxs-lookup"><span data-stu-id="34037-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34037-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34037-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34037-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34037-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34037-136">Java</span><span class="sxs-lookup"><span data-stu-id="34037-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitystatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="34037-137">响应</span><span class="sxs-lookup"><span data-stu-id="34037-137">Response</span></span>

<span data-ttu-id="34037-138">下面是一个响应示例，该响应具有用户的所有相关活动统计信息。</span><span class="sxs-lookup"><span data-stu-id="34037-138">The following is an example of a response with all related activity statistics for a user.</span></span> <span data-ttu-id="34037-139">此响应只显示一周活动的第一天，以缩短其可读性。</span><span class="sxs-lookup"><span data-stu-id="34037-139">This response only shows the first day of a week's activities to shorten it for readability.</span></span>

> <span data-ttu-id="34037-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="34037-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


