---
title: 删除事件
description: 删除事件。
ms.openlocfilehash: cb62f1b7593f4fffe0416fd8c2f81917440e897a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046413"
---
# <a name="delete-event"></a><span data-ttu-id="fd0e2-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="fd0e2-103">Delete event</span></span>

> <span data-ttu-id="fd0e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd0e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd0e2-106">删除事件。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-106">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd0e2-107">权限</span><span class="sxs-lookup"><span data-stu-id="fd0e2-107">Permissions</span></span>
<span data-ttu-id="fd0e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd0e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd0e2-110">Permission type</span></span>      | <span data-ttu-id="fd0e2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd0e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd0e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd0e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd0e2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd0e2-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fd0e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd0e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd0e2-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd0e2-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fd0e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd0e2-116">Application</span></span> | <span data-ttu-id="fd0e2-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd0e2-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd0e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd0e2-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="fd0e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd0e2-119">Request headers</span></span>
| <span data-ttu-id="fd0e2-120">名称</span><span class="sxs-lookup"><span data-stu-id="fd0e2-120">Name</span></span>       | <span data-ttu-id="fd0e2-121">类型</span><span class="sxs-lookup"><span data-stu-id="fd0e2-121">Type</span></span> | <span data-ttu-id="fd0e2-122">说明</span><span class="sxs-lookup"><span data-stu-id="fd0e2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd0e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd0e2-123">Authorization</span></span>  | <span data-ttu-id="fd0e2-124">string</span><span class="sxs-lookup"><span data-stu-id="fd0e2-124">string</span></span>  | <span data-ttu-id="fd0e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd0e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd0e2-127">Request body</span></span>
<span data-ttu-id="fd0e2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd0e2-129">响应</span><span class="sxs-lookup"><span data-stu-id="fd0e2-129">Response</span></span>

<span data-ttu-id="fd0e2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd0e2-132">示例</span><span class="sxs-lookup"><span data-stu-id="fd0e2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd0e2-133">请求</span><span class="sxs-lookup"><span data-stu-id="fd0e2-133">Request</span></span>
<span data-ttu-id="fd0e2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="fd0e2-135">响应</span><span class="sxs-lookup"><span data-stu-id="fd0e2-135">Response</span></span>
<span data-ttu-id="fd0e2-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fd0e2-136">Here is an example of the response.</span></span> 
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
