---
title: 更新事件
description: 更新 event 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d1a6c5f26b732cd98083db5919082a7ce1c41182
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681254"
---
# <a name="update-event"></a><span data-ttu-id="3dcbc-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="3dcbc-103">Update event</span></span>

<span data-ttu-id="3dcbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dcbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dcbc-105">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-105">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dcbc-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dcbc-106">Permissions</span></span>
<span data-ttu-id="3dcbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dcbc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dcbc-109">Permission type</span></span>      | <span data-ttu-id="3dcbc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dcbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dcbc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dcbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3dcbc-112">Calendars.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dcbc-112">Calendars.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dcbc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dcbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dcbc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-114">Not supported.</span></span>    |
|<span data-ttu-id="3dcbc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dcbc-115">Application</span></span> | <span data-ttu-id="3dcbc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dcbc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dcbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3dcbc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dcbc-118">Request headers</span></span>
| <span data-ttu-id="3dcbc-119">名称</span><span class="sxs-lookup"><span data-stu-id="3dcbc-119">Name</span></span>       | <span data-ttu-id="3dcbc-120">类型</span><span class="sxs-lookup"><span data-stu-id="3dcbc-120">Type</span></span> | <span data-ttu-id="3dcbc-121">说明</span><span class="sxs-lookup"><span data-stu-id="3dcbc-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3dcbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dcbc-122">Authorization</span></span>  | <span data-ttu-id="3dcbc-123">string</span><span class="sxs-lookup"><span data-stu-id="3dcbc-123">string</span></span>  | <span data-ttu-id="3dcbc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dcbc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dcbc-126">Request body</span></span>
<span data-ttu-id="3dcbc-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="3dcbc-130">响应</span><span class="sxs-lookup"><span data-stu-id="3dcbc-130">Response</span></span>
<span data-ttu-id="3dcbc-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3dcbc-132">示例</span><span class="sxs-lookup"><span data-stu-id="3dcbc-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3dcbc-133">请求</span><span class="sxs-lookup"><span data-stu-id="3dcbc-133">Request</span></span>
<span data-ttu-id="3dcbc-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3dcbc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dcbc-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3dcbc-136">C#</span><span class="sxs-lookup"><span data-stu-id="3dcbc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dcbc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dcbc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3dcbc-138">Java</span><span class="sxs-lookup"><span data-stu-id="3dcbc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3dcbc-139">响应</span><span class="sxs-lookup"><span data-stu-id="3dcbc-139">Response</span></span>
<span data-ttu-id="3dcbc-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3dcbc-140">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


