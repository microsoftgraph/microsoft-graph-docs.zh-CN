---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 30f9666f7418a116d9c18960da066954a93226cc
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598477"
---
# <a name="get-subscription"></a><span data-ttu-id="4478e-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="4478e-103">Get subscription</span></span>

<span data-ttu-id="4478e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4478e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4478e-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4478e-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4478e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4478e-106">Permissions</span></span>

<span data-ttu-id="4478e-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="4478e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4478e-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4478e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4478e-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="4478e-109">Supported resource</span></span> | <span data-ttu-id="4478e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4478e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4478e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4478e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4478e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4478e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4478e-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="4478e-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="4478e-114">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-114">Not supported</span></span> | <span data-ttu-id="4478e-115">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-115">Not supported</span></span> | <span data-ttu-id="4478e-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-116">CallRecords.Read.All</span></span> |
|[<span data-ttu-id="4478e-117">联系人</span><span class="sxs-lookup"><span data-stu-id="4478e-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4478e-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-118">Contacts.Read</span></span> | <span data-ttu-id="4478e-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-119">Contacts.Read</span></span> | <span data-ttu-id="4478e-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-120">Contacts.Read</span></span> |
|<span data-ttu-id="4478e-121">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="4478e-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4478e-122">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-122">Not supported</span></span> | <span data-ttu-id="4478e-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4478e-123">Files.ReadWrite</span></span> | <span data-ttu-id="4478e-124">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-124">Not supported</span></span> |
|<span data-ttu-id="4478e-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="4478e-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4478e-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="4478e-127">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-127">Not supported</span></span> | <span data-ttu-id="4478e-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4478e-129">事件</span><span class="sxs-lookup"><span data-stu-id="4478e-129">event</span></span>](../resources/event.md) | <span data-ttu-id="4478e-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-130">Calendars.Read</span></span> | <span data-ttu-id="4478e-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-131">Calendars.Read</span></span> | <span data-ttu-id="4478e-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-132">Calendars.Read</span></span> |
|[<span data-ttu-id="4478e-133">组</span><span class="sxs-lookup"><span data-stu-id="4478e-133">group</span></span>](../resources/group.md) | <span data-ttu-id="4478e-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-134">Group.Read.All</span></span> | <span data-ttu-id="4478e-135">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-135">Not supported</span></span> | <span data-ttu-id="4478e-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-136">Group.Read.All</span></span> |
|[<span data-ttu-id="4478e-137">组对话</span><span class="sxs-lookup"><span data-stu-id="4478e-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4478e-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-138">Group.Read.All</span></span> | <span data-ttu-id="4478e-139">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-139">Not supported</span></span> | <span data-ttu-id="4478e-140">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-140">Not supported</span></span> |
|[<span data-ttu-id="4478e-141">列表</span><span class="sxs-lookup"><span data-stu-id="4478e-141">list</span></span>](../resources/list.md) | <span data-ttu-id="4478e-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="4478e-143">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-143">Not supported</span></span> | <span data-ttu-id="4478e-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="4478e-145">邮件</span><span class="sxs-lookup"><span data-stu-id="4478e-145">message</span></span>](../resources/message.md) | <span data-ttu-id="4478e-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4478e-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4478e-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4478e-148">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="4478e-149">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="4478e-149">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="4478e-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4478e-151">不支持</span><span class="sxs-lookup"><span data-stu-id="4478e-151">Not supported</span></span> | <span data-ttu-id="4478e-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4478e-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4478e-153">用户</span><span class="sxs-lookup"><span data-stu-id="4478e-153">user</span></span>](../resources/user.md) | <span data-ttu-id="4478e-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-154">User.Read.All</span></span> | <span data-ttu-id="4478e-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-155">User.Read.All</span></span> | <span data-ttu-id="4478e-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4478e-156">User.Read.All</span></span> |

> <span data-ttu-id="4478e-157">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="4478e-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="4478e-158">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="4478e-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="4478e-159">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="4478e-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4478e-160">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="4478e-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4478e-161">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送变更通知。</span><span class="sxs-lookup"><span data-stu-id="4478e-161">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="4478e-162">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="4478e-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="4478e-163">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="4478e-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4478e-164">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="4478e-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="4478e-165">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="4478e-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4478e-166">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="4478e-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4478e-167">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="4478e-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="4478e-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4478e-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4478e-169">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4478e-169">Optional query parameters</span></span>

<span data-ttu-id="4478e-170">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4478e-170">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4478e-171">请求标头</span><span class="sxs-lookup"><span data-stu-id="4478e-171">Request headers</span></span>

| <span data-ttu-id="4478e-172">名称</span><span class="sxs-lookup"><span data-stu-id="4478e-172">Name</span></span>       | <span data-ttu-id="4478e-173">类型</span><span class="sxs-lookup"><span data-stu-id="4478e-173">Type</span></span> | <span data-ttu-id="4478e-174">说明</span><span class="sxs-lookup"><span data-stu-id="4478e-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4478e-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="4478e-175">Authorization</span></span>  | <span data-ttu-id="4478e-176">string</span><span class="sxs-lookup"><span data-stu-id="4478e-176">string</span></span>  | <span data-ttu-id="4478e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4478e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4478e-179">请求正文</span><span class="sxs-lookup"><span data-stu-id="4478e-179">Request body</span></span>

<span data-ttu-id="4478e-180">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4478e-180">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4478e-181">响应</span><span class="sxs-lookup"><span data-stu-id="4478e-181">Response</span></span>

<span data-ttu-id="4478e-182">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4478e-182">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4478e-183">示例</span><span class="sxs-lookup"><span data-stu-id="4478e-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4478e-184">请求</span><span class="sxs-lookup"><span data-stu-id="4478e-184">Request</span></span>

<span data-ttu-id="4478e-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4478e-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4478e-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="4478e-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="4478e-187">C#</span><span class="sxs-lookup"><span data-stu-id="4478e-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4478e-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4478e-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4478e-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4478e-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4478e-190">Java</span><span class="sxs-lookup"><span data-stu-id="4478e-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4478e-191">响应</span><span class="sxs-lookup"><span data-stu-id="4478e-191">Response</span></span>

<span data-ttu-id="4478e-192">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4478e-192">Here is an example of the response.</span></span>
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
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
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
