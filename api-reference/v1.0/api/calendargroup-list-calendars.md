---
title: 列出日历
description: 检索属于日历组的日历列表。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f4fc5997e3ec93e757137822742c281e39b506a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264699"
---
# <a name="list-calendars"></a><span data-ttu-id="6af26-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="6af26-103">List calendars</span></span>

<span data-ttu-id="6af26-104">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="6af26-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af26-105">权限</span><span class="sxs-lookup"><span data-stu-id="6af26-105">Permissions</span></span>

<span data-ttu-id="6af26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6af26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6af26-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6af26-108">Permission type</span></span>                        | <span data-ttu-id="6af26-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6af26-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6af26-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6af26-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6af26-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af26-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="6af26-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6af26-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af26-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af26-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="6af26-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6af26-114">Application</span></span>                            | <span data-ttu-id="6af26-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af26-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="6af26-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6af26-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6af26-117">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="6af26-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="6af26-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="6af26-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6af26-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6af26-119">Optional query parameters</span></span>

<span data-ttu-id="6af26-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6af26-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6af26-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6af26-121">Request headers</span></span>

| <span data-ttu-id="6af26-122">名称</span><span class="sxs-lookup"><span data-stu-id="6af26-122">Name</span></span>          | <span data-ttu-id="6af26-123">类型</span><span class="sxs-lookup"><span data-stu-id="6af26-123">Type</span></span>   | <span data-ttu-id="6af26-124">说明</span><span class="sxs-lookup"><span data-stu-id="6af26-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="6af26-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6af26-125">Authorization</span></span> | <span data-ttu-id="6af26-126">string</span><span class="sxs-lookup"><span data-stu-id="6af26-126">string</span></span> | <span data-ttu-id="6af26-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6af26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6af26-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6af26-129">Request body</span></span>

<span data-ttu-id="6af26-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6af26-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af26-131">响应</span><span class="sxs-lookup"><span data-stu-id="6af26-131">Response</span></span>

<span data-ttu-id="6af26-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6af26-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af26-133">示例</span><span class="sxs-lookup"><span data-stu-id="6af26-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6af26-134">请求</span><span class="sxs-lookup"><span data-stu-id="6af26-134">Request</span></span>

<span data-ttu-id="6af26-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6af26-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="6af26-136">响应</span><span class="sxs-lookup"><span data-stu-id="6af26-136">Response</span></span>

<span data-ttu-id="6af26-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6af26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6af26-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6af26-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6af26-141">C#</span><span class="sxs-lookup"><span data-stu-id="6af26-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendars-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6af26-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="6af26-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendars-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6af26-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="6af26-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendars-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendargroup-list-calendars.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
