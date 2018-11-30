---
title: 创建事件
description: 使用此 API 新建事件。
ms.openlocfilehash: 79d5b4289c3326a02c279ea8e48fc5fef19a7797
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011537"
---
# <a name="create-event"></a><span data-ttu-id="973ad-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="973ad-103">Create event</span></span>
<span data-ttu-id="973ad-104">使用此 API 新建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="973ad-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="973ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="973ad-105">Permissions</span></span>
<span data-ttu-id="973ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="973ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="973ad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="973ad-108">Permission type</span></span>      | <span data-ttu-id="973ad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="973ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="973ad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="973ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="973ad-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="973ad-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="973ad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="973ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="973ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="973ad-113">Not supported.</span></span>    |
|<span data-ttu-id="973ad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="973ad-114">Application</span></span> | <span data-ttu-id="973ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="973ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="973ad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="973ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="973ad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="973ad-117">Request headers</span></span>
| <span data-ttu-id="973ad-118">标头</span><span class="sxs-lookup"><span data-stu-id="973ad-118">Header</span></span>       | <span data-ttu-id="973ad-119">值</span><span class="sxs-lookup"><span data-stu-id="973ad-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="973ad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="973ad-120">Authorization</span></span>  | <span data-ttu-id="973ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="973ad-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="973ad-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="973ad-123">Request body</span></span>
<span data-ttu-id="973ad-124">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="973ad-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="973ad-125">响应</span><span class="sxs-lookup"><span data-stu-id="973ad-125">Response</span></span>
<span data-ttu-id="973ad-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="973ad-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="973ad-127">示例</span><span class="sxs-lookup"><span data-stu-id="973ad-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="973ad-128">请求</span><span class="sxs-lookup"><span data-stu-id="973ad-128">Request</span></span>
<span data-ttu-id="973ad-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="973ad-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

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
<span data-ttu-id="973ad-130">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="973ad-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="973ad-131">响应</span><span class="sxs-lookup"><span data-stu-id="973ad-131">Response</span></span>
<span data-ttu-id="973ad-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="973ad-132">The following is an example of the response.</span></span>
><span data-ttu-id="973ad-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="973ad-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
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
