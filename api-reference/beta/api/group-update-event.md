---
title: 更新事件
description: 更新 event 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4edf9011db83fa3fa47e52749fa8cc5aa630d035
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592484"
---
# <a name="update-event"></a><span data-ttu-id="c1331-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="c1331-103">Update event</span></span>
<span data-ttu-id="c1331-104">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1331-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1331-105">权限</span><span class="sxs-lookup"><span data-stu-id="c1331-105">Permissions</span></span>
<span data-ttu-id="c1331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1331-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1331-108">Permission type</span></span>      | <span data-ttu-id="c1331-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1331-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1331-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1331-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1331-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1331-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1331-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1331-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1331-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1331-113">Not supported.</span></span>    |
|<span data-ttu-id="c1331-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1331-114">Application</span></span> | <span data-ttu-id="c1331-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1331-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1331-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1331-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c1331-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1331-117">Request headers</span></span>
| <span data-ttu-id="c1331-118">名称</span><span class="sxs-lookup"><span data-stu-id="c1331-118">Name</span></span>       | <span data-ttu-id="c1331-119">类型</span><span class="sxs-lookup"><span data-stu-id="c1331-119">Type</span></span> | <span data-ttu-id="c1331-120">说明</span><span class="sxs-lookup"><span data-stu-id="c1331-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1331-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1331-121">Authorization</span></span>  | <span data-ttu-id="c1331-122">string</span><span class="sxs-lookup"><span data-stu-id="c1331-122">string</span></span>  | <span data-ttu-id="c1331-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1331-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1331-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1331-125">Request body</span></span>
<span data-ttu-id="c1331-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c1331-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="c1331-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1331-129">Response</span></span>
<span data-ttu-id="c1331-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c1331-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c1331-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1331-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c1331-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1331-132">Request</span></span>
<span data-ttu-id="c1331-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1331-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="c1331-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1331-134">Response</span></span>
<span data-ttu-id="c1331-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1331-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1331-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c1331-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c1331-137">语言</span><span class="sxs-lookup"><span data-stu-id="c1331-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1331-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1331-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update-event.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
