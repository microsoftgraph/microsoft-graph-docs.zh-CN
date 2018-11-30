---
title: 创建日历
description: 此 API 可用于新建用户日历。
ms.openlocfilehash: 8ffa88331478d7bbbe1e94c87d58505041d63d41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011129"
---
# <a name="create-calendar"></a><span data-ttu-id="ae917-103">创建日历</span><span class="sxs-lookup"><span data-stu-id="ae917-103">Create Calendar</span></span>

<span data-ttu-id="ae917-104">此 API 可用于新建[用户](../resources/user.md)日历。</span><span class="sxs-lookup"><span data-stu-id="ae917-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ae917-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae917-105">Permissions</span></span>
<span data-ttu-id="ae917-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae917-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae917-108">Permission type</span></span>      | <span data-ttu-id="ae917-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae917-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae917-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae917-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae917-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae917-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ae917-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae917-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae917-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae917-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ae917-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae917-114">Application</span></span> | <span data-ttu-id="ae917-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae917-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae917-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae917-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="ae917-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae917-117">Request headers</span></span>
| <span data-ttu-id="ae917-118">标头</span><span class="sxs-lookup"><span data-stu-id="ae917-118">Header</span></span>       | <span data-ttu-id="ae917-119">值</span><span class="sxs-lookup"><span data-stu-id="ae917-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae917-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae917-120">Authorization</span></span>  | <span data-ttu-id="ae917-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae917-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae917-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae917-123">Content-Type</span></span>  | <span data-ttu-id="ae917-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ae917-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae917-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae917-125">Request body</span></span>
<span data-ttu-id="ae917-126">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae917-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae917-127">响应</span><span class="sxs-lookup"><span data-stu-id="ae917-127">Response</span></span>

<span data-ttu-id="ae917-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae917-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae917-129">示例</span><span class="sxs-lookup"><span data-stu-id="ae917-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae917-130">请求</span><span class="sxs-lookup"><span data-stu-id="ae917-130">Request</span></span>
<span data-ttu-id="ae917-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae917-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="ae917-132">在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae917-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae917-133">响应</span><span class="sxs-lookup"><span data-stu-id="ae917-133">Response</span></span>
<span data-ttu-id="ae917-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae917-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
