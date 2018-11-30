---
title: 删除 historyItem
description: 删除现有用户活动的现有历史记录项。
ms.openlocfilehash: bf8d8c064a3a29aec8f59a2d4de5ae6732d0f0e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043990"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="e488d-103">删除 historyItem</span><span class="sxs-lookup"><span data-stu-id="e488d-103">Delete a historyItem</span></span>

> <span data-ttu-id="e488d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e488d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e488d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e488d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e488d-106">删除现有用户活动的现有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e488d-106">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="e488d-107">权限</span><span class="sxs-lookup"><span data-stu-id="e488d-107">Permissions</span></span>

<span data-ttu-id="e488d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e488d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e488d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e488d-110">Permission type</span></span>      | <span data-ttu-id="e488d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e488d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e488d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e488d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e488d-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e488d-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e488d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e488d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e488d-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e488d-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e488d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e488d-116">Application</span></span> | <span data-ttu-id="e488d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e488d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e488d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e488d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e488d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e488d-119">Request headers</span></span>

|<span data-ttu-id="e488d-120">名称</span><span class="sxs-lookup"><span data-stu-id="e488d-120">Name</span></span> | <span data-ttu-id="e488d-121">类型</span><span class="sxs-lookup"><span data-stu-id="e488d-121">Type</span></span> | <span data-ttu-id="e488d-122">说明</span><span class="sxs-lookup"><span data-stu-id="e488d-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e488d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e488d-123">Authorization</span></span> | <span data-ttu-id="e488d-124">string</span><span class="sxs-lookup"><span data-stu-id="e488d-124">string</span></span> | <span data-ttu-id="e488d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e488d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e488d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e488d-127">Request body</span></span>

<span data-ttu-id="e488d-128">没有请求正文中。</span><span class="sxs-lookup"><span data-stu-id="e488d-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="e488d-129">响应</span><span class="sxs-lookup"><span data-stu-id="e488d-129">Response</span></span>

<span data-ttu-id="e488d-130">如果成功，此方法返回`204 No Content`如果历史记录项已删除的响应代码。</span><span class="sxs-lookup"><span data-stu-id="e488d-130">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="e488d-131">示例</span><span class="sxs-lookup"><span data-stu-id="e488d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e488d-132">请求</span><span class="sxs-lookup"><span data-stu-id="e488d-132">Request</span></span>

<span data-ttu-id="e488d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e488d-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="e488d-134">响应</span><span class="sxs-lookup"><span data-stu-id="e488d-134">Response</span></span>

<span data-ttu-id="e488d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e488d-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->