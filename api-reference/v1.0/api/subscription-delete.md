---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c75f83edcf509f621539a51c4938621d708b3d12
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345868"
---
# <a name="delete-subscription"></a><span data-ttu-id="6ac0e-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="6ac0e-103">Delete subscription</span></span>

<span data-ttu-id="6ac0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ac0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ac0e-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ac0e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ac0e-106">Permissions</span></span>

<span data-ttu-id="6ac0e-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6ac0e-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ac0e-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="6ac0e-109">Supported resource</span></span> | <span data-ttu-id="6ac0e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ac0e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ac0e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ac0e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ac0e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6ac0e-113">联系人</span><span class="sxs-lookup"><span data-stu-id="6ac0e-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6ac0e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-114">Contacts.Read</span></span> | <span data-ttu-id="6ac0e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-115">Contacts.Read</span></span> | <span data-ttu-id="6ac0e-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-116">Contacts.Read</span></span> |
|<span data-ttu-id="6ac0e-117">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="6ac0e-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6ac0e-118">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-118">Not supported</span></span> | <span data-ttu-id="6ac0e-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ac0e-119">Files.ReadWrite</span></span> | <span data-ttu-id="6ac0e-120">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-120">Not supported</span></span> |
|<span data-ttu-id="6ac0e-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6ac0e-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6ac0e-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="6ac0e-123">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-123">Not supported</span></span> | <span data-ttu-id="6ac0e-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6ac0e-125">事件</span><span class="sxs-lookup"><span data-stu-id="6ac0e-125">event</span></span>](../resources/event.md) | <span data-ttu-id="6ac0e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-126">Calendars.Read</span></span> | <span data-ttu-id="6ac0e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-127">Calendars.Read</span></span> | <span data-ttu-id="6ac0e-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-128">Calendars.Read</span></span> |
|[<span data-ttu-id="6ac0e-129">组</span><span class="sxs-lookup"><span data-stu-id="6ac0e-129">group</span></span>](../resources/group.md) | <span data-ttu-id="6ac0e-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-130">Group.Read.All</span></span> | <span data-ttu-id="6ac0e-131">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-131">Not supported</span></span> | <span data-ttu-id="6ac0e-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-132">Group.Read.All</span></span> |
|[<span data-ttu-id="6ac0e-133">组对话</span><span class="sxs-lookup"><span data-stu-id="6ac0e-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6ac0e-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-134">Group.Read.All</span></span> | <span data-ttu-id="6ac0e-135">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-135">Not supported</span></span> | <span data-ttu-id="6ac0e-136">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-136">Not supported</span></span> |
|[<span data-ttu-id="6ac0e-137">列表</span><span class="sxs-lookup"><span data-stu-id="6ac0e-137">list</span></span>](../resources/list.md) | <span data-ttu-id="6ac0e-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6ac0e-139">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-139">Not supported</span></span> | <span data-ttu-id="6ac0e-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6ac0e-141">邮件</span><span class="sxs-lookup"><span data-stu-id="6ac0e-141">message</span></span>](../resources/message.md) | <span data-ttu-id="6ac0e-142">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6ac0e-143">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6ac0e-144">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6ac0e-144">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="6ac0e-145">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="6ac0e-145">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="6ac0e-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6ac0e-147">不支持</span><span class="sxs-lookup"><span data-stu-id="6ac0e-147">Not supported</span></span> | <span data-ttu-id="6ac0e-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6ac0e-149">用户</span><span class="sxs-lookup"><span data-stu-id="6ac0e-149">user</span></span>](../resources/user.md) | <span data-ttu-id="6ac0e-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-150">User.Read.All</span></span> | <span data-ttu-id="6ac0e-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-151">User.Read.All</span></span> | <span data-ttu-id="6ac0e-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ac0e-152">User.Read.All</span></span> |

> <span data-ttu-id="6ac0e-153">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="6ac0e-154">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="6ac0e-155">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6ac0e-156">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6ac0e-157">将为订阅的文件夹中的所请求类型的更改发送更改通知，或在其层次结构中的任何文件、文件夹或其他 driveItem 对象上发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-157">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="6ac0e-158">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="6ac0e-159">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6ac0e-160">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="6ac0e-161">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="6ac0e-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6ac0e-162">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6ac0e-163">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="6ac0e-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ac0e-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6ac0e-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ac0e-165">Request headers</span></span>

| <span data-ttu-id="6ac0e-166">名称</span><span class="sxs-lookup"><span data-stu-id="6ac0e-166">Name</span></span>       | <span data-ttu-id="6ac0e-167">类型</span><span class="sxs-lookup"><span data-stu-id="6ac0e-167">Type</span></span> | <span data-ttu-id="6ac0e-168">说明</span><span class="sxs-lookup"><span data-stu-id="6ac0e-168">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ac0e-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ac0e-169">Authorization</span></span>  | <span data-ttu-id="6ac0e-170">string</span><span class="sxs-lookup"><span data-stu-id="6ac0e-170">string</span></span>  | <span data-ttu-id="6ac0e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ac0e-173">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ac0e-173">Request body</span></span>

<span data-ttu-id="6ac0e-174">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ac0e-175">响应</span><span class="sxs-lookup"><span data-stu-id="6ac0e-175">Response</span></span>

<span data-ttu-id="6ac0e-176">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-176">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ac0e-177">示例</span><span class="sxs-lookup"><span data-stu-id="6ac0e-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6ac0e-178">请求</span><span class="sxs-lookup"><span data-stu-id="6ac0e-178">Request</span></span>

<span data-ttu-id="6ac0e-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ac0e-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ac0e-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="6ac0e-181">C#</span><span class="sxs-lookup"><span data-stu-id="6ac0e-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ac0e-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ac0e-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ac0e-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ac0e-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ac0e-184">Java</span><span class="sxs-lookup"><span data-stu-id="6ac0e-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6ac0e-185">响应</span><span class="sxs-lookup"><span data-stu-id="6ac0e-185">Response</span></span>

<span data-ttu-id="6ac0e-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6ac0e-186">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
