---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6c5a123bdba05db63cdd3bc57c4fb65d411217a6
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598484"
---
# <a name="delete-subscription"></a><span data-ttu-id="1603a-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="1603a-103">Delete subscription</span></span>

<span data-ttu-id="1603a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1603a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1603a-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="1603a-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="1603a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1603a-106">Permissions</span></span>

<span data-ttu-id="1603a-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="1603a-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1603a-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1603a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1603a-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="1603a-109">Supported resource</span></span> | <span data-ttu-id="1603a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1603a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1603a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1603a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1603a-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="1603a-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="1603a-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="1603a-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="1603a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-114">Not supported</span></span> | <span data-ttu-id="1603a-115">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-115">Not supported</span></span> | <span data-ttu-id="1603a-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-116">CallRecords.Read.All</span></span> |
|[<span data-ttu-id="1603a-117">联系人</span><span class="sxs-lookup"><span data-stu-id="1603a-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1603a-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-118">Contacts.Read</span></span> | <span data-ttu-id="1603a-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-119">Contacts.Read</span></span> | <span data-ttu-id="1603a-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-120">Contacts.Read</span></span> |
|<span data-ttu-id="1603a-121">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="1603a-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="1603a-122">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-122">Not supported</span></span> | <span data-ttu-id="1603a-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1603a-123">Files.ReadWrite</span></span> | <span data-ttu-id="1603a-124">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-124">Not supported</span></span> |
|<span data-ttu-id="1603a-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="1603a-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="1603a-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="1603a-127">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-127">Not supported</span></span> | <span data-ttu-id="1603a-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="1603a-129">事件</span><span class="sxs-lookup"><span data-stu-id="1603a-129">event</span></span>](../resources/event.md) | <span data-ttu-id="1603a-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-130">Calendars.Read</span></span> | <span data-ttu-id="1603a-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-131">Calendars.Read</span></span> | <span data-ttu-id="1603a-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-132">Calendars.Read</span></span> |
|[<span data-ttu-id="1603a-133">组</span><span class="sxs-lookup"><span data-stu-id="1603a-133">group</span></span>](../resources/group.md) | <span data-ttu-id="1603a-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-134">Group.Read.All</span></span> | <span data-ttu-id="1603a-135">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-135">Not supported</span></span> | <span data-ttu-id="1603a-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-136">Group.Read.All</span></span> |
|[<span data-ttu-id="1603a-137">组对话</span><span class="sxs-lookup"><span data-stu-id="1603a-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="1603a-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-138">Group.Read.All</span></span> | <span data-ttu-id="1603a-139">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-139">Not supported</span></span> | <span data-ttu-id="1603a-140">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-140">Not supported</span></span> |
|[<span data-ttu-id="1603a-141">列表</span><span class="sxs-lookup"><span data-stu-id="1603a-141">list</span></span>](../resources/list.md) | <span data-ttu-id="1603a-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="1603a-143">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-143">Not supported</span></span> | <span data-ttu-id="1603a-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="1603a-145">邮件</span><span class="sxs-lookup"><span data-stu-id="1603a-145">message</span></span>](../resources/message.md) | <span data-ttu-id="1603a-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1603a-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1603a-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1603a-148">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="1603a-149">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="1603a-149">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="1603a-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="1603a-151">不支持</span><span class="sxs-lookup"><span data-stu-id="1603a-151">Not supported</span></span> | <span data-ttu-id="1603a-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1603a-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="1603a-153">用户</span><span class="sxs-lookup"><span data-stu-id="1603a-153">user</span></span>](../resources/user.md) | <span data-ttu-id="1603a-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-154">User.Read.All</span></span> | <span data-ttu-id="1603a-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-155">User.Read.All</span></span> | <span data-ttu-id="1603a-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1603a-156">User.Read.All</span></span> |

> <span data-ttu-id="1603a-157">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="1603a-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="1603a-158">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="1603a-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="1603a-159">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="1603a-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="1603a-160">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="1603a-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="1603a-161">将为订阅的文件夹中的所请求类型的更改发送更改通知，或在其层次结构中的任何文件、文件夹或其他 driveItem 对象上发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="1603a-161">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="1603a-162">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="1603a-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="1603a-163">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="1603a-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="1603a-164">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="1603a-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="1603a-165">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="1603a-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="1603a-166">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="1603a-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="1603a-167">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="1603a-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="1603a-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1603a-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1603a-169">请求标头</span><span class="sxs-lookup"><span data-stu-id="1603a-169">Request headers</span></span>

| <span data-ttu-id="1603a-170">名称</span><span class="sxs-lookup"><span data-stu-id="1603a-170">Name</span></span>       | <span data-ttu-id="1603a-171">类型</span><span class="sxs-lookup"><span data-stu-id="1603a-171">Type</span></span> | <span data-ttu-id="1603a-172">说明</span><span class="sxs-lookup"><span data-stu-id="1603a-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1603a-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="1603a-173">Authorization</span></span>  | <span data-ttu-id="1603a-174">string</span><span class="sxs-lookup"><span data-stu-id="1603a-174">string</span></span>  | <span data-ttu-id="1603a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1603a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1603a-177">请求正文</span><span class="sxs-lookup"><span data-stu-id="1603a-177">Request body</span></span>

<span data-ttu-id="1603a-178">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1603a-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1603a-179">响应</span><span class="sxs-lookup"><span data-stu-id="1603a-179">Response</span></span>

<span data-ttu-id="1603a-180">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1603a-180">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="1603a-181">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="1603a-181">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="1603a-182">示例</span><span class="sxs-lookup"><span data-stu-id="1603a-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1603a-183">请求</span><span class="sxs-lookup"><span data-stu-id="1603a-183">Request</span></span>

<span data-ttu-id="1603a-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1603a-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1603a-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="1603a-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="1603a-186">C#</span><span class="sxs-lookup"><span data-stu-id="1603a-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1603a-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1603a-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1603a-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1603a-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1603a-189">Java</span><span class="sxs-lookup"><span data-stu-id="1603a-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1603a-190">响应</span><span class="sxs-lookup"><span data-stu-id="1603a-190">Response</span></span>

<span data-ttu-id="1603a-191">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1603a-191">Here is an example of the response.</span></span>
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
