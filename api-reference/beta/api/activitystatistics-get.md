---
title: 获取 activityStatistics
description: 为用户检索 activityStatistics 对象的属性。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: ebe19c4523ea9929ae77c9f4c408396f7b147b2c
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37723847"
---
# <a name="get-activitystatistics"></a><span data-ttu-id="ae7a2-103">获取 activityStatistics</span><span class="sxs-lookup"><span data-stu-id="ae7a2-103">Get activityStatistics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae7a2-104">获取用户的[activityStatistics](../resources/activitystatistics.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-104">Get the properties of an [activityStatistics](../resources/activitystatistics.md) object for a user.</span></span>

<span data-ttu-id="ae7a2-105">您可以获取指定用户和日期范围的[activityStatistics](../resources/activitystatistics.md)类型的属性。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-105">You can get the properties of a type of [activityStatistics](../resources/activitystatistics.md) for the specified user and date range.</span></span> <span data-ttu-id="ae7a2-106">您可以通过`id`在查询中使用支持的[活动 id 属性](../resources/activitystatistics.md#activity-id-property)的格式来指定统计信息和日期范围的类型。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-106">You can specify the type of statistics and date range by using the supported format of the [activity id property](../resources/activitystatistics.md#activity-id-property) for `id` in the query.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae7a2-107">权限</span><span class="sxs-lookup"><span data-stu-id="ae7a2-107">Permissions</span></span>

<span data-ttu-id="ae7a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae7a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae7a2-110">Permission type</span></span>                        | <span data-ttu-id="ae7a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae7a2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae7a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7a2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae7a2-113">Analytics.Read</span><span class="sxs-lookup"><span data-stu-id="ae7a2-113">Analytics.Read</span></span> |
| <span data-ttu-id="ae7a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-115">Not supported.</span></span> |
| <span data-ttu-id="ae7a2-116">Application</span><span class="sxs-lookup"><span data-stu-id="ae7a2-116">Application</span></span>                            | <span data-ttu-id="ae7a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae7a2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" }  -->

```http
GET /me/analytics/activitystatistics/{id}
GET /users/{id|userPrincipalName}/analytics/activitystatistics/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae7a2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae7a2-119">Optional query parameters</span></span>

<span data-ttu-id="ae7a2-120">此方法不支持用于自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-120">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae7a2-121">请求头</span><span class="sxs-lookup"><span data-stu-id="ae7a2-121">Request headers</span></span>

| <span data-ttu-id="ae7a2-122">名称</span><span class="sxs-lookup"><span data-stu-id="ae7a2-122">Name</span></span>      |<span data-ttu-id="ae7a2-123">说明</span><span class="sxs-lookup"><span data-stu-id="ae7a2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae7a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7a2-124">Authorization</span></span> | <span data-ttu-id="ae7a2-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ae7a2-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae7a2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae7a2-126">Request body</span></span>

<span data-ttu-id="ae7a2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae7a2-128">响应</span><span class="sxs-lookup"><span data-stu-id="ae7a2-128">Response</span></span>

<span data-ttu-id="ae7a2-129">如果成功，此方法将返回`200 OK`响应代码和请求的活动统计信息类型，这是从[activityStatistics](../resources/activitystatistics.md)中派生的以下资源之一： {[Call](../resources/callactivitystatistics.md)， [Chat](../resources/chatactivitystatistics.md)， [Email](../resources/emailactivitystatistics.md)， [Focus](../resources/focusactivitystatistics.md)，和[会议](../resources/meetingactivitystatistics.md)}。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-129">If successful, this method returns a `200 OK` response code and the requested type of activity statistics, which is one of the following resources derived from [activityStatistics](../resources/activitystatistics.md):{[Call](../resources/callactivitystatistics.md), [Chat](../resources/chatactivitystatistics.md), [Email](../resources/emailactivitystatistics.md), [Focus](../resources/focusactivitystatistics.md), and [Meeting](../resources/meetingactivitystatistics.md)}.</span></span>

## <a name="example"></a><span data-ttu-id="ae7a2-130">示例</span><span class="sxs-lookup"><span data-stu-id="ae7a2-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ae7a2-131">请求</span><span class="sxs-lookup"><span data-stu-id="ae7a2-131">Request</span></span>

<span data-ttu-id="ae7a2-132">下面的示例请求在2019-06-16 和2019-06-17 之间的日期范围内登录用户的类型 emailActivityStatistics 的统计信息。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-132">The following example requests statistics of the type emailActivityStatistics of the signed-in user, for the date range between 2019-06-16 and 2019-06-17.</span></span> <span data-ttu-id="ae7a2-133">有关常规 id 属性格式的详细信息，请参阅[activity id 属性](../resources/activitystatistics.md#activity-id-property)。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-133">For more information about the general id property format, see [activity id property](../resources/activitystatistics.md#activity-id-property).</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae7a2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae7a2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae7a2-135">C#</span><span class="sxs-lookup"><span data-stu-id="ae7a2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae7a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae7a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae7a2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae7a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae7a2-138">响应</span><span class="sxs-lookup"><span data-stu-id="ae7a2-138">Response</span></span>

<span data-ttu-id="ae7a2-139">下面的示例演示了一个响应，该响应获取特定活动和一天的已登录用户的活动统计信息。</span><span class="sxs-lookup"><span data-stu-id="ae7a2-139">The following is an example of the response that gets activity statistics of a signed-in user for a specific activity and day.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics/$entity",
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityStatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
