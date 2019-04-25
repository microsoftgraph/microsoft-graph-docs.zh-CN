---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e868489ca5eb95cdc2ee8c33176c8da20271bd12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537095"
---
# <a name="update-subscription"></a><span data-ttu-id="95b69-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="95b69-103">Update subscription</span></span>

<span data-ttu-id="95b69-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="95b69-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="95b69-105">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="95b69-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="95b69-106">为了避免丢失通知, 应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="95b69-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="95b69-107">有关每种资源类型的最大订阅长度, 请参阅[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="95b69-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="95b69-108">权限</span><span class="sxs-lookup"><span data-stu-id="95b69-108">Permissions</span></span>

<span data-ttu-id="95b69-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="95b69-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="95b69-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95b69-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95b69-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="95b69-111">Supported resource</span></span> | <span data-ttu-id="95b69-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95b69-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95b69-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95b69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95b69-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="95b69-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="95b69-115">联系人</span><span class="sxs-lookup"><span data-stu-id="95b69-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="95b69-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-116">Contacts.Read</span></span> | <span data-ttu-id="95b69-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-117">Contacts.Read</span></span> | <span data-ttu-id="95b69-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-118">Contacts.Read</span></span> |
|<span data-ttu-id="95b69-119">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="95b69-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="95b69-120">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-120">Not supported</span></span> | <span data-ttu-id="95b69-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95b69-121">Files.ReadWrite</span></span> | <span data-ttu-id="95b69-122">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-122">Not supported</span></span> |
|<span data-ttu-id="95b69-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="95b69-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="95b69-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b69-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="95b69-125">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-125">Not supported</span></span> | <span data-ttu-id="95b69-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b69-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="95b69-127">event</span><span class="sxs-lookup"><span data-stu-id="95b69-127">event</span></span>](../resources/event.md) | <span data-ttu-id="95b69-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-128">Calendars.Read</span></span> | <span data-ttu-id="95b69-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-129">Calendars.Read</span></span> | <span data-ttu-id="95b69-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-130">Calendars.Read</span></span> |
|[<span data-ttu-id="95b69-131">组</span><span class="sxs-lookup"><span data-stu-id="95b69-131">group</span></span>](../resources/group.md) | <span data-ttu-id="95b69-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-132">Group.Read.All</span></span> | <span data-ttu-id="95b69-133">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-133">Not supported</span></span> | <span data-ttu-id="95b69-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-134">Group.Read.All</span></span> |
|[<span data-ttu-id="95b69-135">组对话</span><span class="sxs-lookup"><span data-stu-id="95b69-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="95b69-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-136">Group.Read.All</span></span> | <span data-ttu-id="95b69-137">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-137">Not supported</span></span> | <span data-ttu-id="95b69-138">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-138">Not supported</span></span> |
|[<span data-ttu-id="95b69-139">message</span><span class="sxs-lookup"><span data-stu-id="95b69-139">message</span></span>](../resources/message.md) | <span data-ttu-id="95b69-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-140">Mail.Read</span></span> | <span data-ttu-id="95b69-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-141">Mail.Read</span></span> | <span data-ttu-id="95b69-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="95b69-142">Mail.Read</span></span> |
|<span data-ttu-id="95b69-143">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="95b69-143">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="95b69-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b69-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="95b69-145">不支持</span><span class="sxs-lookup"><span data-stu-id="95b69-145">Not supported</span></span> | <span data-ttu-id="95b69-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b69-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="95b69-147">用户</span><span class="sxs-lookup"><span data-stu-id="95b69-147">user</span></span>](../resources/user.md) | <span data-ttu-id="95b69-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-148">User.Read.All</span></span> | <span data-ttu-id="95b69-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-149">User.Read.All</span></span> | <span data-ttu-id="95b69-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="95b69-150">User.Read.All</span></span> |

> <span data-ttu-id="95b69-151">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="95b69-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="95b69-152">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="95b69-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="95b69-153">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="95b69-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="95b69-154">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="95b69-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="95b69-155">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="95b69-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="95b69-156">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="95b69-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="95b69-157">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="95b69-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="95b69-158">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="95b69-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="95b69-159">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="95b69-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="95b69-160">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="95b69-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="95b69-161">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="95b69-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="95b69-162">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95b69-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95b69-163">请求标头</span><span class="sxs-lookup"><span data-stu-id="95b69-163">Request headers</span></span>

| <span data-ttu-id="95b69-164">名称</span><span class="sxs-lookup"><span data-stu-id="95b69-164">Name</span></span>       | <span data-ttu-id="95b69-165">类型</span><span class="sxs-lookup"><span data-stu-id="95b69-165">Type</span></span> | <span data-ttu-id="95b69-166">说明</span><span class="sxs-lookup"><span data-stu-id="95b69-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="95b69-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="95b69-167">Authorization</span></span>  | <span data-ttu-id="95b69-168">string</span><span class="sxs-lookup"><span data-stu-id="95b69-168">string</span></span>  | <span data-ttu-id="95b69-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95b69-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="95b69-171">响应</span><span class="sxs-lookup"><span data-stu-id="95b69-171">Response</span></span>

<span data-ttu-id="95b69-172">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95b69-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b69-173">示例</span><span class="sxs-lookup"><span data-stu-id="95b69-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95b69-174">请求</span><span class="sxs-lookup"><span data-stu-id="95b69-174">Request</span></span>

<span data-ttu-id="95b69-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95b69-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="95b69-176">响应</span><span class="sxs-lookup"><span data-stu-id="95b69-176">Response</span></span>

<span data-ttu-id="95b69-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="95b69-177">Here is an example of the response.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
