---
title: 创建日历
description: 此 API 可用于在用户的日历组中新建日历。
ms.openlocfilehash: 220922567eac421479803ad6dd0252a114701c9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043671"
---
# <a name="create-calendar"></a><span data-ttu-id="69746-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="69746-103">Create Calendar</span></span>

> <span data-ttu-id="69746-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69746-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69746-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69746-106">此 API 可用于在[用户](../resources/user.md)的日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="69746-106">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69746-107">权限</span><span class="sxs-lookup"><span data-stu-id="69746-107">Permissions</span></span>

<span data-ttu-id="69746-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69746-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69746-110">Permission type</span></span>                        | <span data-ttu-id="69746-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69746-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="69746-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69746-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="69746-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69746-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="69746-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69746-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69746-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69746-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="69746-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69746-116">Application</span></span>                            | <span data-ttu-id="69746-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69746-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="69746-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69746-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="69746-119">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="69746-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="69746-120">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="69746-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="69746-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="69746-121">Request headers</span></span>

| <span data-ttu-id="69746-122">标头</span><span class="sxs-lookup"><span data-stu-id="69746-122">Header</span></span>        | <span data-ttu-id="69746-123">值</span><span class="sxs-lookup"><span data-stu-id="69746-123">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="69746-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69746-124">Authorization</span></span> | <span data-ttu-id="69746-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69746-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="69746-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69746-127">Content-Type</span></span>  | <span data-ttu-id="69746-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="69746-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69746-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="69746-130">Request body</span></span>

<span data-ttu-id="69746-131">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69746-131">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="69746-132">响应</span><span class="sxs-lookup"><span data-stu-id="69746-132">Response</span></span>

<span data-ttu-id="69746-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69746-133">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69746-134">示例</span><span class="sxs-lookup"><span data-stu-id="69746-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69746-135">请求</span><span class="sxs-lookup"><span data-stu-id="69746-135">Request</span></span>

<span data-ttu-id="69746-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69746-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="69746-137">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69746-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="69746-138">响应</span><span class="sxs-lookup"><span data-stu-id="69746-138">Response</span></span>

<span data-ttu-id="69746-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69746-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
