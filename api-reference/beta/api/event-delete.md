---
title: 删除事件
description: 删除事件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 69efc9d1dd51e7d79b8e9daa319789b4a4d53706
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415765"
---
# <a name="delete-event"></a><span data-ttu-id="8996b-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="8996b-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8996b-104">删除事件。</span><span class="sxs-lookup"><span data-stu-id="8996b-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="8996b-105">权限</span><span class="sxs-lookup"><span data-stu-id="8996b-105">Permissions</span></span>
<span data-ttu-id="8996b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8996b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8996b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8996b-108">Permission type</span></span>      | <span data-ttu-id="8996b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8996b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8996b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8996b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8996b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8996b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8996b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8996b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8996b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8996b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8996b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8996b-114">Application</span></span> | <span data-ttu-id="8996b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8996b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8996b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8996b-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="8996b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8996b-117">Request headers</span></span>
| <span data-ttu-id="8996b-118">名称</span><span class="sxs-lookup"><span data-stu-id="8996b-118">Name</span></span>       | <span data-ttu-id="8996b-119">类型</span><span class="sxs-lookup"><span data-stu-id="8996b-119">Type</span></span> | <span data-ttu-id="8996b-120">说明</span><span class="sxs-lookup"><span data-stu-id="8996b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8996b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8996b-121">Authorization</span></span>  | <span data-ttu-id="8996b-122">string</span><span class="sxs-lookup"><span data-stu-id="8996b-122">string</span></span>  | <span data-ttu-id="8996b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8996b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8996b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8996b-125">Request body</span></span>
<span data-ttu-id="8996b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8996b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8996b-127">响应</span><span class="sxs-lookup"><span data-stu-id="8996b-127">Response</span></span>

<span data-ttu-id="8996b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8996b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8996b-130">示例</span><span class="sxs-lookup"><span data-stu-id="8996b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8996b-131">请求</span><span class="sxs-lookup"><span data-stu-id="8996b-131">Request</span></span>
<span data-ttu-id="8996b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8996b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8996b-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8996b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8996b-134">C#</span><span class="sxs-lookup"><span data-stu-id="8996b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8996b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8996b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8996b-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="8996b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8996b-137">响应</span><span class="sxs-lookup"><span data-stu-id="8996b-137">Response</span></span>
<span data-ttu-id="8996b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8996b-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
