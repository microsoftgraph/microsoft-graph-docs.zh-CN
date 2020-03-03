---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3328291435e3d6ce067b21a604d76ce46ee5ea2e
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394465"
---
# <a name="delete-subscription"></a><span data-ttu-id="329d1-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="329d1-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="329d1-104">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="329d1-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="329d1-105">权限</span><span class="sxs-lookup"><span data-stu-id="329d1-105">Permissions</span></span>

<span data-ttu-id="329d1-106">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="329d1-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="329d1-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="329d1-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="329d1-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="329d1-108">Supported resource</span></span> | <span data-ttu-id="329d1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="329d1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="329d1-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="329d1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="329d1-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="329d1-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="329d1-112">callRecord</span><span class="sxs-lookup"><span data-stu-id="329d1-112">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="329d1-113">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-113">Not supported</span></span> | <span data-ttu-id="329d1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-114">Not supported</span></span> | <span data-ttu-id="329d1-115">CallRecords</span><span class="sxs-lookup"><span data-stu-id="329d1-115">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="329d1-116">联系人</span><span class="sxs-lookup"><span data-stu-id="329d1-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="329d1-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-117">Contacts.Read</span></span> | <span data-ttu-id="329d1-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-118">Contacts.Read</span></span> | <span data-ttu-id="329d1-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-119">Contacts.Read</span></span> |
|<span data-ttu-id="329d1-120">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="329d1-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="329d1-121">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-121">Not supported</span></span> | <span data-ttu-id="329d1-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="329d1-122">Files.ReadWrite</span></span> | <span data-ttu-id="329d1-123">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-123">Not supported</span></span> |
|<span data-ttu-id="329d1-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="329d1-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="329d1-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="329d1-126">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-126">Not supported</span></span> | <span data-ttu-id="329d1-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="329d1-128">事件</span><span class="sxs-lookup"><span data-stu-id="329d1-128">event</span></span>](../resources/event.md) | <span data-ttu-id="329d1-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-129">Calendars.Read</span></span> | <span data-ttu-id="329d1-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-130">Calendars.Read</span></span> | <span data-ttu-id="329d1-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-131">Calendars.Read</span></span> |
|[<span data-ttu-id="329d1-132">组</span><span class="sxs-lookup"><span data-stu-id="329d1-132">group</span></span>](../resources/group.md) | <span data-ttu-id="329d1-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-133">Group.Read.All</span></span> | <span data-ttu-id="329d1-134">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-134">Not supported</span></span> | <span data-ttu-id="329d1-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-135">Group.Read.All</span></span> |
|[<span data-ttu-id="329d1-136">组对话</span><span class="sxs-lookup"><span data-stu-id="329d1-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="329d1-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-137">Group.Read.All</span></span> | <span data-ttu-id="329d1-138">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-138">Not supported</span></span> | <span data-ttu-id="329d1-139">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-139">Not supported</span></span> |
|[<span data-ttu-id="329d1-140">list</span><span class="sxs-lookup"><span data-stu-id="329d1-140">list</span></span>](../resources/list.md) | <span data-ttu-id="329d1-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="329d1-142">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-142">Not supported</span></span> | <span data-ttu-id="329d1-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="329d1-144">邮件</span><span class="sxs-lookup"><span data-stu-id="329d1-144">message</span></span>](../resources/message.md) | <span data-ttu-id="329d1-145">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="329d1-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="329d1-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="329d1-147">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="329d1-148">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="329d1-148">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="329d1-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="329d1-150">不支持</span><span class="sxs-lookup"><span data-stu-id="329d1-150">Not supported</span></span> | <span data-ttu-id="329d1-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329d1-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="329d1-152">用户</span><span class="sxs-lookup"><span data-stu-id="329d1-152">user</span></span>](../resources/user.md) | <span data-ttu-id="329d1-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-153">User.Read.All</span></span> | <span data-ttu-id="329d1-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-154">User.Read.All</span></span> | <span data-ttu-id="329d1-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="329d1-155">User.Read.All</span></span> |

> <span data-ttu-id="329d1-156">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="329d1-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="329d1-157">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="329d1-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="329d1-158">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="329d1-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="329d1-159">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="329d1-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="329d1-160">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="329d1-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="329d1-161">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="329d1-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="329d1-162">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="329d1-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="329d1-163">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="329d1-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="329d1-164">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="329d1-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="329d1-165">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="329d1-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="329d1-166">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="329d1-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="329d1-167">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="329d1-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="329d1-168">请求标头</span><span class="sxs-lookup"><span data-stu-id="329d1-168">Request headers</span></span>

| <span data-ttu-id="329d1-169">名称</span><span class="sxs-lookup"><span data-stu-id="329d1-169">Name</span></span>       | <span data-ttu-id="329d1-170">类型</span><span class="sxs-lookup"><span data-stu-id="329d1-170">Type</span></span> | <span data-ttu-id="329d1-171">说明</span><span class="sxs-lookup"><span data-stu-id="329d1-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="329d1-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="329d1-172">Authorization</span></span>  | <span data-ttu-id="329d1-173">string</span><span class="sxs-lookup"><span data-stu-id="329d1-173">string</span></span>  | <span data-ttu-id="329d1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="329d1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="329d1-176">请求正文</span><span class="sxs-lookup"><span data-stu-id="329d1-176">Request body</span></span>

<span data-ttu-id="329d1-177">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="329d1-177">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="329d1-178">响应</span><span class="sxs-lookup"><span data-stu-id="329d1-178">Response</span></span>

<span data-ttu-id="329d1-179">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="329d1-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="329d1-180">示例</span><span class="sxs-lookup"><span data-stu-id="329d1-180">Example</span></span>

##### <a name="request"></a><span data-ttu-id="329d1-181">请求</span><span class="sxs-lookup"><span data-stu-id="329d1-181">Request</span></span>

<span data-ttu-id="329d1-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="329d1-182">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="329d1-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="329d1-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="329d1-184">C#</span><span class="sxs-lookup"><span data-stu-id="329d1-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="329d1-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="329d1-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="329d1-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="329d1-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="329d1-187">响应</span><span class="sxs-lookup"><span data-stu-id="329d1-187">Response</span></span>

<span data-ttu-id="329d1-188">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="329d1-188">Here is an example of the response.</span></span>
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
  ]
}
-->
