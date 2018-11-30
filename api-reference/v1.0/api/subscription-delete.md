---
title: 删除订阅
description: 删除订阅。
ms.openlocfilehash: 249393cef11e2768eec0a6435a8485b51cf6921c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011510"
---
# <a name="delete-subscription"></a><span data-ttu-id="07b98-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="07b98-103">Delete subscription</span></span>

<span data-ttu-id="07b98-104">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="07b98-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="07b98-105">权限</span><span class="sxs-lookup"><span data-stu-id="07b98-105">Permissions</span></span>

<span data-ttu-id="07b98-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07b98-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07b98-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="07b98-108">Resource type / Item</span></span>        | <span data-ttu-id="07b98-109">权限</span><span class="sxs-lookup"><span data-stu-id="07b98-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="07b98-110">联系人</span><span class="sxs-lookup"><span data-stu-id="07b98-110">Contacts</span></span>                    | <span data-ttu-id="07b98-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07b98-111">Contacts.Read</span></span>       |
| <span data-ttu-id="07b98-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="07b98-112">Conversations</span></span>               | <span data-ttu-id="07b98-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07b98-113">Group.Read.All</span></span>      |
| <span data-ttu-id="07b98-114">Events</span><span class="sxs-lookup"><span data-stu-id="07b98-114">Events</span></span>                      | <span data-ttu-id="07b98-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07b98-115">Calendars.Read</span></span>      |
| <span data-ttu-id="07b98-116">Messages</span><span class="sxs-lookup"><span data-stu-id="07b98-116">Messages</span></span>                    | <span data-ttu-id="07b98-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07b98-117">Mail.Read</span></span>           |
| <span data-ttu-id="07b98-118">Groups</span><span class="sxs-lookup"><span data-stu-id="07b98-118">Groups</span></span>                      | <span data-ttu-id="07b98-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07b98-119">Group.Read.All</span></span>      |
| <span data-ttu-id="07b98-120">Users</span><span class="sxs-lookup"><span data-stu-id="07b98-120">Users</span></span>                       | <span data-ttu-id="07b98-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07b98-121">User.Read.All</span></span>       |
| <span data-ttu-id="07b98-122">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="07b98-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="07b98-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07b98-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="07b98-124">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="07b98-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="07b98-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b98-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="07b98-126">安全警报</span><span class="sxs-lookup"><span data-stu-id="07b98-126">Security alert</span></span>| <span data-ttu-id="07b98-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b98-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07b98-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07b98-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="07b98-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="07b98-129">Request headers</span></span>

| <span data-ttu-id="07b98-130">名称</span><span class="sxs-lookup"><span data-stu-id="07b98-130">Name</span></span>       | <span data-ttu-id="07b98-131">类型</span><span class="sxs-lookup"><span data-stu-id="07b98-131">Type</span></span> | <span data-ttu-id="07b98-132">说明</span><span class="sxs-lookup"><span data-stu-id="07b98-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07b98-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="07b98-133">Authorization</span></span>  | <span data-ttu-id="07b98-134">string</span><span class="sxs-lookup"><span data-stu-id="07b98-134">string</span></span>  | <span data-ttu-id="07b98-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07b98-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07b98-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="07b98-137">Request body</span></span>

<span data-ttu-id="07b98-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07b98-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07b98-139">响应</span><span class="sxs-lookup"><span data-stu-id="07b98-139">Response</span></span>

<span data-ttu-id="07b98-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="07b98-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07b98-141">示例</span><span class="sxs-lookup"><span data-stu-id="07b98-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="07b98-142">请求</span><span class="sxs-lookup"><span data-stu-id="07b98-142">Request</span></span>

<span data-ttu-id="07b98-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07b98-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="07b98-144">响应</span><span class="sxs-lookup"><span data-stu-id="07b98-144">Response</span></span>

<span data-ttu-id="07b98-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="07b98-145">Here is an example of the response.</span></span>
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
