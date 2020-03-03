---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4063be8500e67d4630e10d027359774612c0613a
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394445"
---
# <a name="get-subscription"></a><span data-ttu-id="98382-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="98382-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98382-104">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98382-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="98382-105">权限</span><span class="sxs-lookup"><span data-stu-id="98382-105">Permissions</span></span>

<span data-ttu-id="98382-106">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="98382-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="98382-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98382-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98382-108">支持的资源</span><span class="sxs-lookup"><span data-stu-id="98382-108">Supported resource</span></span> | <span data-ttu-id="98382-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98382-109">Delegated (work or school account)</span></span> | <span data-ttu-id="98382-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98382-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98382-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="98382-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="98382-112">callRecord</span><span class="sxs-lookup"><span data-stu-id="98382-112">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="98382-113">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-113">Not supported</span></span> | <span data-ttu-id="98382-114">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-114">Not supported</span></span> | <span data-ttu-id="98382-115">CallRecords</span><span class="sxs-lookup"><span data-stu-id="98382-115">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="98382-116">联系人</span><span class="sxs-lookup"><span data-stu-id="98382-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="98382-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98382-117">Contacts.Read</span></span> | <span data-ttu-id="98382-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98382-118">Contacts.Read</span></span> | <span data-ttu-id="98382-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98382-119">Contacts.Read</span></span> |
|<span data-ttu-id="98382-120">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="98382-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="98382-121">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-121">Not supported</span></span> | <span data-ttu-id="98382-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98382-122">Files.ReadWrite</span></span> | <span data-ttu-id="98382-123">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-123">Not supported</span></span> |
|<span data-ttu-id="98382-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="98382-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="98382-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="98382-126">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-126">Not supported</span></span> | <span data-ttu-id="98382-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="98382-128">事件</span><span class="sxs-lookup"><span data-stu-id="98382-128">event</span></span>](../resources/event.md) | <span data-ttu-id="98382-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98382-129">Calendars.Read</span></span> | <span data-ttu-id="98382-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98382-130">Calendars.Read</span></span> | <span data-ttu-id="98382-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98382-131">Calendars.Read</span></span> |
|[<span data-ttu-id="98382-132">组</span><span class="sxs-lookup"><span data-stu-id="98382-132">group</span></span>](../resources/group.md) | <span data-ttu-id="98382-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-133">Group.Read.All</span></span> | <span data-ttu-id="98382-134">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-134">Not supported</span></span> | <span data-ttu-id="98382-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-135">Group.Read.All</span></span> |
|[<span data-ttu-id="98382-136">组对话</span><span class="sxs-lookup"><span data-stu-id="98382-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="98382-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-137">Group.Read.All</span></span> | <span data-ttu-id="98382-138">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-138">Not supported</span></span> | <span data-ttu-id="98382-139">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-139">Not supported</span></span> |
|[<span data-ttu-id="98382-140">list</span><span class="sxs-lookup"><span data-stu-id="98382-140">list</span></span>](../resources/list.md) | <span data-ttu-id="98382-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="98382-142">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-142">Not supported</span></span> | <span data-ttu-id="98382-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="98382-144">邮件</span><span class="sxs-lookup"><span data-stu-id="98382-144">message</span></span>](../resources/message.md) | <span data-ttu-id="98382-145">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98382-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="98382-146">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98382-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="98382-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98382-147">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="98382-148">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="98382-148">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="98382-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="98382-150">不支持</span><span class="sxs-lookup"><span data-stu-id="98382-150">Not supported</span></span> | <span data-ttu-id="98382-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98382-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="98382-152">用户</span><span class="sxs-lookup"><span data-stu-id="98382-152">user</span></span>](../resources/user.md) | <span data-ttu-id="98382-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-153">User.Read.All</span></span> | <span data-ttu-id="98382-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-154">User.Read.All</span></span> | <span data-ttu-id="98382-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="98382-155">User.Read.All</span></span> |

> <span data-ttu-id="98382-156">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="98382-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="98382-157">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="98382-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="98382-158">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="98382-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="98382-159">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="98382-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="98382-160">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 driveItem 对象所做更改属于请求的更改类型时，会发送通知。</span><span class="sxs-lookup"><span data-stu-id="98382-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="98382-161">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="98382-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="98382-162">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="98382-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="98382-163">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="98382-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="98382-164">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="98382-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="98382-165">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="98382-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="98382-166">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="98382-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="98382-167">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98382-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98382-168">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98382-168">Optional query parameters</span></span>

<span data-ttu-id="98382-169">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98382-169">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98382-170">请求标头</span><span class="sxs-lookup"><span data-stu-id="98382-170">Request headers</span></span>

| <span data-ttu-id="98382-171">名称</span><span class="sxs-lookup"><span data-stu-id="98382-171">Name</span></span>       | <span data-ttu-id="98382-172">类型</span><span class="sxs-lookup"><span data-stu-id="98382-172">Type</span></span> | <span data-ttu-id="98382-173">说明</span><span class="sxs-lookup"><span data-stu-id="98382-173">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="98382-174">Authorization</span><span class="sxs-lookup"><span data-stu-id="98382-174">Authorization</span></span>  | <span data-ttu-id="98382-175">string</span><span class="sxs-lookup"><span data-stu-id="98382-175">string</span></span>  | <span data-ttu-id="98382-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98382-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98382-178">请求正文</span><span class="sxs-lookup"><span data-stu-id="98382-178">Request body</span></span>

<span data-ttu-id="98382-179">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98382-179">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98382-180">响应</span><span class="sxs-lookup"><span data-stu-id="98382-180">Response</span></span>

<span data-ttu-id="98382-181">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98382-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98382-182">示例</span><span class="sxs-lookup"><span data-stu-id="98382-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98382-183">请求</span><span class="sxs-lookup"><span data-stu-id="98382-183">Request</span></span>

<span data-ttu-id="98382-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98382-184">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98382-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="98382-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="98382-186">C#</span><span class="sxs-lookup"><span data-stu-id="98382-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98382-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98382-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98382-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98382-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98382-189">响应</span><span class="sxs-lookup"><span data-stu-id="98382-189">Response</span></span>

<span data-ttu-id="98382-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="98382-190">Here is an example of the response.</span></span>
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
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
}
```

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
  ]
}
-->
