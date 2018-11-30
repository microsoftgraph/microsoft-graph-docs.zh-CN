---
title: 删除事件
description: 删除事件。
ms.openlocfilehash: 6f9ee81f60fc3a45018cb137288bad7f22fb98a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011149"
---
# <a name="delete-event"></a><span data-ttu-id="7d20b-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="7d20b-103">Delete event</span></span>

<span data-ttu-id="7d20b-104">删除事件。</span><span class="sxs-lookup"><span data-stu-id="7d20b-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d20b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7d20b-105">Permissions</span></span>
<span data-ttu-id="7d20b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d20b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d20b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d20b-108">Permission type</span></span>      | <span data-ttu-id="7d20b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d20b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d20b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d20b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d20b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d20b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7d20b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d20b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d20b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d20b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7d20b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d20b-114">Application</span></span> | <span data-ttu-id="7d20b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d20b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d20b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d20b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7d20b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d20b-117">Request headers</span></span>
| <span data-ttu-id="7d20b-118">名称</span><span class="sxs-lookup"><span data-stu-id="7d20b-118">Name</span></span>       | <span data-ttu-id="7d20b-119">类型</span><span class="sxs-lookup"><span data-stu-id="7d20b-119">Type</span></span> | <span data-ttu-id="7d20b-120">说明</span><span class="sxs-lookup"><span data-stu-id="7d20b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d20b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d20b-121">Authorization</span></span>  | <span data-ttu-id="7d20b-122">string</span><span class="sxs-lookup"><span data-stu-id="7d20b-122">string</span></span>  | <span data-ttu-id="7d20b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d20b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d20b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d20b-125">Request body</span></span>
<span data-ttu-id="7d20b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d20b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d20b-127">响应</span><span class="sxs-lookup"><span data-stu-id="7d20b-127">Response</span></span>

<span data-ttu-id="7d20b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7d20b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d20b-130">示例</span><span class="sxs-lookup"><span data-stu-id="7d20b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d20b-131">请求</span><span class="sxs-lookup"><span data-stu-id="7d20b-131">Request</span></span>
<span data-ttu-id="7d20b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d20b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="7d20b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7d20b-133">Response</span></span>
<span data-ttu-id="7d20b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d20b-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
