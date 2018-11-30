---
title: 删除订阅
description: 删除订阅。
ms.openlocfilehash: be2c32f0915e8718203e46489be9861bf0f05451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043064"
---
# <a name="delete-subscription"></a><span data-ttu-id="7caf3-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="7caf3-103">Delete subscription</span></span>

> <span data-ttu-id="7caf3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7caf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7caf3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7caf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7caf3-106">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="7caf3-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="7caf3-107">权限</span><span class="sxs-lookup"><span data-stu-id="7caf3-107">Permissions</span></span>

<span data-ttu-id="7caf3-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7caf3-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7caf3-110">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="7caf3-110">Resource type / Item</span></span>        | <span data-ttu-id="7caf3-111">权限</span><span class="sxs-lookup"><span data-stu-id="7caf3-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="7caf3-112">联系人</span><span class="sxs-lookup"><span data-stu-id="7caf3-112">Contacts</span></span>                    | <span data-ttu-id="7caf3-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7caf3-113">Contacts.Read</span></span>       |
| <span data-ttu-id="7caf3-114">Conversations</span><span class="sxs-lookup"><span data-stu-id="7caf3-114">Conversations</span></span>               | <span data-ttu-id="7caf3-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-115">Group.Read.All</span></span>      |
| <span data-ttu-id="7caf3-116">Events</span><span class="sxs-lookup"><span data-stu-id="7caf3-116">Events</span></span>                      | <span data-ttu-id="7caf3-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7caf3-117">Calendars.Read</span></span>      |
| <span data-ttu-id="7caf3-118">Messages</span><span class="sxs-lookup"><span data-stu-id="7caf3-118">Messages</span></span>                    | <span data-ttu-id="7caf3-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7caf3-119">Mail.Read</span></span>           |
| <span data-ttu-id="7caf3-120">Groups</span><span class="sxs-lookup"><span data-stu-id="7caf3-120">Groups</span></span>                      | <span data-ttu-id="7caf3-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-121">Group.Read.All</span></span>      |
| <span data-ttu-id="7caf3-122">Users</span><span class="sxs-lookup"><span data-stu-id="7caf3-122">Users</span></span>                       | <span data-ttu-id="7caf3-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-123">User.Read.All</span></span>       |
| <span data-ttu-id="7caf3-124">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="7caf3-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="7caf3-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7caf3-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="7caf3-126">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="7caf3-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="7caf3-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="7caf3-128">安全警报</span><span class="sxs-lookup"><span data-stu-id="7caf3-128">Security alert</span></span>              | <span data-ttu-id="7caf3-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7caf3-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="7caf3-130">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="7caf3-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="7caf3-131">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="7caf3-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="7caf3-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7caf3-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7caf3-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="7caf3-133">Request headers</span></span>

| <span data-ttu-id="7caf3-134">名称</span><span class="sxs-lookup"><span data-stu-id="7caf3-134">Name</span></span>       | <span data-ttu-id="7caf3-135">类型</span><span class="sxs-lookup"><span data-stu-id="7caf3-135">Type</span></span> | <span data-ttu-id="7caf3-136">说明</span><span class="sxs-lookup"><span data-stu-id="7caf3-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7caf3-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7caf3-137">Authorization</span></span>  | <span data-ttu-id="7caf3-138">string</span><span class="sxs-lookup"><span data-stu-id="7caf3-138">string</span></span>  | <span data-ttu-id="7caf3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7caf3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7caf3-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="7caf3-141">Request body</span></span>

<span data-ttu-id="7caf3-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7caf3-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7caf3-143">响应</span><span class="sxs-lookup"><span data-stu-id="7caf3-143">Response</span></span>

<span data-ttu-id="7caf3-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7caf3-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7caf3-145">示例</span><span class="sxs-lookup"><span data-stu-id="7caf3-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7caf3-146">请求</span><span class="sxs-lookup"><span data-stu-id="7caf3-146">Request</span></span>

<span data-ttu-id="7caf3-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7caf3-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="7caf3-148">响应</span><span class="sxs-lookup"><span data-stu-id="7caf3-148">Response</span></span>

<span data-ttu-id="7caf3-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7caf3-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
