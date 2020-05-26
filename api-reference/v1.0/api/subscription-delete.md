---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f1f0dc151748d1f61f002f94243c13ce0f81c94b
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353175"
---
# <a name="delete-subscription"></a><span data-ttu-id="21d00-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="21d00-103">Delete subscription</span></span>

<span data-ttu-id="21d00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21d00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21d00-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="21d00-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="21d00-106">权限</span><span class="sxs-lookup"><span data-stu-id="21d00-106">Permissions</span></span>

<span data-ttu-id="21d00-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="21d00-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="21d00-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21d00-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21d00-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="21d00-109">Supported resource</span></span> | <span data-ttu-id="21d00-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21d00-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21d00-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21d00-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21d00-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="21d00-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="21d00-113">联系人</span><span class="sxs-lookup"><span data-stu-id="21d00-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="21d00-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-114">Contacts.Read</span></span> | <span data-ttu-id="21d00-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-115">Contacts.Read</span></span> | <span data-ttu-id="21d00-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-116">Contacts.Read</span></span> |
|<span data-ttu-id="21d00-117">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="21d00-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="21d00-118">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-118">Not supported</span></span> | <span data-ttu-id="21d00-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21d00-119">Files.ReadWrite</span></span> | <span data-ttu-id="21d00-120">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-120">Not supported</span></span> |
|<span data-ttu-id="21d00-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="21d00-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="21d00-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="21d00-123">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-123">Not supported</span></span> | <span data-ttu-id="21d00-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="21d00-125">事件</span><span class="sxs-lookup"><span data-stu-id="21d00-125">event</span></span>](../resources/event.md) | <span data-ttu-id="21d00-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-126">Calendars.Read</span></span> | <span data-ttu-id="21d00-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-127">Calendars.Read</span></span> | <span data-ttu-id="21d00-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-128">Calendars.Read</span></span> |
|[<span data-ttu-id="21d00-129">组</span><span class="sxs-lookup"><span data-stu-id="21d00-129">group</span></span>](../resources/group.md) | <span data-ttu-id="21d00-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-130">Group.Read.All</span></span> | <span data-ttu-id="21d00-131">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-131">Not supported</span></span> | <span data-ttu-id="21d00-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-132">Group.Read.All</span></span> |
|[<span data-ttu-id="21d00-133">组对话</span><span class="sxs-lookup"><span data-stu-id="21d00-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="21d00-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-134">Group.Read.All</span></span> | <span data-ttu-id="21d00-135">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-135">Not supported</span></span> | <span data-ttu-id="21d00-136">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-136">Not supported</span></span> |
|[<span data-ttu-id="21d00-137">列表</span><span class="sxs-lookup"><span data-stu-id="21d00-137">list</span></span>](../resources/list.md) | <span data-ttu-id="21d00-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="21d00-139">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-139">Not supported</span></span> | <span data-ttu-id="21d00-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="21d00-141">邮件</span><span class="sxs-lookup"><span data-stu-id="21d00-141">message</span></span>](../resources/message.md) | <span data-ttu-id="21d00-142">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="21d00-143">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="21d00-144">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="21d00-144">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="21d00-145">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="21d00-145">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="21d00-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="21d00-147">不支持</span><span class="sxs-lookup"><span data-stu-id="21d00-147">Not supported</span></span> | <span data-ttu-id="21d00-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d00-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="21d00-149">用户</span><span class="sxs-lookup"><span data-stu-id="21d00-149">user</span></span>](../resources/user.md) | <span data-ttu-id="21d00-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-150">User.Read.All</span></span> | <span data-ttu-id="21d00-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-151">User.Read.All</span></span> | <span data-ttu-id="21d00-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d00-152">User.Read.All</span></span> |

> <span data-ttu-id="21d00-153">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="21d00-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="21d00-154">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="21d00-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="21d00-155">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="21d00-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="21d00-156">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="21d00-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="21d00-157">将为订阅的文件夹中的所请求类型的更改发送更改通知，或在其层次结构中的任何文件、文件夹或其他 driveItem 对象上发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="21d00-157">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="21d00-158">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="21d00-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="21d00-159">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="21d00-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="21d00-160">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="21d00-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="21d00-161">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="21d00-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="21d00-162">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="21d00-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="21d00-163">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="21d00-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="21d00-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21d00-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21d00-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="21d00-165">Request headers</span></span>

| <span data-ttu-id="21d00-166">名称</span><span class="sxs-lookup"><span data-stu-id="21d00-166">Name</span></span>       | <span data-ttu-id="21d00-167">类型</span><span class="sxs-lookup"><span data-stu-id="21d00-167">Type</span></span> | <span data-ttu-id="21d00-168">说明</span><span class="sxs-lookup"><span data-stu-id="21d00-168">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21d00-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="21d00-169">Authorization</span></span>  | <span data-ttu-id="21d00-170">string</span><span class="sxs-lookup"><span data-stu-id="21d00-170">string</span></span>  | <span data-ttu-id="21d00-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21d00-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21d00-173">请求正文</span><span class="sxs-lookup"><span data-stu-id="21d00-173">Request body</span></span>

<span data-ttu-id="21d00-174">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21d00-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21d00-175">响应</span><span class="sxs-lookup"><span data-stu-id="21d00-175">Response</span></span>

<span data-ttu-id="21d00-176">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="21d00-176">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="21d00-177">有关如何返回错误的详细信息，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="21d00-177">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="21d00-178">示例</span><span class="sxs-lookup"><span data-stu-id="21d00-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="21d00-179">请求</span><span class="sxs-lookup"><span data-stu-id="21d00-179">Request</span></span>

<span data-ttu-id="21d00-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21d00-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21d00-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="21d00-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="21d00-182">C#</span><span class="sxs-lookup"><span data-stu-id="21d00-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21d00-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21d00-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21d00-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21d00-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21d00-185">Java</span><span class="sxs-lookup"><span data-stu-id="21d00-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="21d00-186">响应</span><span class="sxs-lookup"><span data-stu-id="21d00-186">Response</span></span>

<span data-ttu-id="21d00-187">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="21d00-187">Here is an example of the response.</span></span>
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
