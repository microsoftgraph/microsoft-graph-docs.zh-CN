---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509460"
---
# <a name="delete-subscription"></a><span data-ttu-id="5352f-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="5352f-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5352f-104">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="5352f-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="5352f-105">权限</span><span class="sxs-lookup"><span data-stu-id="5352f-105">Permissions</span></span>

<span data-ttu-id="5352f-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5352f-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5352f-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="5352f-108">Resource type / Item</span></span>        | <span data-ttu-id="5352f-109">权限</span><span class="sxs-lookup"><span data-stu-id="5352f-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="5352f-110">联系人</span><span class="sxs-lookup"><span data-stu-id="5352f-110">Contacts</span></span>                    | <span data-ttu-id="5352f-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5352f-111">Contacts.Read</span></span>       |
| <span data-ttu-id="5352f-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="5352f-112">Conversations</span></span>               | <span data-ttu-id="5352f-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5352f-113">Group.Read.All</span></span>      |
| <span data-ttu-id="5352f-114">Events</span><span class="sxs-lookup"><span data-stu-id="5352f-114">Events</span></span>                      | <span data-ttu-id="5352f-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5352f-115">Calendars.Read</span></span>      |
| <span data-ttu-id="5352f-116">Messages</span><span class="sxs-lookup"><span data-stu-id="5352f-116">Messages</span></span>                    | <span data-ttu-id="5352f-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5352f-117">Mail.Read</span></span>           |
| <span data-ttu-id="5352f-118">组</span><span class="sxs-lookup"><span data-stu-id="5352f-118">Groups</span></span>                      | <span data-ttu-id="5352f-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5352f-119">Group.Read.All</span></span>      |
| <span data-ttu-id="5352f-120">用户</span><span class="sxs-lookup"><span data-stu-id="5352f-120">Users</span></span>                       | <span data-ttu-id="5352f-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5352f-121">User.Read.All</span></span>       |
| <span data-ttu-id="5352f-122">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="5352f-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="5352f-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5352f-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="5352f-124">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="5352f-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="5352f-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5352f-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="5352f-126">安全警报</span><span class="sxs-lookup"><span data-stu-id="5352f-126">Security alert</span></span>              | <span data-ttu-id="5352f-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5352f-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="5352f-128">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="5352f-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="5352f-129">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="5352f-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="5352f-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5352f-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5352f-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="5352f-131">Request headers</span></span>

| <span data-ttu-id="5352f-132">名称</span><span class="sxs-lookup"><span data-stu-id="5352f-132">Name</span></span>       | <span data-ttu-id="5352f-133">类型</span><span class="sxs-lookup"><span data-stu-id="5352f-133">Type</span></span> | <span data-ttu-id="5352f-134">说明</span><span class="sxs-lookup"><span data-stu-id="5352f-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5352f-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5352f-135">Authorization</span></span>  | <span data-ttu-id="5352f-136">string</span><span class="sxs-lookup"><span data-stu-id="5352f-136">string</span></span>  | <span data-ttu-id="5352f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5352f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5352f-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="5352f-139">Request body</span></span>

<span data-ttu-id="5352f-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5352f-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5352f-141">响应</span><span class="sxs-lookup"><span data-stu-id="5352f-141">Response</span></span>

<span data-ttu-id="5352f-142">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5352f-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5352f-143">示例</span><span class="sxs-lookup"><span data-stu-id="5352f-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5352f-144">请求</span><span class="sxs-lookup"><span data-stu-id="5352f-144">Request</span></span>

<span data-ttu-id="5352f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5352f-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="5352f-146">响应</span><span class="sxs-lookup"><span data-stu-id="5352f-146">Response</span></span>

<span data-ttu-id="5352f-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5352f-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
