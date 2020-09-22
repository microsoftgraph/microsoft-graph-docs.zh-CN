---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: aee0ca84cccd371c307b405357516d8fda61deab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038030"
---
# <a name="update-subscription"></a><span data-ttu-id="2f506-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="2f506-103">Update subscription</span></span>

<span data-ttu-id="2f506-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f506-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f506-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="2f506-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="2f506-106">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="2f506-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="2f506-107">为了避免丢失更改通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="2f506-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="2f506-108">有关每种资源类型的最大订阅长度，请参阅 [订阅](../resources/subscription.md) 。</span><span class="sxs-lookup"><span data-stu-id="2f506-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f506-109">权限</span><span class="sxs-lookup"><span data-stu-id="2f506-109">Permissions</span></span>

<span data-ttu-id="2f506-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="2f506-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2f506-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f506-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f506-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="2f506-112">Supported resource</span></span> | <span data-ttu-id="2f506-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f506-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f506-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f506-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f506-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f506-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2f506-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="2f506-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="2f506-117">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-117">Not supported</span></span> | <span data-ttu-id="2f506-118">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-118">Not supported</span></span> | <span data-ttu-id="2f506-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-119">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="2f506-120">联系人</span><span class="sxs-lookup"><span data-stu-id="2f506-120">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2f506-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-121">Contacts.Read</span></span> | <span data-ttu-id="2f506-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-122">Contacts.Read</span></span> | <span data-ttu-id="2f506-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-123">Contacts.Read</span></span> |
|<span data-ttu-id="2f506-124">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="2f506-124">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2f506-125">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-125">Not supported</span></span> | <span data-ttu-id="2f506-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f506-126">Files.ReadWrite</span></span> | <span data-ttu-id="2f506-127">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-127">Not supported</span></span> |
|<span data-ttu-id="2f506-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2f506-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2f506-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-129">Files.ReadWrite.All</span></span> | <span data-ttu-id="2f506-130">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-130">Not supported</span></span> | <span data-ttu-id="2f506-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-131">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f506-132">事件</span><span class="sxs-lookup"><span data-stu-id="2f506-132">event</span></span>](../resources/event.md) | <span data-ttu-id="2f506-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-133">Calendars.Read</span></span> | <span data-ttu-id="2f506-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-134">Calendars.Read</span></span> | <span data-ttu-id="2f506-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-135">Calendars.Read</span></span> |
|[<span data-ttu-id="2f506-136">组</span><span class="sxs-lookup"><span data-stu-id="2f506-136">group</span></span>](../resources/group.md) | <span data-ttu-id="2f506-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-137">Group.Read.All</span></span> | <span data-ttu-id="2f506-138">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-138">Not supported</span></span> | <span data-ttu-id="2f506-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-139">Group.Read.All</span></span> |
|[<span data-ttu-id="2f506-140">组对话</span><span class="sxs-lookup"><span data-stu-id="2f506-140">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2f506-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-141">Group.Read.All</span></span> | <span data-ttu-id="2f506-142">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-142">Not supported</span></span> | <span data-ttu-id="2f506-143">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-143">Not supported</span></span> |
|[<span data-ttu-id="2f506-144">列表</span><span class="sxs-lookup"><span data-stu-id="2f506-144">list</span></span>](../resources/list.md) | <span data-ttu-id="2f506-145">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-145">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2f506-146">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-146">Not supported</span></span> | <span data-ttu-id="2f506-147">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-147">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f506-148">邮件</span><span class="sxs-lookup"><span data-stu-id="2f506-148">message</span></span>](../resources/message.md) | <span data-ttu-id="2f506-149">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2f506-150">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-150">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2f506-151">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2f506-151">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="2f506-152">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="2f506-152">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="2f506-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-153">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2f506-154">不支持</span><span class="sxs-lookup"><span data-stu-id="2f506-154">Not supported</span></span> | <span data-ttu-id="2f506-155">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f506-155">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2f506-156">用户</span><span class="sxs-lookup"><span data-stu-id="2f506-156">user</span></span>](../resources/user.md) | <span data-ttu-id="2f506-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-157">User.Read.All</span></span> | <span data-ttu-id="2f506-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-158">User.Read.All</span></span> | <span data-ttu-id="2f506-159">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f506-159">User.Read.All</span></span> |

> <span data-ttu-id="2f506-160">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="2f506-160">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="2f506-161">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="2f506-161">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="2f506-162">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="2f506-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2f506-163">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="2f506-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2f506-164">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送变更通知。</span><span class="sxs-lookup"><span data-stu-id="2f506-164">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="2f506-165">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="2f506-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="2f506-166">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="2f506-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2f506-167">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="2f506-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="2f506-168">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="2f506-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2f506-169">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="2f506-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2f506-170">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="2f506-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="2f506-171">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f506-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2f506-172">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f506-172">Request headers</span></span>

| <span data-ttu-id="2f506-173">名称</span><span class="sxs-lookup"><span data-stu-id="2f506-173">Name</span></span>       | <span data-ttu-id="2f506-174">类型</span><span class="sxs-lookup"><span data-stu-id="2f506-174">Type</span></span> | <span data-ttu-id="2f506-175">说明</span><span class="sxs-lookup"><span data-stu-id="2f506-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f506-176">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f506-176">Authorization</span></span>  | <span data-ttu-id="2f506-177">string</span><span class="sxs-lookup"><span data-stu-id="2f506-177">string</span></span>  | <span data-ttu-id="2f506-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f506-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f506-180">响应</span><span class="sxs-lookup"><span data-stu-id="2f506-180">Response</span></span>

<span data-ttu-id="2f506-181">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f506-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="2f506-182">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="2f506-182">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="2f506-183">示例</span><span class="sxs-lookup"><span data-stu-id="2f506-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f506-184">请求</span><span class="sxs-lookup"><span data-stu-id="2f506-184">Request</span></span>

<span data-ttu-id="2f506-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f506-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f506-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f506-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="2f506-187">C#</span><span class="sxs-lookup"><span data-stu-id="2f506-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f506-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f506-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f506-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f506-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f506-190">Java</span><span class="sxs-lookup"><span data-stu-id="2f506-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f506-191">响应</span><span class="sxs-lookup"><span data-stu-id="2f506-191">Response</span></span>

<span data-ttu-id="2f506-192">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2f506-192">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

