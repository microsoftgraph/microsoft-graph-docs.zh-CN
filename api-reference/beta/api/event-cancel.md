---
title: 事件： 取消
description: '此操作允许组织者的会议发送取消邮件和取消事件。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e39066c3360113965b0009473e520557853ba284
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530151"
---
# <a name="event-cancel"></a><span data-ttu-id="ed233-103">事件： 取消</span><span class="sxs-lookup"><span data-stu-id="ed233-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed233-104">此操作允许组织者的会议发送取消邮件和取消事件。</span><span class="sxs-lookup"><span data-stu-id="ed233-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="ed233-105">操作将事件移到已删除邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="ed233-105">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="ed233-106">组织者还可以取消的定期会议通过提供出现事件 id。</span><span class="sxs-lookup"><span data-stu-id="ed233-106">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="ed233-107">调用此操作与会者获取错误 （HTTP 400 错误请求），与以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="ed233-107">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="ed233-108">"无法完成您的请求。</span><span class="sxs-lookup"><span data-stu-id="ed233-108">"Your request can't be completed.</span></span> <span data-ttu-id="ed233-109">您需要取消会议组织者。"</span><span class="sxs-lookup"><span data-stu-id="ed233-109">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="ed233-110">此操作与[删除](event-delete.md)区别在于**取消**可供仅组织者，并允许组织者向取消有关与会者发送自定义消息。</span><span class="sxs-lookup"><span data-stu-id="ed233-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed233-111">权限</span><span class="sxs-lookup"><span data-stu-id="ed233-111">Permissions</span></span>
<span data-ttu-id="ed233-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed233-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed233-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed233-114">Permission type</span></span>      | <span data-ttu-id="ed233-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed233-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed233-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed233-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ed233-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed233-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ed233-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed233-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed233-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed233-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ed233-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed233-120">Application</span></span> | <span data-ttu-id="ed233-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed233-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed233-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed233-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="ed233-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed233-123">Request headers</span></span>
| <span data-ttu-id="ed233-124">名称</span><span class="sxs-lookup"><span data-stu-id="ed233-124">Name</span></span>       | <span data-ttu-id="ed233-125">类型</span><span class="sxs-lookup"><span data-stu-id="ed233-125">Type</span></span> | <span data-ttu-id="ed233-126">说明</span><span class="sxs-lookup"><span data-stu-id="ed233-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed233-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed233-127">Authorization</span></span>  | <span data-ttu-id="ed233-128">string</span><span class="sxs-lookup"><span data-stu-id="ed233-128">string</span></span>  | <span data-ttu-id="ed233-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed233-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed233-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed233-131">Content-Type</span></span> | <span data-ttu-id="ed233-132">string</span><span class="sxs-lookup"><span data-stu-id="ed233-132">string</span></span>  | <span data-ttu-id="ed233-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="ed233-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed233-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed233-135">Request body</span></span>
<span data-ttu-id="ed233-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ed233-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ed233-137">参数</span><span class="sxs-lookup"><span data-stu-id="ed233-137">Parameter</span></span>    | <span data-ttu-id="ed233-138">类型</span><span class="sxs-lookup"><span data-stu-id="ed233-138">Type</span></span>   |<span data-ttu-id="ed233-139">说明</span><span class="sxs-lookup"><span data-stu-id="ed233-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed233-140">注释</span><span class="sxs-lookup"><span data-stu-id="ed233-140">comment</span></span>|<span data-ttu-id="ed233-141">String</span><span class="sxs-lookup"><span data-stu-id="ed233-141">String</span></span>|<span data-ttu-id="ed233-142">有关取消发送给所有与会者的注释。</span><span class="sxs-lookup"><span data-stu-id="ed233-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="ed233-143">可选。</span><span class="sxs-lookup"><span data-stu-id="ed233-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="ed233-144">响应</span><span class="sxs-lookup"><span data-stu-id="ed233-144">Response</span></span>

<span data-ttu-id="ed233-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ed233-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed233-147">示例</span><span class="sxs-lookup"><span data-stu-id="ed233-147">Example</span></span>
<span data-ttu-id="ed233-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ed233-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed233-149">请求</span><span class="sxs-lookup"><span data-stu-id="ed233-149">Request</span></span>
<span data-ttu-id="ed233-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed233-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```

##### <a name="response"></a><span data-ttu-id="ed233-151">响应</span><span class="sxs-lookup"><span data-stu-id="ed233-151">Response</span></span>
<span data-ttu-id="ed233-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed233-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
