---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9fa5a60bbb00bb7d15ae14a0b76235a5629f2c42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537131"
---
# <a name="delete-subscription"></a><span data-ttu-id="f2b21-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="f2b21-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b21-104">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="f2b21-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b21-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2b21-105">Permissions</span></span>

<span data-ttu-id="f2b21-106">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="f2b21-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f2b21-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b21-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2b21-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="f2b21-108">Supported resource</span></span> | <span data-ttu-id="f2b21-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b21-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f2b21-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b21-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2b21-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b21-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="f2b21-112">联系人</span><span class="sxs-lookup"><span data-stu-id="f2b21-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f2b21-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-113">Contacts.Read</span></span> | <span data-ttu-id="f2b21-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-114">Contacts.Read</span></span> | <span data-ttu-id="f2b21-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-115">Contacts.Read</span></span> |
|<span data-ttu-id="f2b21-116">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="f2b21-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="f2b21-117">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-117">Not supported</span></span> | <span data-ttu-id="f2b21-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2b21-118">Files.ReadWrite</span></span> | <span data-ttu-id="f2b21-119">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-119">Not supported</span></span> |
|<span data-ttu-id="f2b21-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="f2b21-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="f2b21-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="f2b21-122">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-122">Not supported</span></span> | <span data-ttu-id="f2b21-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="f2b21-124">event</span><span class="sxs-lookup"><span data-stu-id="f2b21-124">event</span></span>](../resources/event.md) | <span data-ttu-id="f2b21-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-125">Calendars.Read</span></span> | <span data-ttu-id="f2b21-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-126">Calendars.Read</span></span> | <span data-ttu-id="f2b21-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-127">Calendars.Read</span></span> |
|[<span data-ttu-id="f2b21-128">组</span><span class="sxs-lookup"><span data-stu-id="f2b21-128">group</span></span>](../resources/group.md) | <span data-ttu-id="f2b21-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-129">Group.Read.All</span></span> | <span data-ttu-id="f2b21-130">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-130">Not supported</span></span> | <span data-ttu-id="f2b21-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-131">Group.Read.All</span></span> |
|[<span data-ttu-id="f2b21-132">组对话</span><span class="sxs-lookup"><span data-stu-id="f2b21-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="f2b21-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-133">Group.Read.All</span></span> | <span data-ttu-id="f2b21-134">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-134">Not supported</span></span> | <span data-ttu-id="f2b21-135">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-135">Not supported</span></span> |
|[<span data-ttu-id="f2b21-136">message</span><span class="sxs-lookup"><span data-stu-id="f2b21-136">message</span></span>](../resources/message.md) | <span data-ttu-id="f2b21-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-137">Mail.Read</span></span> | <span data-ttu-id="f2b21-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-138">Mail.Read</span></span> | <span data-ttu-id="f2b21-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2b21-139">Mail.Read</span></span> |
|<span data-ttu-id="f2b21-140">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="f2b21-140">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="f2b21-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="f2b21-142">不支持</span><span class="sxs-lookup"><span data-stu-id="f2b21-142">Not supported</span></span> | <span data-ttu-id="f2b21-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="f2b21-144">用户</span><span class="sxs-lookup"><span data-stu-id="f2b21-144">user</span></span>](../resources/user.md) | <span data-ttu-id="f2b21-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-145">User.Read.All</span></span> | <span data-ttu-id="f2b21-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-146">User.Read.All</span></span> | <span data-ttu-id="f2b21-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2b21-147">User.Read.All</span></span> |

> <span data-ttu-id="f2b21-148">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="f2b21-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="f2b21-149">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="f2b21-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="f2b21-150">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="f2b21-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="f2b21-151">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="f2b21-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="f2b21-152">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="f2b21-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="f2b21-153">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="f2b21-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="f2b21-154">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="f2b21-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="f2b21-155">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="f2b21-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="f2b21-156">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="f2b21-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="f2b21-157">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="f2b21-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="f2b21-158">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="f2b21-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="f2b21-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2b21-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2b21-160">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b21-160">Request headers</span></span>

| <span data-ttu-id="f2b21-161">名称</span><span class="sxs-lookup"><span data-stu-id="f2b21-161">Name</span></span>       | <span data-ttu-id="f2b21-162">类型</span><span class="sxs-lookup"><span data-stu-id="f2b21-162">Type</span></span> | <span data-ttu-id="f2b21-163">说明</span><span class="sxs-lookup"><span data-stu-id="f2b21-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2b21-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b21-164">Authorization</span></span>  | <span data-ttu-id="f2b21-165">string</span><span class="sxs-lookup"><span data-stu-id="f2b21-165">string</span></span>  | <span data-ttu-id="f2b21-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b21-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2b21-168">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b21-168">Request body</span></span>

<span data-ttu-id="f2b21-169">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2b21-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2b21-170">响应</span><span class="sxs-lookup"><span data-stu-id="f2b21-170">Response</span></span>

<span data-ttu-id="f2b21-171">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2b21-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2b21-172">示例</span><span class="sxs-lookup"><span data-stu-id="f2b21-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f2b21-173">请求</span><span class="sxs-lookup"><span data-stu-id="f2b21-173">Request</span></span>

<span data-ttu-id="f2b21-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b21-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="f2b21-175">响应</span><span class="sxs-lookup"><span data-stu-id="f2b21-175">Response</span></span>

<span data-ttu-id="f2b21-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2b21-176">Here is an example of the response.</span></span>
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
