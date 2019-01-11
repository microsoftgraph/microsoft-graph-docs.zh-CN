---
title: 创建事件
description: 使用此 API 新建事件。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4b7e0803b6eb59a2446da658815c19d08256587b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883907"
---
# <a name="create-event"></a><span data-ttu-id="ca68c-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="ca68c-103">Create event</span></span>

> <span data-ttu-id="ca68c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca68c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca68c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca68c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca68c-106">使用此 API 新建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="ca68c-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca68c-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca68c-107">Permissions</span></span>
<span data-ttu-id="ca68c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca68c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca68c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca68c-110">Permission type</span></span>      | <span data-ttu-id="ca68c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca68c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca68c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca68c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca68c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca68c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca68c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca68c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca68c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca68c-115">Not supported.</span></span>    |
|<span data-ttu-id="ca68c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca68c-116">Application</span></span> | <span data-ttu-id="ca68c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca68c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca68c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca68c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="ca68c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca68c-119">Request headers</span></span>
| <span data-ttu-id="ca68c-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca68c-120">Header</span></span>       | <span data-ttu-id="ca68c-121">值</span><span class="sxs-lookup"><span data-stu-id="ca68c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca68c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca68c-122">Authorization</span></span>  | <span data-ttu-id="ca68c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca68c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca68c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca68c-125">Request body</span></span>
<span data-ttu-id="ca68c-126">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca68c-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca68c-127">响应</span><span class="sxs-lookup"><span data-stu-id="ca68c-127">Response</span></span>
<span data-ttu-id="ca68c-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca68c-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca68c-129">示例</span><span class="sxs-lookup"><span data-stu-id="ca68c-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ca68c-130">请求</span><span class="sxs-lookup"><span data-stu-id="ca68c-130">Request</span></span>
<span data-ttu-id="ca68c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca68c-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="ca68c-132">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca68c-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="ca68c-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca68c-133">Response</span></span>
<span data-ttu-id="ca68c-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca68c-134">The following is an example of the response.</span></span>
><span data-ttu-id="ca68c-135">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ca68c-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ca68c-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ca68c-136">All the properties will be returned from an actual call.</span></span>
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
