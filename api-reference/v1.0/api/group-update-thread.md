---
title: 更新对话线程
description: 更新 thread 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1216771a7955cc9460faeab420b8550150d55b84
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679867"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="0f263-103">更新对话线程</span><span class="sxs-lookup"><span data-stu-id="0f263-103">Update conversation thread</span></span>

<span data-ttu-id="0f263-104">命名空间：microsoft.graph 更新 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f263-104">Namespace: microsoft.graph Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f263-105">权限</span><span class="sxs-lookup"><span data-stu-id="0f263-105">Permissions</span></span>
<span data-ttu-id="0f263-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f263-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f263-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f263-108">Permission type</span></span>      | <span data-ttu-id="0f263-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f263-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f263-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f263-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f263-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f263-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f263-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f263-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f263-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f263-113">Not supported.</span></span>    |
|<span data-ttu-id="0f263-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f263-114">Application</span></span> | <span data-ttu-id="0f263-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f263-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f263-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f263-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f263-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f263-117">Request headers</span></span>
| <span data-ttu-id="0f263-118">名称</span><span class="sxs-lookup"><span data-stu-id="0f263-118">Name</span></span>       | <span data-ttu-id="0f263-119">类型</span><span class="sxs-lookup"><span data-stu-id="0f263-119">Type</span></span> | <span data-ttu-id="0f263-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f263-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f263-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f263-121">Authorization</span></span>  | <span data-ttu-id="0f263-122">string</span><span class="sxs-lookup"><span data-stu-id="0f263-122">string</span></span>  | <span data-ttu-id="0f263-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f263-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f263-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f263-125">Request body</span></span>
<span data-ttu-id="0f263-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0f263-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="0f263-129">响应</span><span class="sxs-lookup"><span data-stu-id="0f263-129">Response</span></span>
<span data-ttu-id="0f263-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0f263-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f263-131">示例</span><span class="sxs-lookup"><span data-stu-id="0f263-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f263-132">请求</span><span class="sxs-lookup"><span data-stu-id="0f263-132">Request</span></span>
<span data-ttu-id="0f263-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0f263-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0f263-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f263-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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
# <a name="javascript"></a>[<span data-ttu-id="0f263-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f263-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f263-136">响应</span><span class="sxs-lookup"><span data-stu-id="0f263-136">Response</span></span>
<span data-ttu-id="0f263-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0f263-137">The following is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

