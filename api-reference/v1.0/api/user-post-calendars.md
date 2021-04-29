---
title: 创建日历
description: 此 API 可用于新建用户日历。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b19e7fdfb56518d26ba0dafd597838047ea21ae
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031499"
---
# <a name="create-calendar"></a><span data-ttu-id="4ed3f-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="4ed3f-103">Create Calendar</span></span>

<span data-ttu-id="4ed3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed3f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ed3f-105">此 API 可用于新建[用户](../resources/user.md)日历。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-105">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4ed3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ed3f-106">Permissions</span></span>
<span data-ttu-id="4ed3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ed3f-109">Permission type</span></span>      | <span data-ttu-id="4ed3f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ed3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ed3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ed3f-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ed3f-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ed3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ed3f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ed3f-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4ed3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ed3f-115">Application</span></span> | <span data-ttu-id="4ed3f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ed3f-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ed3f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ed3f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="4ed3f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ed3f-118">Request headers</span></span>
| <span data-ttu-id="4ed3f-119">标头</span><span class="sxs-lookup"><span data-stu-id="4ed3f-119">Header</span></span>       | <span data-ttu-id="4ed3f-120">值</span><span class="sxs-lookup"><span data-stu-id="4ed3f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ed3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ed3f-121">Authorization</span></span>  | <span data-ttu-id="4ed3f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ed3f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ed3f-124">Content-Type</span></span>  | <span data-ttu-id="4ed3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed3f-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ed3f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ed3f-126">Request body</span></span>
<span data-ttu-id="4ed3f-127">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-127">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4ed3f-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ed3f-128">Response</span></span>

<span data-ttu-id="4ed3f-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-129">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed3f-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ed3f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ed3f-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ed3f-131">Request</span></span>
<span data-ttu-id="4ed3f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ed3f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed3f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="4ed3f-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ed3f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ed3f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ed3f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ed3f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ed3f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ed3f-137">Java</span><span class="sxs-lookup"><span data-stu-id="4ed3f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4ed3f-138">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-138">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="4ed3f-139">响应</span><span class="sxs-lookup"><span data-stu-id="4ed3f-139">Response</span></span>
<span data-ttu-id="4ed3f-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-140">Here is an example of the response.</span></span> <span data-ttu-id="4ed3f-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ed3f-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "canEdit":true,
    "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

