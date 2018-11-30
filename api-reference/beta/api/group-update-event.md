---
title: 更新事件
description: 更新 event 对象。
ms.openlocfilehash: 94dfa35e4b37e4e38746223604d3d3b3c7311a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045636"
---
# <a name="update-event"></a><span data-ttu-id="14737-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="14737-103">Update event</span></span>

> <span data-ttu-id="14737-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14737-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14737-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14737-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14737-106">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14737-106">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14737-107">权限</span><span class="sxs-lookup"><span data-stu-id="14737-107">Permissions</span></span>
<span data-ttu-id="14737-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14737-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14737-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14737-110">Permission type</span></span>      | <span data-ttu-id="14737-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14737-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14737-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14737-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14737-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14737-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14737-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14737-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14737-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14737-115">Not supported.</span></span>    |
|<span data-ttu-id="14737-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14737-116">Application</span></span> | <span data-ttu-id="14737-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14737-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14737-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14737-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14737-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14737-119">Request headers</span></span>
| <span data-ttu-id="14737-120">名称</span><span class="sxs-lookup"><span data-stu-id="14737-120">Name</span></span>       | <span data-ttu-id="14737-121">类型</span><span class="sxs-lookup"><span data-stu-id="14737-121">Type</span></span> | <span data-ttu-id="14737-122">说明</span><span class="sxs-lookup"><span data-stu-id="14737-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14737-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14737-123">Authorization</span></span>  | <span data-ttu-id="14737-124">string</span><span class="sxs-lookup"><span data-stu-id="14737-124">string</span></span>  | <span data-ttu-id="14737-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14737-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14737-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14737-127">Request body</span></span>
<span data-ttu-id="14737-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="14737-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="14737-131">响应</span><span class="sxs-lookup"><span data-stu-id="14737-131">Response</span></span>
<span data-ttu-id="14737-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="14737-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14737-133">示例</span><span class="sxs-lookup"><span data-stu-id="14737-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="14737-134">请求</span><span class="sxs-lookup"><span data-stu-id="14737-134">Request</span></span>
<span data-ttu-id="14737-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14737-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="14737-136">响应</span><span class="sxs-lookup"><span data-stu-id="14737-136">Response</span></span>
<span data-ttu-id="14737-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14737-137">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->