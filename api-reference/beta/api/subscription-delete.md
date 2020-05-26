---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 8ce81955a4436f65d0833d3b4f9301bb44c62a3f
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353271"
---
# <a name="delete-subscription"></a><span data-ttu-id="44e7b-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="44e7b-103">Delete subscription</span></span>

<span data-ttu-id="44e7b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44e7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e7b-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="44e7b-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="44e7b-106">权限</span><span class="sxs-lookup"><span data-stu-id="44e7b-106">Permissions</span></span>

<span data-ttu-id="44e7b-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="44e7b-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="44e7b-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44e7b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44e7b-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="44e7b-109">Supported resource</span></span> | <span data-ttu-id="44e7b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44e7b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44e7b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44e7b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44e7b-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="44e7b-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="44e7b-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="44e7b-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="44e7b-114">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-114">Not supported</span></span> | <span data-ttu-id="44e7b-115">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-115">Not supported</span></span> | <span data-ttu-id="44e7b-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-116">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="44e7b-117">联系人</span><span class="sxs-lookup"><span data-stu-id="44e7b-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="44e7b-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-118">Contacts.Read</span></span> | <span data-ttu-id="44e7b-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-119">Contacts.Read</span></span> | <span data-ttu-id="44e7b-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-120">Contacts.Read</span></span> |
|<span data-ttu-id="44e7b-121">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="44e7b-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="44e7b-122">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-122">Not supported</span></span> | <span data-ttu-id="44e7b-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44e7b-123">Files.ReadWrite</span></span> | <span data-ttu-id="44e7b-124">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-124">Not supported</span></span> |
|<span data-ttu-id="44e7b-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="44e7b-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="44e7b-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="44e7b-127">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-127">Not supported</span></span> | <span data-ttu-id="44e7b-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="44e7b-129">事件</span><span class="sxs-lookup"><span data-stu-id="44e7b-129">event</span></span>](../resources/event.md) | <span data-ttu-id="44e7b-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-130">Calendars.Read</span></span> | <span data-ttu-id="44e7b-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-131">Calendars.Read</span></span> | <span data-ttu-id="44e7b-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-132">Calendars.Read</span></span> |
|[<span data-ttu-id="44e7b-133">组</span><span class="sxs-lookup"><span data-stu-id="44e7b-133">group</span></span>](../resources/group.md) | <span data-ttu-id="44e7b-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-134">Group.Read.All</span></span> | <span data-ttu-id="44e7b-135">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-135">Not supported</span></span> | <span data-ttu-id="44e7b-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-136">Group.Read.All</span></span> |
|[<span data-ttu-id="44e7b-137">组对话</span><span class="sxs-lookup"><span data-stu-id="44e7b-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="44e7b-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-138">Group.Read.All</span></span> | <span data-ttu-id="44e7b-139">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-139">Not supported</span></span> | <span data-ttu-id="44e7b-140">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-140">Not supported</span></span> |
|[<span data-ttu-id="44e7b-141">列表</span><span class="sxs-lookup"><span data-stu-id="44e7b-141">list</span></span>](../resources/list.md) | <span data-ttu-id="44e7b-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="44e7b-143">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-143">Not supported</span></span> | <span data-ttu-id="44e7b-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="44e7b-145">邮件</span><span class="sxs-lookup"><span data-stu-id="44e7b-145">message</span></span>](../resources/message.md) | <span data-ttu-id="44e7b-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="44e7b-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="44e7b-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="44e7b-148">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="44e7b-149">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="44e7b-149">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="44e7b-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="44e7b-151">不支持</span><span class="sxs-lookup"><span data-stu-id="44e7b-151">Not supported</span></span> | <span data-ttu-id="44e7b-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="44e7b-153">用户</span><span class="sxs-lookup"><span data-stu-id="44e7b-153">user</span></span>](../resources/user.md) | <span data-ttu-id="44e7b-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-154">User.Read.All</span></span> | <span data-ttu-id="44e7b-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-155">User.Read.All</span></span> | <span data-ttu-id="44e7b-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="44e7b-156">User.Read.All</span></span> |

> <span data-ttu-id="44e7b-157">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="44e7b-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="44e7b-158">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="44e7b-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="44e7b-159">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="44e7b-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="44e7b-160">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="44e7b-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="44e7b-161">将为订阅的文件夹中的所请求类型的更改发送更改通知，或在其层次结构中的任何文件、文件夹或其他 driveItem 对象上发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="44e7b-161">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="44e7b-162">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="44e7b-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="44e7b-163">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="44e7b-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="44e7b-164">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="44e7b-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="44e7b-165">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="44e7b-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="44e7b-166">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="44e7b-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="44e7b-167">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="44e7b-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="44e7b-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44e7b-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44e7b-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="44e7b-169">Request headers</span></span>

| <span data-ttu-id="44e7b-170">名称</span><span class="sxs-lookup"><span data-stu-id="44e7b-170">Name</span></span>       | <span data-ttu-id="44e7b-171">类型</span><span class="sxs-lookup"><span data-stu-id="44e7b-171">Type</span></span> | <span data-ttu-id="44e7b-172">说明</span><span class="sxs-lookup"><span data-stu-id="44e7b-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44e7b-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e7b-173">Authorization</span></span>  | <span data-ttu-id="44e7b-174">string</span><span class="sxs-lookup"><span data-stu-id="44e7b-174">string</span></span>  | <span data-ttu-id="44e7b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44e7b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44e7b-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="44e7b-177">Request body</span></span>

<span data-ttu-id="44e7b-178">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44e7b-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44e7b-179">响应</span><span class="sxs-lookup"><span data-stu-id="44e7b-179">Response</span></span>

<span data-ttu-id="44e7b-180">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="44e7b-180">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="44e7b-181">有关如何返回错误的详细信息，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="44e7b-181">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="44e7b-182">示例</span><span class="sxs-lookup"><span data-stu-id="44e7b-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="44e7b-183">请求</span><span class="sxs-lookup"><span data-stu-id="44e7b-183">Request</span></span>

<span data-ttu-id="44e7b-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44e7b-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44e7b-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="44e7b-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="44e7b-186">C#</span><span class="sxs-lookup"><span data-stu-id="44e7b-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44e7b-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44e7b-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44e7b-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44e7b-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="44e7b-189">响应</span><span class="sxs-lookup"><span data-stu-id="44e7b-189">Response</span></span>

<span data-ttu-id="44e7b-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="44e7b-190">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

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
