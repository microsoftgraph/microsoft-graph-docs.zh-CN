---
title: 创建日历
description: 此 API 可用于新建用户日历。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2e9f4984f45795494fdbc5f6eaddcac23be6ed05
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346364"
---
# <a name="create-calendar"></a><span data-ttu-id="00b13-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="00b13-103">Create Calendar</span></span>

<span data-ttu-id="00b13-104">此 API 可用于新建[用户](../resources/user.md)日历。</span><span class="sxs-lookup"><span data-stu-id="00b13-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="00b13-105">权限</span><span class="sxs-lookup"><span data-stu-id="00b13-105">Permissions</span></span>
<span data-ttu-id="00b13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00b13-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="00b13-108">Permission type</span></span>      | <span data-ttu-id="00b13-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00b13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00b13-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00b13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00b13-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00b13-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="00b13-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00b13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00b13-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00b13-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="00b13-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="00b13-114">Application</span></span> | <span data-ttu-id="00b13-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00b13-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00b13-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00b13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="00b13-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00b13-117">Request headers</span></span>
| <span data-ttu-id="00b13-118">标头</span><span class="sxs-lookup"><span data-stu-id="00b13-118">Header</span></span>       | <span data-ttu-id="00b13-119">值</span><span class="sxs-lookup"><span data-stu-id="00b13-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00b13-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00b13-120">Authorization</span></span>  | <span data-ttu-id="00b13-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00b13-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00b13-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00b13-123">Content-Type</span></span>  | <span data-ttu-id="00b13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00b13-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00b13-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="00b13-125">Request body</span></span>
<span data-ttu-id="00b13-126">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b13-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00b13-127">响应</span><span class="sxs-lookup"><span data-stu-id="00b13-127">Response</span></span>

<span data-ttu-id="00b13-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00b13-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00b13-129">示例</span><span class="sxs-lookup"><span data-stu-id="00b13-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00b13-130">请求</span><span class="sxs-lookup"><span data-stu-id="00b13-130">Request</span></span>
<span data-ttu-id="00b13-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00b13-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00b13-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="00b13-132">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="00b13-133">C#</span><span class="sxs-lookup"><span data-stu-id="00b13-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00b13-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00b13-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00b13-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00b13-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00b13-136">Java</span><span class="sxs-lookup"><span data-stu-id="00b13-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="00b13-137">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b13-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00b13-138">响应</span><span class="sxs-lookup"><span data-stu-id="00b13-138">Response</span></span>
<span data-ttu-id="00b13-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00b13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
