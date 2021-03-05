---
title: 创建日历
description: 此 API 可用于在用户的日历组中新建日历。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3573c4ebc1df251706f4fc3b11f66ce4445374d7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432959"
---
# <a name="create-calendar"></a><span data-ttu-id="8f8ca-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="8f8ca-103">Create Calendar</span></span>

<span data-ttu-id="8f8ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f8ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f8ca-105">此 API 可用于在[用户](../resources/user.md)的日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-105">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f8ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f8ca-106">Permissions</span></span>

<span data-ttu-id="8f8ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f8ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f8ca-109">Permission type</span></span>                        | <span data-ttu-id="8f8ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f8ca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8f8ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f8ca-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f8ca-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="8f8ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f8ca-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f8ca-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="8f8ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f8ca-115">Application</span></span>                            | <span data-ttu-id="8f8ca-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f8ca-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f8ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f8ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8f8ca-118">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="8f8ca-119">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="8f8ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f8ca-120">Request headers</span></span>

| <span data-ttu-id="8f8ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="8f8ca-121">Header</span></span>        | <span data-ttu-id="8f8ca-122">值</span><span class="sxs-lookup"><span data-stu-id="8f8ca-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="8f8ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f8ca-123">Authorization</span></span> | <span data-ttu-id="8f8ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8f8ca-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f8ca-126">Content-Type</span></span>  | <span data-ttu-id="8f8ca-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8f8ca-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f8ca-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f8ca-129">Request body</span></span>

<span data-ttu-id="8f8ca-130">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8f8ca-131">响应</span><span class="sxs-lookup"><span data-stu-id="8f8ca-131">Response</span></span>

<span data-ttu-id="8f8ca-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-132">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f8ca-133">示例</span><span class="sxs-lookup"><span data-stu-id="8f8ca-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f8ca-134">请求</span><span class="sxs-lookup"><span data-stu-id="8f8ca-134">Request</span></span>

<span data-ttu-id="8f8ca-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f8ca-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f8ca-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars
Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascript"></a>[<span data-ttu-id="8f8ca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f8ca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8f8ca-138">C#</span><span class="sxs-lookup"><span data-stu-id="8f8ca-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f8ca-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f8ca-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f8ca-140">Java</span><span class="sxs-lookup"><span data-stu-id="8f8ca-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8f8ca-141">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-141">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8f8ca-142">响应</span><span class="sxs-lookup"><span data-stu-id="8f8ca-142">Response</span></span>

<span data-ttu-id="8f8ca-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f8ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
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

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

