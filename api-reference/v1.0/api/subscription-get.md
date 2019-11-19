---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fdd850b5965e20b4de2602368c3ece3fe47b65b5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703803"
---
# <a name="get-subscription"></a><span data-ttu-id="5809c-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="5809c-103">Get subscription</span></span>

<span data-ttu-id="5809c-104">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5809c-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="5809c-105">权限</span><span class="sxs-lookup"><span data-stu-id="5809c-105">Permissions</span></span>

<span data-ttu-id="5809c-106">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="5809c-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5809c-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5809c-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5809c-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="5809c-108">Supported resource</span></span> | <span data-ttu-id="5809c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5809c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5809c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5809c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5809c-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="5809c-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="5809c-112">联系人</span><span class="sxs-lookup"><span data-stu-id="5809c-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5809c-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-113">Contacts.Read</span></span> | <span data-ttu-id="5809c-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-114">Contacts.Read</span></span> | <span data-ttu-id="5809c-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-115">Contacts.Read</span></span> |
|<span data-ttu-id="5809c-116">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="5809c-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5809c-117">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-117">Not supported</span></span> | <span data-ttu-id="5809c-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5809c-118">Files.ReadWrite</span></span> | <span data-ttu-id="5809c-119">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-119">Not supported</span></span> |
|<span data-ttu-id="5809c-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="5809c-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5809c-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5809c-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="5809c-122">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-122">Not supported</span></span> | <span data-ttu-id="5809c-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5809c-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5809c-124">事件</span><span class="sxs-lookup"><span data-stu-id="5809c-124">event</span></span>](../resources/event.md) | <span data-ttu-id="5809c-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-125">Calendars.Read</span></span> | <span data-ttu-id="5809c-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-126">Calendars.Read</span></span> | <span data-ttu-id="5809c-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-127">Calendars.Read</span></span> |
|[<span data-ttu-id="5809c-128">组</span><span class="sxs-lookup"><span data-stu-id="5809c-128">group</span></span>](../resources/group.md) | <span data-ttu-id="5809c-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-129">Group.Read.All</span></span> | <span data-ttu-id="5809c-130">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-130">Not supported</span></span> | <span data-ttu-id="5809c-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-131">Group.Read.All</span></span> |
|[<span data-ttu-id="5809c-132">组对话</span><span class="sxs-lookup"><span data-stu-id="5809c-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5809c-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-133">Group.Read.All</span></span> | <span data-ttu-id="5809c-134">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-134">Not supported</span></span> | <span data-ttu-id="5809c-135">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-135">Not supported</span></span> |
|[<span data-ttu-id="5809c-136">邮件</span><span class="sxs-lookup"><span data-stu-id="5809c-136">message</span></span>](../resources/message.md) | <span data-ttu-id="5809c-137">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-137">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5809c-138">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5809c-139">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5809c-139">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="5809c-140">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="5809c-140">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="5809c-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5809c-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5809c-142">不支持</span><span class="sxs-lookup"><span data-stu-id="5809c-142">Not supported</span></span> | <span data-ttu-id="5809c-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5809c-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5809c-144">用户</span><span class="sxs-lookup"><span data-stu-id="5809c-144">user</span></span>](../resources/user.md) | <span data-ttu-id="5809c-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-145">User.Read.All</span></span> | <span data-ttu-id="5809c-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-146">User.Read.All</span></span> | <span data-ttu-id="5809c-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809c-147">User.Read.All</span></span> |

> <span data-ttu-id="5809c-148">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="5809c-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="5809c-149">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="5809c-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="5809c-150">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="5809c-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5809c-151">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="5809c-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5809c-152">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="5809c-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="5809c-153">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="5809c-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="5809c-154">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="5809c-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5809c-155">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="5809c-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5809c-156">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="5809c-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5809c-157">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="5809c-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5809c-158">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="5809c-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="5809c-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5809c-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5809c-160">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5809c-160">Optional query parameters</span></span>

<span data-ttu-id="5809c-161">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5809c-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5809c-162">请求标头</span><span class="sxs-lookup"><span data-stu-id="5809c-162">Request headers</span></span>

| <span data-ttu-id="5809c-163">名称</span><span class="sxs-lookup"><span data-stu-id="5809c-163">Name</span></span>       | <span data-ttu-id="5809c-164">类型</span><span class="sxs-lookup"><span data-stu-id="5809c-164">Type</span></span> | <span data-ttu-id="5809c-165">说明</span><span class="sxs-lookup"><span data-stu-id="5809c-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5809c-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="5809c-166">Authorization</span></span>  | <span data-ttu-id="5809c-167">string</span><span class="sxs-lookup"><span data-stu-id="5809c-167">string</span></span>  | <span data-ttu-id="5809c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5809c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5809c-170">请求正文</span><span class="sxs-lookup"><span data-stu-id="5809c-170">Request body</span></span>

<span data-ttu-id="5809c-171">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5809c-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5809c-172">响应</span><span class="sxs-lookup"><span data-stu-id="5809c-172">Response</span></span>

<span data-ttu-id="5809c-173">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5809c-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5809c-174">示例</span><span class="sxs-lookup"><span data-stu-id="5809c-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5809c-175">请求</span><span class="sxs-lookup"><span data-stu-id="5809c-175">Request</span></span>

<span data-ttu-id="5809c-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5809c-176">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5809c-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="5809c-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5809c-178">C#</span><span class="sxs-lookup"><span data-stu-id="5809c-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5809c-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5809c-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5809c-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5809c-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5809c-181">Java</span><span class="sxs-lookup"><span data-stu-id="5809c-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5809c-182">响应</span><span class="sxs-lookup"><span data-stu-id="5809c-182">Response</span></span>

<span data-ttu-id="5809c-183">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5809c-183">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
