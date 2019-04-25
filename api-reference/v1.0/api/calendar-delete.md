---
title: 删除日历
description: 删除默认日历以外的日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af1fe9a0b13aeb20a269b39bac8966bcc31508b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551370"
---
# <a name="delete-calendar"></a><span data-ttu-id="a9c11-103">删除日历</span><span class="sxs-lookup"><span data-stu-id="a9c11-103">Delete calendar</span></span>

<span data-ttu-id="a9c11-104">删除默认日历以外的日历。</span><span class="sxs-lookup"><span data-stu-id="a9c11-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9c11-105">权限</span><span class="sxs-lookup"><span data-stu-id="a9c11-105">Permissions</span></span>
<span data-ttu-id="a9c11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c11-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9c11-108">Permission type</span></span>      | <span data-ttu-id="a9c11-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9c11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9c11-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9c11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9c11-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9c11-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a9c11-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9c11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9c11-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9c11-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a9c11-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9c11-114">Application</span></span> | <span data-ttu-id="a9c11-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9c11-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9c11-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9c11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a9c11-117">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="a9c11-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="a9c11-118">指定 [calendarGroup](../resources/calendargroup.md) 中的 [日历](../resources/calendar.md)（非默认日历）。</span><span class="sxs-lookup"><span data-stu-id="a9c11-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9c11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9c11-119">Request headers</span></span>
| <span data-ttu-id="a9c11-120">名称</span><span class="sxs-lookup"><span data-stu-id="a9c11-120">Name</span></span>           |  <span data-ttu-id="a9c11-121">类型</span><span class="sxs-lookup"><span data-stu-id="a9c11-121">Type</span></span>    | <span data-ttu-id="a9c11-122">说明</span><span class="sxs-lookup"><span data-stu-id="a9c11-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="a9c11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9c11-123">Authorization</span></span>  |  <span data-ttu-id="a9c11-124">string</span><span class="sxs-lookup"><span data-stu-id="a9c11-124">string</span></span>  | <span data-ttu-id="a9c11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9c11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9c11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9c11-127">Request body</span></span>
<span data-ttu-id="a9c11-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9c11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9c11-129">响应</span><span class="sxs-lookup"><span data-stu-id="a9c11-129">Response</span></span>

<span data-ttu-id="a9c11-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9c11-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c11-132">示例</span><span class="sxs-lookup"><span data-stu-id="a9c11-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9c11-133">请求</span><span class="sxs-lookup"><span data-stu-id="a9c11-133">Request</span></span>
<span data-ttu-id="a9c11-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9c11-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="a9c11-135">响应</span><span class="sxs-lookup"><span data-stu-id="a9c11-135">Response</span></span>
<span data-ttu-id="a9c11-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9c11-136">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
