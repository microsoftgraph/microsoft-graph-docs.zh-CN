---
title: 创建日历
description: 此 API 可用于在用户的日历组中新建日历。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f0f3fac9b9dcccb41ebea46b689080cfce879f4f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047698"
---
# <a name="create-calendar"></a><span data-ttu-id="c0cb5-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="c0cb5-103">Create Calendar</span></span>

<span data-ttu-id="c0cb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0cb5-105">此 API 可用于在[用户](../resources/user.md)的日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-105">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0cb5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c0cb5-106">Permissions</span></span>

<span data-ttu-id="c0cb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0cb5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0cb5-109">Permission type</span></span>                        | <span data-ttu-id="c0cb5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0cb5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c0cb5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0cb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0cb5-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0cb5-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="c0cb5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0cb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0cb5-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0cb5-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="c0cb5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0cb5-115">Application</span></span>                            | <span data-ttu-id="c0cb5-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0cb5-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c0cb5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0cb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c0cb5-118">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="c0cb5-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="c0cb5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0cb5-120">Request headers</span></span>

| <span data-ttu-id="c0cb5-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0cb5-121">Header</span></span>        | <span data-ttu-id="c0cb5-122">值</span><span class="sxs-lookup"><span data-stu-id="c0cb5-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="c0cb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0cb5-123">Authorization</span></span> | <span data-ttu-id="c0cb5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c0cb5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0cb5-126">Content-Type</span></span>  | <span data-ttu-id="c0cb5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c0cb5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0cb5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0cb5-129">Request body</span></span>

<span data-ttu-id="c0cb5-130">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0cb5-131">响应</span><span class="sxs-lookup"><span data-stu-id="c0cb5-131">Response</span></span>

<span data-ttu-id="c0cb5-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-132">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0cb5-133">示例</span><span class="sxs-lookup"><span data-stu-id="c0cb5-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0cb5-134">请求</span><span class="sxs-lookup"><span data-stu-id="c0cb5-134">Request</span></span>

<span data-ttu-id="c0cb5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0cb5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0cb5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars
Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascript"></a>[<span data-ttu-id="c0cb5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0cb5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c0cb5-138">C#</span><span class="sxs-lookup"><span data-stu-id="c0cb5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0cb5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0cb5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0cb5-140">Java</span><span class="sxs-lookup"><span data-stu-id="c0cb5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c0cb5-141">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-141">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c0cb5-142">响应</span><span class="sxs-lookup"><span data-stu-id="c0cb5-142">Response</span></span>

<span data-ttu-id="c0cb5-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-143">Here is an example of the response.</span></span> <span data-ttu-id="c0cb5-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0cb5-144">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


