---
title: 列出日历
description: 检索属于日历组的日历列表。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9ffa22a25fcc5c42ca9a61ea09a5cc68d2f3351b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814201"
---
# <a name="list-calendars"></a><span data-ttu-id="074ac-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="074ac-103">List calendars</span></span>

> <span data-ttu-id="074ac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="074ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="074ac-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="074ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="074ac-106">检索属于日历组的日历列表。</span><span class="sxs-lookup"><span data-stu-id="074ac-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="074ac-107">权限</span><span class="sxs-lookup"><span data-stu-id="074ac-107">Permissions</span></span>

<span data-ttu-id="074ac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="074ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="074ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="074ac-110">Permission type</span></span>                        | <span data-ttu-id="074ac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="074ac-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="074ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="074ac-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="074ac-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="074ac-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="074ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="074ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="074ac-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="074ac-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="074ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="074ac-116">Application</span></span>                            | <span data-ttu-id="074ac-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="074ac-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="074ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="074ac-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="074ac-119">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="074ac-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="074ac-120">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="074ac-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="074ac-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="074ac-121">Optional query parameters</span></span>

<span data-ttu-id="074ac-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="074ac-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="074ac-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="074ac-123">Request headers</span></span>

| <span data-ttu-id="074ac-124">名称</span><span class="sxs-lookup"><span data-stu-id="074ac-124">Name</span></span>          | <span data-ttu-id="074ac-125">类型</span><span class="sxs-lookup"><span data-stu-id="074ac-125">Type</span></span>   | <span data-ttu-id="074ac-126">说明</span><span class="sxs-lookup"><span data-stu-id="074ac-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="074ac-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="074ac-127">Authorization</span></span> | <span data-ttu-id="074ac-128">string</span><span class="sxs-lookup"><span data-stu-id="074ac-128">string</span></span> | <span data-ttu-id="074ac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="074ac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="074ac-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="074ac-131">Request body</span></span>

<span data-ttu-id="074ac-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="074ac-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="074ac-133">响应</span><span class="sxs-lookup"><span data-stu-id="074ac-133">Response</span></span>

<span data-ttu-id="074ac-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="074ac-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="074ac-135">示例</span><span class="sxs-lookup"><span data-stu-id="074ac-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="074ac-136">请求</span><span class="sxs-lookup"><span data-stu-id="074ac-136">Request</span></span>

<span data-ttu-id="074ac-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="074ac-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="074ac-138">响应</span><span class="sxs-lookup"><span data-stu-id="074ac-138">Response</span></span>

<span data-ttu-id="074ac-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="074ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
