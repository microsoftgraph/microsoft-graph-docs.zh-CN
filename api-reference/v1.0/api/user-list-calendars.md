---
title: 列出日历
description: '获取用户的所有日历（`/calendars` 导航属性），从默认日历组或特定日历组中获取日历。 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 762a8ffeaacbc294587e88bf14290cc985c8b2d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925782"
---
# <a name="list-calendars"></a><span data-ttu-id="76657-103">列出日历</span><span class="sxs-lookup"><span data-stu-id="76657-103">List calendars</span></span>

<span data-ttu-id="76657-104">获取用户的所有日历（`/calendars` 导航属性），从默认日历组或特定日历组中获取日历。</span><span class="sxs-lookup"><span data-stu-id="76657-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="76657-105">权限</span><span class="sxs-lookup"><span data-stu-id="76657-105">Permissions</span></span>
<span data-ttu-id="76657-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76657-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="76657-108">Permission type</span></span>      | <span data-ttu-id="76657-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76657-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76657-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76657-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76657-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76657-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="76657-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76657-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76657-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76657-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="76657-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="76657-114">Application</span></span> | <span data-ttu-id="76657-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76657-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="76657-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76657-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="76657-117">用户的所有日历。</span><span class="sxs-lookup"><span data-stu-id="76657-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="76657-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="76657-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="76657-119">特定 [calendarGroup](../resources/calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="76657-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76657-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76657-120">Optional query parameters</span></span>
<span data-ttu-id="76657-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76657-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="76657-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="76657-122">Request headers</span></span>
| <span data-ttu-id="76657-123">标头</span><span class="sxs-lookup"><span data-stu-id="76657-123">Header</span></span>       | <span data-ttu-id="76657-124">值</span><span class="sxs-lookup"><span data-stu-id="76657-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76657-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="76657-125">Authorization</span></span>  | <span data-ttu-id="76657-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76657-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76657-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76657-128">Content-Type</span></span>   | <span data-ttu-id="76657-129">application/json</span><span class="sxs-lookup"><span data-stu-id="76657-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76657-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="76657-130">Request body</span></span>
<span data-ttu-id="76657-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76657-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76657-132">响应</span><span class="sxs-lookup"><span data-stu-id="76657-132">Response</span></span>

<span data-ttu-id="76657-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Calendar](../resources/calendar.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="76657-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76657-134">示例</span><span class="sxs-lookup"><span data-stu-id="76657-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76657-135">请求</span><span class="sxs-lookup"><span data-stu-id="76657-135">Request</span></span>
<span data-ttu-id="76657-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76657-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="76657-137">响应</span><span class="sxs-lookup"><span data-stu-id="76657-137">Response</span></span>
<span data-ttu-id="76657-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76657-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "canShare":true,
            "canViewPrivateItems":true,
            "canEdit":true,
            "owner":{
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
            }
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
