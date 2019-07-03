---
title: 创建日历
description: 此 API 可用于在用户的日历组中新建日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 79ea80ff78cfb2320d6db17146a0d85f1cad5008
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438816"
---
# <a name="create-calendar"></a><span data-ttu-id="17f25-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="17f25-103">Create Calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17f25-104">此 API 可用于在[用户](../resources/user.md)的日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="17f25-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17f25-105">权限</span><span class="sxs-lookup"><span data-stu-id="17f25-105">Permissions</span></span>

<span data-ttu-id="17f25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17f25-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="17f25-108">Permission type</span></span>                        | <span data-ttu-id="17f25-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17f25-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="17f25-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17f25-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="17f25-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f25-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="17f25-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17f25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17f25-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f25-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="17f25-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="17f25-114">Application</span></span>                            | <span data-ttu-id="17f25-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17f25-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="17f25-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17f25-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="17f25-117">用户的默认 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="17f25-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="17f25-118">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="17f25-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="17f25-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17f25-119">Request headers</span></span>

| <span data-ttu-id="17f25-120">标头</span><span class="sxs-lookup"><span data-stu-id="17f25-120">Header</span></span>        | <span data-ttu-id="17f25-121">值</span><span class="sxs-lookup"><span data-stu-id="17f25-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="17f25-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17f25-122">Authorization</span></span> | <span data-ttu-id="17f25-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17f25-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="17f25-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17f25-125">Content-Type</span></span>  | <span data-ttu-id="17f25-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="17f25-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17f25-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="17f25-128">Request body</span></span>

<span data-ttu-id="17f25-129">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17f25-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="17f25-130">响应</span><span class="sxs-lookup"><span data-stu-id="17f25-130">Response</span></span>

<span data-ttu-id="17f25-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17f25-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f25-132">示例</span><span class="sxs-lookup"><span data-stu-id="17f25-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="17f25-133">请求</span><span class="sxs-lookup"><span data-stu-id="17f25-133">Request</span></span>

<span data-ttu-id="17f25-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17f25-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="17f25-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17f25-135">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17f25-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="17f25-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="17f25-137">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17f25-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="17f25-138">响应</span><span class="sxs-lookup"><span data-stu-id="17f25-138">Response</span></span>

<span data-ttu-id="17f25-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17f25-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
