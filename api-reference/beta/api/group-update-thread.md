---
title: 更新对话线程
description: 更新 thread 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: defb7560a1d407a60ac813154ebd978f554e9763
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966256"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="7aee5-103">更新对话线程</span><span class="sxs-lookup"><span data-stu-id="7aee5-103">Update conversation thread</span></span>

> <span data-ttu-id="7aee5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7aee5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aee5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7aee5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7aee5-106">更新 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7aee5-106">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aee5-107">权限</span><span class="sxs-lookup"><span data-stu-id="7aee5-107">Permissions</span></span>
<span data-ttu-id="7aee5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aee5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aee5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aee5-110">Permission type</span></span>      | <span data-ttu-id="7aee5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aee5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aee5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aee5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7aee5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aee5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aee5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aee5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aee5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aee5-115">Not supported.</span></span>    |
|<span data-ttu-id="7aee5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aee5-116">Application</span></span> | <span data-ttu-id="7aee5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aee5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aee5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aee5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7aee5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aee5-119">Request headers</span></span>
| <span data-ttu-id="7aee5-120">名称</span><span class="sxs-lookup"><span data-stu-id="7aee5-120">Name</span></span>       | <span data-ttu-id="7aee5-121">类型</span><span class="sxs-lookup"><span data-stu-id="7aee5-121">Type</span></span> | <span data-ttu-id="7aee5-122">说明</span><span class="sxs-lookup"><span data-stu-id="7aee5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7aee5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aee5-123">Authorization</span></span>  | <span data-ttu-id="7aee5-124">string</span><span class="sxs-lookup"><span data-stu-id="7aee5-124">string</span></span>  | <span data-ttu-id="7aee5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aee5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aee5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aee5-127">Request body</span></span>
<span data-ttu-id="7aee5-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7aee5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7aee5-131">响应</span><span class="sxs-lookup"><span data-stu-id="7aee5-131">Response</span></span>
<span data-ttu-id="7aee5-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7aee5-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7aee5-133">示例</span><span class="sxs-lookup"><span data-stu-id="7aee5-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7aee5-134">请求</span><span class="sxs-lookup"><span data-stu-id="7aee5-134">Request</span></span>
<span data-ttu-id="7aee5-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7aee5-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="7aee5-136">响应</span><span class="sxs-lookup"><span data-stu-id="7aee5-136">Response</span></span>
<span data-ttu-id="7aee5-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7aee5-137">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
