---
title: 创建日历
description: 此 API 可用于新建用户日历。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 867641a47ca02e903c22a3338a0fe87f7c70bddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887820"
---
# <a name="create-calendar"></a><span data-ttu-id="ebe23-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="ebe23-103">Create Calendar</span></span>

> <span data-ttu-id="ebe23-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ebe23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebe23-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ebe23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebe23-106">此 API 可用于新建[用户](../resources/user.md)日历。</span><span class="sxs-lookup"><span data-stu-id="ebe23-106">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ebe23-107">权限</span><span class="sxs-lookup"><span data-stu-id="ebe23-107">Permissions</span></span>
<span data-ttu-id="ebe23-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebe23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebe23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebe23-110">Permission type</span></span>      | <span data-ttu-id="ebe23-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebe23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebe23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebe23-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebe23-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ebe23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebe23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe23-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebe23-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ebe23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebe23-116">Application</span></span> | <span data-ttu-id="ebe23-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebe23-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebe23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebe23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="ebe23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebe23-119">Request headers</span></span>
| <span data-ttu-id="ebe23-120">标头</span><span class="sxs-lookup"><span data-stu-id="ebe23-120">Header</span></span>       | <span data-ttu-id="ebe23-121">值</span><span class="sxs-lookup"><span data-stu-id="ebe23-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebe23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebe23-122">Authorization</span></span>  | <span data-ttu-id="ebe23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebe23-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ebe23-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebe23-125">Content-Type</span></span>  | <span data-ttu-id="ebe23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebe23-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebe23-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebe23-127">Request body</span></span>
<span data-ttu-id="ebe23-128">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebe23-128">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ebe23-129">响应</span><span class="sxs-lookup"><span data-stu-id="ebe23-129">Response</span></span>

<span data-ttu-id="ebe23-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebe23-130">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebe23-131">示例</span><span class="sxs-lookup"><span data-stu-id="ebe23-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebe23-132">请求</span><span class="sxs-lookup"><span data-stu-id="ebe23-132">Request</span></span>
<span data-ttu-id="ebe23-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebe23-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
<span data-ttu-id="ebe23-134">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebe23-134">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ebe23-135">响应</span><span class="sxs-lookup"><span data-stu-id="ebe23-135">Response</span></span>
<span data-ttu-id="ebe23-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebe23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
  "tocPath": ""
}-->
