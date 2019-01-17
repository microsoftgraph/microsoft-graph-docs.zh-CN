---
title: 创建事件
description: 使用此 API 新建事件。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 83d41f083a19ce813205dccc0056b2de16935541
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915177"
---
# <a name="create-event"></a><span data-ttu-id="c95aa-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="c95aa-103">Create event</span></span>

> <span data-ttu-id="c95aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c95aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c95aa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c95aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c95aa-106">使用此 API 新建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="c95aa-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c95aa-107">权限</span><span class="sxs-lookup"><span data-stu-id="c95aa-107">Permissions</span></span>
<span data-ttu-id="c95aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c95aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c95aa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c95aa-110">Permission type</span></span>      | <span data-ttu-id="c95aa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c95aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c95aa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c95aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c95aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c95aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c95aa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c95aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c95aa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c95aa-115">Not supported.</span></span>    |
|<span data-ttu-id="c95aa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c95aa-116">Application</span></span> | <span data-ttu-id="c95aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c95aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c95aa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c95aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="c95aa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c95aa-119">Request headers</span></span>
| <span data-ttu-id="c95aa-120">标头</span><span class="sxs-lookup"><span data-stu-id="c95aa-120">Header</span></span>       | <span data-ttu-id="c95aa-121">值</span><span class="sxs-lookup"><span data-stu-id="c95aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c95aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c95aa-122">Authorization</span></span>  | <span data-ttu-id="c95aa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c95aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c95aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c95aa-125">Request body</span></span>
<span data-ttu-id="c95aa-126">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c95aa-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c95aa-127">响应</span><span class="sxs-lookup"><span data-stu-id="c95aa-127">Response</span></span>
<span data-ttu-id="c95aa-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c95aa-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c95aa-129">示例</span><span class="sxs-lookup"><span data-stu-id="c95aa-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c95aa-130">请求</span><span class="sxs-lookup"><span data-stu-id="c95aa-130">Request</span></span>
<span data-ttu-id="c95aa-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c95aa-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="c95aa-132">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c95aa-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="c95aa-133">响应</span><span class="sxs-lookup"><span data-stu-id="c95aa-133">Response</span></span>
<span data-ttu-id="c95aa-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c95aa-134">The following is an example of the response.</span></span>
><span data-ttu-id="c95aa-135">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c95aa-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c95aa-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c95aa-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
