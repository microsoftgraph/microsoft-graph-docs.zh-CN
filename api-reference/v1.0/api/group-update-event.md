---
title: 更新事件
description: 更新 event 对象。
author: dkershaw10
ms.openlocfilehash: c8aacc7df62bf336c355801e89e1b6bea5c2b1f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321159"
---
# <a name="update-event"></a><span data-ttu-id="cd9fa-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="cd9fa-103">Update event</span></span>
<span data-ttu-id="cd9fa-104">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd9fa-105">权限</span><span class="sxs-lookup"><span data-stu-id="cd9fa-105">Permissions</span></span>
<span data-ttu-id="cd9fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd9fa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd9fa-108">Permission type</span></span>      | <span data-ttu-id="cd9fa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd9fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd9fa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd9fa-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9fa-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd9fa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd9fa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-113">Not supported.</span></span>    |
|<span data-ttu-id="cd9fa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd9fa-114">Application</span></span> | <span data-ttu-id="cd9fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd9fa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd9fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd9fa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd9fa-117">Request headers</span></span>
| <span data-ttu-id="cd9fa-118">Name</span><span class="sxs-lookup"><span data-stu-id="cd9fa-118">Name</span></span>       | <span data-ttu-id="cd9fa-119">类型</span><span class="sxs-lookup"><span data-stu-id="cd9fa-119">Type</span></span> | <span data-ttu-id="cd9fa-120">说明</span><span class="sxs-lookup"><span data-stu-id="cd9fa-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd9fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9fa-121">Authorization</span></span>  | <span data-ttu-id="cd9fa-122">string</span><span class="sxs-lookup"><span data-stu-id="cd9fa-122">string</span></span>  | <span data-ttu-id="cd9fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd9fa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd9fa-125">Request body</span></span>
<span data-ttu-id="cd9fa-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="cd9fa-129">响应</span><span class="sxs-lookup"><span data-stu-id="cd9fa-129">Response</span></span>
<span data-ttu-id="cd9fa-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd9fa-131">示例</span><span class="sxs-lookup"><span data-stu-id="cd9fa-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cd9fa-132">请求</span><span class="sxs-lookup"><span data-stu-id="cd9fa-132">Request</span></span>
<span data-ttu-id="cd9fa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-133">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="cd9fa-134">响应</span><span class="sxs-lookup"><span data-stu-id="cd9fa-134">Response</span></span>
<span data-ttu-id="cd9fa-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cd9fa-135">The following is an example of the response.</span></span>

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