---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0597ca754c04e684eeeca7f8e798904dea4df10c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603166"
---
# <a name="get-subscription"></a><span data-ttu-id="38322-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="38322-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38322-104">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38322-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="38322-105">权限</span><span class="sxs-lookup"><span data-stu-id="38322-105">Permissions</span></span>

<span data-ttu-id="38322-106">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="38322-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="38322-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38322-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38322-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="38322-108">Supported resource</span></span> | <span data-ttu-id="38322-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38322-109">Delegated (work or school account)</span></span> | <span data-ttu-id="38322-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38322-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38322-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="38322-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="38322-112">联系人</span><span class="sxs-lookup"><span data-stu-id="38322-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="38322-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="38322-113">Contacts.Read</span></span> | <span data-ttu-id="38322-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="38322-114">Contacts.Read</span></span> | <span data-ttu-id="38322-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="38322-115">Contacts.Read</span></span> |
|<span data-ttu-id="38322-116">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="38322-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="38322-117">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-117">Not supported</span></span> | <span data-ttu-id="38322-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38322-118">Files.ReadWrite</span></span> | <span data-ttu-id="38322-119">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-119">Not supported</span></span> |
|<span data-ttu-id="38322-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="38322-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="38322-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38322-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="38322-122">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-122">Not supported</span></span> | <span data-ttu-id="38322-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38322-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="38322-124">事件</span><span class="sxs-lookup"><span data-stu-id="38322-124">event</span></span>](../resources/event.md) | <span data-ttu-id="38322-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38322-125">Calendars.Read</span></span> | <span data-ttu-id="38322-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38322-126">Calendars.Read</span></span> | <span data-ttu-id="38322-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="38322-127">Calendars.Read</span></span> |
|[<span data-ttu-id="38322-128">组</span><span class="sxs-lookup"><span data-stu-id="38322-128">group</span></span>](../resources/group.md) | <span data-ttu-id="38322-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-129">Group.Read.All</span></span> | <span data-ttu-id="38322-130">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-130">Not supported</span></span> | <span data-ttu-id="38322-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-131">Group.Read.All</span></span> |
|[<span data-ttu-id="38322-132">组对话</span><span class="sxs-lookup"><span data-stu-id="38322-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="38322-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-133">Group.Read.All</span></span> | <span data-ttu-id="38322-134">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-134">Not supported</span></span> | <span data-ttu-id="38322-135">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-135">Not supported</span></span> |
|[<span data-ttu-id="38322-136">邮件</span><span class="sxs-lookup"><span data-stu-id="38322-136">message</span></span>](../resources/message.md) | <span data-ttu-id="38322-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="38322-137">Mail.Read</span></span> | <span data-ttu-id="38322-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="38322-138">Mail.Read</span></span> | <span data-ttu-id="38322-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="38322-139">Mail.Read</span></span> |
|<span data-ttu-id="38322-140">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="38322-140">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="38322-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38322-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="38322-142">不支持</span><span class="sxs-lookup"><span data-stu-id="38322-142">Not supported</span></span> | <span data-ttu-id="38322-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38322-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="38322-144">用户</span><span class="sxs-lookup"><span data-stu-id="38322-144">user</span></span>](../resources/user.md) | <span data-ttu-id="38322-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-145">User.Read.All</span></span> | <span data-ttu-id="38322-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-146">User.Read.All</span></span> | <span data-ttu-id="38322-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="38322-147">User.Read.All</span></span> |

> <span data-ttu-id="38322-148">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="38322-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="38322-149">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="38322-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="38322-150">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="38322-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="38322-151">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="38322-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="38322-152">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="38322-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="38322-153">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="38322-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="38322-154">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="38322-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="38322-155">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="38322-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="38322-156">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="38322-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="38322-157">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="38322-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="38322-158">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="38322-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="38322-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38322-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38322-160">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38322-160">Optional query parameters</span></span>

<span data-ttu-id="38322-161">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38322-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38322-162">请求标头</span><span class="sxs-lookup"><span data-stu-id="38322-162">Request headers</span></span>

| <span data-ttu-id="38322-163">名称</span><span class="sxs-lookup"><span data-stu-id="38322-163">Name</span></span>       | <span data-ttu-id="38322-164">类型</span><span class="sxs-lookup"><span data-stu-id="38322-164">Type</span></span> | <span data-ttu-id="38322-165">说明</span><span class="sxs-lookup"><span data-stu-id="38322-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="38322-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="38322-166">Authorization</span></span>  | <span data-ttu-id="38322-167">string</span><span class="sxs-lookup"><span data-stu-id="38322-167">string</span></span>  | <span data-ttu-id="38322-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38322-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38322-170">请求正文</span><span class="sxs-lookup"><span data-stu-id="38322-170">Request body</span></span>

<span data-ttu-id="38322-171">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38322-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38322-172">响应</span><span class="sxs-lookup"><span data-stu-id="38322-172">Response</span></span>

<span data-ttu-id="38322-173">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38322-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38322-174">示例</span><span class="sxs-lookup"><span data-stu-id="38322-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38322-175">请求</span><span class="sxs-lookup"><span data-stu-id="38322-175">Request</span></span>

<span data-ttu-id="38322-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38322-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="38322-177">响应</span><span class="sxs-lookup"><span data-stu-id="38322-177">Response</span></span>

<span data-ttu-id="38322-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="38322-178">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38322-179">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="38322-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38322-180">C#</span><span class="sxs-lookup"><span data-stu-id="38322-180">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscription-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38322-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="38322-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscription-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
