---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1aa7cc397f54b8d9b2d47835fbabab95034950bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038058"
---
# <a name="delete-subscription"></a><span data-ttu-id="a4180-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="a4180-103">Delete subscription</span></span>

<span data-ttu-id="a4180-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4180-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4180-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="a4180-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4180-106">权限</span><span class="sxs-lookup"><span data-stu-id="a4180-106">Permissions</span></span>

<span data-ttu-id="a4180-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="a4180-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a4180-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4180-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4180-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="a4180-109">Supported resource</span></span> | <span data-ttu-id="a4180-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4180-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4180-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4180-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4180-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4180-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a4180-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="a4180-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="a4180-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-114">Not supported</span></span> | <span data-ttu-id="a4180-115">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-115">Not supported</span></span> | <span data-ttu-id="a4180-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-116">CallRecords.Read.All</span></span> |
|[<span data-ttu-id="a4180-117">联系人</span><span class="sxs-lookup"><span data-stu-id="a4180-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a4180-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-118">Contacts.Read</span></span> | <span data-ttu-id="a4180-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-119">Contacts.Read</span></span> | <span data-ttu-id="a4180-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-120">Contacts.Read</span></span> |
|<span data-ttu-id="a4180-121">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a4180-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a4180-122">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-122">Not supported</span></span> | <span data-ttu-id="a4180-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4180-123">Files.ReadWrite</span></span> | <span data-ttu-id="a4180-124">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-124">Not supported</span></span> |
|<span data-ttu-id="a4180-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a4180-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a4180-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="a4180-127">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-127">Not supported</span></span> | <span data-ttu-id="a4180-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a4180-129">事件</span><span class="sxs-lookup"><span data-stu-id="a4180-129">event</span></span>](../resources/event.md) | <span data-ttu-id="a4180-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-130">Calendars.Read</span></span> | <span data-ttu-id="a4180-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-131">Calendars.Read</span></span> | <span data-ttu-id="a4180-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-132">Calendars.Read</span></span> |
|[<span data-ttu-id="a4180-133">组</span><span class="sxs-lookup"><span data-stu-id="a4180-133">group</span></span>](../resources/group.md) | <span data-ttu-id="a4180-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-134">Group.Read.All</span></span> | <span data-ttu-id="a4180-135">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-135">Not supported</span></span> | <span data-ttu-id="a4180-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-136">Group.Read.All</span></span> |
|[<span data-ttu-id="a4180-137">组对话</span><span class="sxs-lookup"><span data-stu-id="a4180-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a4180-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-138">Group.Read.All</span></span> | <span data-ttu-id="a4180-139">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-139">Not supported</span></span> | <span data-ttu-id="a4180-140">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-140">Not supported</span></span> |
|[<span data-ttu-id="a4180-141">列表</span><span class="sxs-lookup"><span data-stu-id="a4180-141">list</span></span>](../resources/list.md) | <span data-ttu-id="a4180-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a4180-143">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-143">Not supported</span></span> | <span data-ttu-id="a4180-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a4180-145">邮件</span><span class="sxs-lookup"><span data-stu-id="a4180-145">message</span></span>](../resources/message.md) | <span data-ttu-id="a4180-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a4180-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a4180-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a4180-148">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="a4180-149">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="a4180-149">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="a4180-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a4180-151">不支持</span><span class="sxs-lookup"><span data-stu-id="a4180-151">Not supported</span></span> | <span data-ttu-id="a4180-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4180-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a4180-153">用户</span><span class="sxs-lookup"><span data-stu-id="a4180-153">user</span></span>](../resources/user.md) | <span data-ttu-id="a4180-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-154">User.Read.All</span></span> | <span data-ttu-id="a4180-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-155">User.Read.All</span></span> | <span data-ttu-id="a4180-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4180-156">User.Read.All</span></span> |

> <span data-ttu-id="a4180-157">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="a4180-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="a4180-158">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="a4180-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="a4180-159">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="a4180-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a4180-160">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="a4180-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a4180-161">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送变更通知。</span><span class="sxs-lookup"><span data-stu-id="a4180-161">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="a4180-162">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="a4180-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="a4180-163">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="a4180-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a4180-164">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="a4180-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="a4180-165">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="a4180-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a4180-166">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="a4180-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a4180-167">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="a4180-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="a4180-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4180-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4180-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4180-169">Request headers</span></span>

| <span data-ttu-id="a4180-170">名称</span><span class="sxs-lookup"><span data-stu-id="a4180-170">Name</span></span>       | <span data-ttu-id="a4180-171">类型</span><span class="sxs-lookup"><span data-stu-id="a4180-171">Type</span></span> | <span data-ttu-id="a4180-172">说明</span><span class="sxs-lookup"><span data-stu-id="a4180-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4180-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4180-173">Authorization</span></span>  | <span data-ttu-id="a4180-174">string</span><span class="sxs-lookup"><span data-stu-id="a4180-174">string</span></span>  | <span data-ttu-id="a4180-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4180-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4180-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4180-177">Request body</span></span>

<span data-ttu-id="a4180-178">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4180-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4180-179">响应</span><span class="sxs-lookup"><span data-stu-id="a4180-179">Response</span></span>

<span data-ttu-id="a4180-180">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4180-180">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="a4180-181">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="a4180-181">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="a4180-182">示例</span><span class="sxs-lookup"><span data-stu-id="a4180-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a4180-183">请求</span><span class="sxs-lookup"><span data-stu-id="a4180-183">Request</span></span>

<span data-ttu-id="a4180-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4180-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4180-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4180-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="a4180-186">C#</span><span class="sxs-lookup"><span data-stu-id="a4180-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4180-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4180-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4180-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4180-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4180-189">Java</span><span class="sxs-lookup"><span data-stu-id="a4180-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4180-190">响应</span><span class="sxs-lookup"><span data-stu-id="a4180-190">Response</span></span>

<span data-ttu-id="a4180-191">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4180-191">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

