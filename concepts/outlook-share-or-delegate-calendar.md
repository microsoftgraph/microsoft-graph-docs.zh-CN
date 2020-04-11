---
title: 在 Outlook 中共享或委派日历
description: 在 Outlook 中，日历所有者可与其他用户共享日历，或委派其他用户来管理所有者主要日历中的会议。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 7654928f0fab1080f7f85eee48186964957224dc
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229421"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a><span data-ttu-id="0575c-103">在 Outlook 中共享或委派日历</span><span class="sxs-lookup"><span data-stu-id="0575c-103">Share or delegate a calendar in Outlook</span></span>

<span data-ttu-id="0575c-104">在 Outlook 中，日历所有者可与其他用户共享日历。</span><span class="sxs-lookup"><span data-stu-id="0575c-104">In Outlook, a calendar owner can share the calendar with another user.</span></span> <span data-ttu-id="0575c-105">所有者可以指定非私人活动中的哪些信息是可供查看的，并且可向同一组织中的用户授予对日历的写入访问权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-105">The owner can specify which information in non-private events is viewable, and can give write access to the calendar to users in the same organization.</span></span> 

<span data-ttu-id="0575c-106">所有者还可以委派其他用户来管理所有者_主要_日历中的会议。</span><span class="sxs-lookup"><span data-stu-id="0575c-106">The owner can also delegate another user to manage meetings in the owner's _primary_ calendar.</span></span> <span data-ttu-id="0575c-107">委托人是指可以查看所有信息并对非私人活动具有写入访问权限的共享者。</span><span class="sxs-lookup"><span data-stu-id="0575c-107">Delegates are sharees who can view all information in and have write access to non-private events.</span></span> <span data-ttu-id="0575c-108">他们还会收到会议请求和响应，并代表所有者响应会议请求。</span><span class="sxs-lookup"><span data-stu-id="0575c-108">They also receive meeting requests and responses, and respond to meeting requests on behalf of the owner.</span></span> <span data-ttu-id="0575c-109">此外，所有者可以向委托人授予在日历上查看所有者的_私人_活动的显式权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-109">Additionally, the owner can give explicit permissions to delegates to view the owner's _private_ events on the calendar.</span></span> 

<span data-ttu-id="0575c-110">在日历共享或委派生效之前，所有者将向共享者或委托人发送邀请，共享者或委托人需要接受邀请，所有者也可以显式添加共享或委派日历以供访问。</span><span class="sxs-lookup"><span data-stu-id="0575c-110">Before calendar sharing or delegation can take effect, the owner sends a sharee or delegate an invitation, and the sharee or delegate accepts the invitation, or, explicitly adds the shared or delegated calendar for access.</span></span> <span data-ttu-id="0575c-111">可在 Outlook 客户端中进行邀请和添加共享或委派日历。</span><span class="sxs-lookup"><span data-stu-id="0575c-111">The invitation and adding a shared or delegated calendar occur in an Outlook client.</span></span> 

<span data-ttu-id="0575c-112">在 Outlook 中设置共享或委派后，应用可使用 Microsoft Graph API 管理共享和委派。</span><span class="sxs-lookup"><span data-stu-id="0575c-112">After sharing or delegation is set up in Outlook, apps can then use the Microsoft Graph API to manage the sharing and delegation.</span></span>

<span data-ttu-id="0575c-113">本文的其余部分基于以下示例方案：</span><span class="sxs-lookup"><span data-stu-id="0575c-113">The rest of this article is based on the following example scenario:</span></span>

- <span data-ttu-id="0575c-114">Alex Wilber 已将 Megan Bowen 委派到其主要日历，并且还允许 Megan 查看该日历中的私人活动。</span><span class="sxs-lookup"><span data-stu-id="0575c-114">Alex Wilber has delegated Megan Bowen to his primary calendar, and also permitted Megan to view private events in that calendar.</span></span> 
- <span data-ttu-id="0575c-115">Alex 与 Adele Vance 和 Megan Bowen 共享了一个“儿童派对”日历，并向 Adele 和 Megan 授予了`read`权限，允许他们查看“儿童派对”日历上的非私人活动的所有详细信息，以及私人活动的忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="0575c-115">Alex shared a "Kids parties" calendar with Adele Vance and Megan Bowen, and gave both Adele and Megan `read` permissions to all the details of non-private events on the "Kids parties" calendar, and free/busy status for private events.</span></span> 

<span data-ttu-id="0575c-116">本文介绍如何使用共享或委派日历以编程方式执行以下任务：</span><span class="sxs-lookup"><span data-stu-id="0575c-116">This article describes programmatically carrying out the following tasks with a shared or delegated calendar:</span></span>

- <span data-ttu-id="0575c-117">[获取有关共享者、委托人和允许的权限的日历信息，以及更新各个权限](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions)。</span><span class="sxs-lookup"><span data-stu-id="0575c-117">[Get calendar information about sharees, delegates, and allowed permissions, and update individual permissions](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).</span></span>
- <span data-ttu-id="0575c-118">[获取用于描述日历的共享或委派的属性](#get-properties-of-a-shared-or-delegated-calendar)。</span><span class="sxs-lookup"><span data-stu-id="0575c-118">[Get the properties that describe the sharing or delegation of the calendar](#get-properties-of-a-shared-or-delegated-calendar).</span></span>
- <span data-ttu-id="0575c-119">[获取或设置邮箱设置以接收委派日历的会议请求和响应](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses)。</span><span class="sxs-lookup"><span data-stu-id="0575c-119">[Get or set mailbox setting to receive meeting requests and responses for a delegated calendar](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).</span></span>
- <span data-ttu-id="0575c-120">[删除日历的共享者或委托人](#delete-a-sharee-or-delegate-of-a-calendar)。</span><span class="sxs-lookup"><span data-stu-id="0575c-120">[Delete a sharee or delegate of a calendar](#delete-a-sharee-or-delegate-of-a-calendar).</span></span>

<span data-ttu-id="0575c-121">应用还可以使用通用版 API 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0575c-121">Apps can also do the following using API that is generally available:</span></span>

- [<span data-ttu-id="0575c-122">获取共享或委托 Outlook 日历或其活动</span><span class="sxs-lookup"><span data-stu-id="0575c-122">Get shared or delegated Outlook calendar or its events</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="0575c-123">在共享或委托日历中创建 Outlook 活动</span><span class="sxs-lookup"><span data-stu-id="0575c-123">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a><span data-ttu-id="0575c-124">获取有关共享者和委托人的日历信息，以及更新各个权限</span><span class="sxs-lookup"><span data-stu-id="0575c-124">Get calendar information about sharees and delegates, and update individual permissions</span></span>

<span data-ttu-id="0575c-125">本节内容：</span><span class="sxs-lookup"><span data-stu-id="0575c-125">In this section:</span></span>

- [<span data-ttu-id="0575c-126">日历所有者：获取共享或委派信息及权限</span><span class="sxs-lookup"><span data-stu-id="0575c-126">Calendar owner: Get sharing or delegation information and permissions</span></span>](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [<span data-ttu-id="0575c-127">日历所有者：在日历上更新现有共享者或委托人的权限</span><span class="sxs-lookup"><span data-stu-id="0575c-127">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

<span data-ttu-id="0575c-128">每个日历都与 [calendarPermission](/graph/api/resources/calendarpermission) 对象的集合相关联，其中每个对象都描述了日历所有者已设置的共享者或委托人以及关联权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-128">Each calendar is associated with a collection of [calendarPermission](/graph/api/resources/calendarpermission) objects, each of which describes a sharee or delegate and the associated permission that the calendar owner has set up.</span></span> <span data-ttu-id="0575c-129">[calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) 枚举定义了 Microsoft Graph 支持的权限范围：</span><span class="sxs-lookup"><span data-stu-id="0575c-129">The [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) enumeration defines the range of permissions that Microsoft Graph supports:</span></span>

- <span data-ttu-id="0575c-130">`none` 此值仅适用于对日历没有任何权限的 `My Organization`。</span><span class="sxs-lookup"><span data-stu-id="0575c-130">`none` This value applies to only `My Organization` which does not have any permissions to the calendar.</span></span> <span data-ttu-id="0575c-131">它不适用于单个用户，因为只有具有权限的用户才与日历的 **calendarPermission** 对象相关联。</span><span class="sxs-lookup"><span data-stu-id="0575c-131">It doesn't apply to individual users, as only users with permissions are associated with a **calendarPermission** object for the calendar.</span></span>
- <span data-ttu-id="0575c-132">`freeBusyRead` 共享者可以查看所有者的忙/闲状态，但不能查看日历上的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="0575c-132">`freeBusyRead` The sharee can view the owner's free/busy status, but not other details on the calendar.</span></span>
- <span data-ttu-id="0575c-133">`limitedRead` 共享者可以查看所有者的忙/闲状态以及日历上的非私人活动的标题和位置。</span><span class="sxs-lookup"><span data-stu-id="0575c-133">`limitedRead` The sharee can view the owner's free/busy status, and the titles and locations of non-private events on the calendar.</span></span>
- <span data-ttu-id="0575c-134">`read` 共享者可以查看所有者在私人活动中的忙/闲状态，以及日历上的非私人活动的所有详细信息。</span><span class="sxs-lookup"><span data-stu-id="0575c-134">`read` The sharee can view the owner's free/busy status in private events, and all the details of non-private events on the calendar.</span></span>
- <span data-ttu-id="0575c-135">`write` 共享者可以查看所有者在私人活动中的忙/闲状态，还可以查看日历上的非私人活动的所有详细信息并进行编辑（创建、更新或删除）。</span><span class="sxs-lookup"><span data-stu-id="0575c-135">`write` The sharee can view the owner's free/busy status in private events, and can view all the details and edit (create, update, or delete) non-private events on the calendar.</span></span>
- <span data-ttu-id="0575c-136">`delegateWithoutPrivateEventAccess` _委托人_可以查看所有者在私人活动中的忙/闲状态，并且对日历上的非私人活动具有`write`访问权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-136">`delegateWithoutPrivateEventAccess` The _delegate_ can view the owner's free/busy status in private events, and has `write` access to non-private events on the calendar.</span></span>
- <span data-ttu-id="0575c-137">`delegateWithPrivateEventAccess` _委托人_可以查看所有者的私人活动和非私人活动的详细信息，并且对日历上的所有活动都具有`write`访问权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-137">`delegateWithPrivateEventAccess` The _delegate_ can view details of the owner's private and non-private events, and has `write` access to all the events on the calendar.</span></span>

<span data-ttu-id="0575c-138">用户的主要日历始终与“我的组织”共享，它代表与所有者位于同一组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="0575c-138">The primary calendar of a user is always shared with "My Organization", which represents the users in the same organization as the owner.</span></span> <span data-ttu-id="0575c-139">默认情况下，他们可以在该日历上读取所有者的忙/闲状态，并且具有`freeBusyRead`权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-139">By default, they can read the owner's free/busy status on that calendar and have the `freeBusyRead` permission.</span></span>


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a><span data-ttu-id="0575c-140">日历所有者：获取共享或委派信息及权限</span><span class="sxs-lookup"><span data-stu-id="0575c-140">Calendar owner: Get sharing or delegation information and permissions</span></span>

<span data-ttu-id="0575c-141">下面的示例演示在 Alex 或管理员同意的情况下，如何获取与 Alex 的主要日历关联的 **calendarPermission** 对象。</span><span class="sxs-lookup"><span data-stu-id="0575c-141">The following example shows with the consent of Alex or administrator, how to get the **calendarPermission** objects associated with Alex' primary calendar.</span></span> <span data-ttu-id="0575c-142">请求将返回两个此类权限对象：</span><span class="sxs-lookup"><span data-stu-id="0575c-142">The request returns two such permission objects:</span></span>

- <span data-ttu-id="0575c-143">第一个 **calendarPermission** 对象已分配给委托人 Megan，并且具有下列属性值：</span><span class="sxs-lookup"><span data-stu-id="0575c-143">The first **calendarPermission** object is assigned to the delegate, Megan, and has the following property values:</span></span>

  - <span data-ttu-id="0575c-144">**isRemovable** 设置为 true，为 Alex 提供了取消委派的选项。</span><span class="sxs-lookup"><span data-stu-id="0575c-144">**isRemovable** is set to true, providing Alex the option to cancel the delegation.</span></span>
  - <span data-ttu-id="0575c-145">**isInsideOrganization** 为 true，因为只有同一组织中的用户才能成为委托人。</span><span class="sxs-lookup"><span data-stu-id="0575c-145">**isInsideOrganization** is true as only users in the same organization can be delegates.</span></span>
  - <span data-ttu-id="0575c-146">Megan 的 **role** 是由 Alex 设置的 `delegateWithPrivateEventAccess`。</span><span class="sxs-lookup"><span data-stu-id="0575c-146">**role** for Megan is `delegateWithPrivateEventAccess`, as set up by Alex.</span></span>
  - <span data-ttu-id="0575c-147">**allowedRoles** 包括支持委派的角色类型 `delegateWithoutPrivateEventAccess` 和 `delegateWithPrivateEventAccess`。</span><span class="sxs-lookup"><span data-stu-id="0575c-147">**allowedRoles** includes the role types `delegateWithoutPrivateEventAccess` and `delegateWithPrivateEventAccess` that support delegation.</span></span>
  - <span data-ttu-id="0575c-148">**emailAddress** 指定 Megan。</span><span class="sxs-lookup"><span data-stu-id="0575c-148">**emailAddress** specifies Megan.</span></span>

- <span data-ttu-id="0575c-149">第二个 **calendarPermission** 对象是分配给“我的组织”的默认对象，并且具有下列属性值：</span><span class="sxs-lookup"><span data-stu-id="0575c-149">The second **calendarPermission** object is a default object assigned to "My Organization", and has the following property values:</span></span>

  - <span data-ttu-id="0575c-150">**isRemovable** 设置为 false，因为主要日历始终与所有者的组织共享。</span><span class="sxs-lookup"><span data-stu-id="0575c-150">**isRemovable** is set to false, since the primary calendar is always shared with the owner's organization.</span></span>
  - <span data-ttu-id="0575c-151">**isInsideOrganization** 为 true。</span><span class="sxs-lookup"><span data-stu-id="0575c-151">**isInsideOrganization** is true.</span></span>
  - <span data-ttu-id="0575c-152">**role** 为 `freeBusyRead`，即“我的组织”的默认设置。</span><span class="sxs-lookup"><span data-stu-id="0575c-152">**role** is `freeBusyRead`, the default setting for "My Organization".</span></span>
  - <span data-ttu-id="0575c-153">**emailAddress** 将 **name** 子属性指定为“我的组织”；“我的组织”的 **address** 默认为 null。</span><span class="sxs-lookup"><span data-stu-id="0575c-153">**emailAddress** specifies the **name** sub-property as "My Organization"; **address** for "My Organization" is by default null.</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[<span data-ttu-id="0575c-155">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarperms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendarperms",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/calendarPermissions",
    "value": [
        {
            "id": "L289RXhjaGFuZ2VMYWJTWVnYW5C",
            "isRemovable": true,
            "isInsideOrganization": true,
            "role": "delegateWithPrivateEventAccess",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read",
                "write",
                "delegateWithoutPrivateEventAccess",
                "delegateWithPrivateEventAccess"
            ],
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a><span data-ttu-id="0575c-158">日历所有者：在日历上更新现有共享者或委托人的权限</span><span class="sxs-lookup"><span data-stu-id="0575c-158">Calendar owner: Update permissions for an existing sharee or delegate on a calendar</span></span>

<span data-ttu-id="0575c-159">在 Alex 或管理员同意的情况下，只要最初为该日历的共享者或委托人设置的这些 **allowedRoles** 支持新权限，你就可以更新分配给现有共享者或委托人的权限（由 **role** 属性指定）。</span><span class="sxs-lookup"><span data-stu-id="0575c-159">With the consent of Alex or administrator, you can update the permissions assigned to an existing sharee or delegate (specified by the **role** property), as long as the new permissions are supported by those **allowedRoles** set up initially for the sharee or delegate for that calendar.</span></span> 

<span data-ttu-id="0575c-160">除了 **role** 属性之外，你不能更新现有共享者或委托人的其他属性。</span><span class="sxs-lookup"><span data-stu-id="0575c-160">Aside from the **role** property, you cannot update other properties of an existing sharee or delegate.</span></span> <span data-ttu-id="0575c-161">更改 **emailAddress** 属性值需要删除共享者或委托人，并再次设置 **calendarPermission** 的新实例。</span><span class="sxs-lookup"><span data-stu-id="0575c-161">Changing the **emailAddress** property value requires deleting the sharee or delegate and setting up a new instance of **calendarPermission** again.</span></span>

<span data-ttu-id="0575c-162">以下示例更新了 **role** 属性，将自定义日历“儿童派对”的现有共享者 Adele 的权限从 `read` 更改为 `write`。</span><span class="sxs-lookup"><span data-stu-id="0575c-162">The following example updates the **role** property, changing the permission of an existing sharee, Adele, from `read` to `write` for the custom calendar "Kids parties".</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarperm",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJQWRlbGVW"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[<span data-ttu-id="0575c-164">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarperm-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "update_calendarperm",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AAMkADAwAABf02bAAAA%3D')/calendarPermissions/$entity",
    "id": "L289RXhjaGFuZ2VMYWJQWRlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="0575c-167">获取共享或委托日历的属性</span><span class="sxs-lookup"><span data-stu-id="0575c-167">Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="0575c-168">本节内容：</span><span class="sxs-lookup"><span data-stu-id="0575c-168">In this section:</span></span>

- [<span data-ttu-id="0575c-169">日历所有者：获取共享或委托日历的属性</span><span class="sxs-lookup"><span data-stu-id="0575c-169">Calendar owner: Get properties of a shared or delegated calendar</span></span>](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [<span data-ttu-id="0575c-170">共享者或委托人：获取共享或委托日历的属性</span><span class="sxs-lookup"><span data-stu-id="0575c-170">Sharee or delegate: Get properties of shared or delegated calendar</span></span>](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

<span data-ttu-id="0575c-171">在本示例中，Alex 委派了他的主要日历，并向委托人 Megan Bowen 授予了查看标记为“私人”的日历项目的权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-171">Recalling in this example, Alex has delegated his primary calendar and given the delegate, Megan Bowen, the permission to view calendar items that are marked private.</span></span>
<span data-ttu-id="0575c-172">此部分显示委派日历的属性，首先从所有者 Alex 的角度出发并征得其同意，然后从委托人 Megan 的角度出发并征得其同意。</span><span class="sxs-lookup"><span data-stu-id="0575c-172">This section shows the properties of the delegated calendar, first from the perspective of and with the consent of the owner, Alex, and then from the perspective of and with the consent of the delegate, Megan.</span></span> <span data-ttu-id="0575c-173">来自管理员的同意也适用于每种情况。</span><span class="sxs-lookup"><span data-stu-id="0575c-173">Consent from the administrator also works for each case.</span></span>

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a><span data-ttu-id="0575c-174">日历所有者：获取共享或委托日历的属性</span><span class="sxs-lookup"><span data-stu-id="0575c-174">Calendar owner: Get properties of a shared or delegated calendar</span></span>

<span data-ttu-id="0575c-175">以下示例从所有者 Alex 的角度获取主要日历的属性。</span><span class="sxs-lookup"><span data-stu-id="0575c-175">The following example gets the properties of the primary calendar from the perspective of the owner, Alex.</span></span> 

<span data-ttu-id="0575c-176">注意以下代表 Alex 的属性：</span><span class="sxs-lookup"><span data-stu-id="0575c-176">Note the following properties on Alex' behalf:</span></span>

- <span data-ttu-id="0575c-177">**canShare** 为 true，因为 Alex 是所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-177">**canShare** is true as Alex is the owner.</span></span>
- <span data-ttu-id="0575c-178">**canViewPrivateItems** 为 true，因为 Alex 是所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-178">**canViewPrivateItems** is true since Alex is the owner.</span></span>
- <span data-ttu-id="0575c-179">**isShared** 设置为 true，因为 Alex 为此日历设置了委托人。</span><span class="sxs-lookup"><span data-stu-id="0575c-179">**isShared** is set to true, as Alex has set up a delegate for this calendar.</span></span>
- <span data-ttu-id="0575c-180">对于日历所有者，**isSharedWithMe** 始终为 false。</span><span class="sxs-lookup"><span data-stu-id="0575c-180">**isSharedWithMe** is always false for the calendar owner.</span></span>
- <span data-ttu-id="0575c-181">**owner** 显示 Alex 为所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-181">**owner** shows Alex as the owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="0575c-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[<span data-ttu-id="0575c-183">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAw7QAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "isDefaultCalendar": true,
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a><span data-ttu-id="0575c-186">共享者或委托人：获取共享或委托日历的属性</span><span class="sxs-lookup"><span data-stu-id="0575c-186">Sharee or delegate: Get properties of shared or delegated calendar</span></span>

<span data-ttu-id="0575c-187">以下示例从委托人 Megan 的角度获取同一日历的属性。</span><span class="sxs-lookup"><span data-stu-id="0575c-187">The following example gets the properties of the same calendar from the perspective of the delegate, Megan.</span></span> 

<span data-ttu-id="0575c-188">注意下列属性：</span><span class="sxs-lookup"><span data-stu-id="0575c-188">Note the following properties:</span></span>

- <span data-ttu-id="0575c-189">默认情况下，日历的 **name** 是所有者的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0575c-189">**name** of the calendar is by default the owner's display name.</span></span> <span data-ttu-id="0575c-190">在本例中，它是“Alex Wilber”，因为这是 Alex 委派给 Megan 的日历。</span><span class="sxs-lookup"><span data-stu-id="0575c-190">In this case, it's "Alex Wilber", since this is Alex' calendar delegated to Megan.</span></span> 
- <span data-ttu-id="0575c-191">**canShare** 为 false，因为 Megan 不是此日历的所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-191">**canShare** is false, since Megan is not the owner of this calendar.</span></span>
- <span data-ttu-id="0575c-192">对于由 Alex 设置的委托人 Megan，**canViewPrivateItems** 为 true。</span><span class="sxs-lookup"><span data-stu-id="0575c-192">**canViewPrivateItems** is true for the delegate Megan, as set up by Alex.</span></span> <span data-ttu-id="0575c-193">对于不是委托人的共享者，此属性始终为 false。</span><span class="sxs-lookup"><span data-stu-id="0575c-193">For a sharee that is not a delegate, this property is always false.</span></span>
- <span data-ttu-id="0575c-194">**isShared** 为 false。</span><span class="sxs-lookup"><span data-stu-id="0575c-194">**isShared** is false.</span></span> <span data-ttu-id="0575c-195">此属性仅向日历_所有者_指示日历是共享日历还是委派日历。</span><span class="sxs-lookup"><span data-stu-id="0575c-195">This property indicates only to a calendar _owner_ whether the calendar has been shared or delegated.</span></span>
- <span data-ttu-id="0575c-196">**isSharedWithMe** 属性为 true，因为 Megan 是委托人。</span><span class="sxs-lookup"><span data-stu-id="0575c-196">**isSharedWithMe** property is true, since Megan is a delegate.</span></span>
- <span data-ttu-id="0575c-197">**canEdit** 是 true，因为包括 Megan 在内的委托人具有写入访问权限。</span><span class="sxs-lookup"><span data-stu-id="0575c-197">**canEdit** is true, since delegates, including Megan, have write access.</span></span>
- <span data-ttu-id="0575c-198">**owner** 设置为 Alex。</span><span class="sxs-lookup"><span data-stu-id="0575c-198">**owner** is set to Alex.</span></span>

> [!NOTE] 
> <span data-ttu-id="0575c-199">共享者或委托人只能自定义共享/委派日历的 **name** 属性。</span><span class="sxs-lookup"><span data-stu-id="0575c-199">A sharee or delegate can customize only the **name** property of a shared/delegated calendar.</span></span> <span data-ttu-id="0575c-200">更新仅对他们自己可见；日历所有者无法查看此类日历名称更改。</span><span class="sxs-lookup"><span data-stu-id="0575c-200">The update is visible only to themselves; the calendar owner does not see such calendar name changes.</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[<span data-ttu-id="0575c-202">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-delegate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_delegate",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('meganb%40contoso.OnMicrosoft.com')/calendars/$entity",
    "id": "AAMkADlAABhbftjAAA=",
    "name": "Alex Wilber",
    "color": "auto",
    "hexColor": "",
    "isDefaultCalendar": false,
    "changeKey": "E6LznKWmX0KTsAD9qRJjeAAAYWo3EQ==",
    "canShare": false,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": true,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a><span data-ttu-id="0575c-205">获取或设置邮箱设置以接收会议请求和响应</span><span class="sxs-lookup"><span data-stu-id="0575c-205">Get or set mailbox setting to receive meeting requests and responses</span></span>

<span data-ttu-id="0575c-206">本节内容：</span><span class="sxs-lookup"><span data-stu-id="0575c-206">In this section:</span></span>

- [<span data-ttu-id="0575c-207">获取用户邮箱的委派传递设置</span><span class="sxs-lookup"><span data-stu-id="0575c-207">Get delegation delivery setting for a user's mailbox</span></span>](#get-delegation-delivery-setting-for-a-users-mailbox)
- [<span data-ttu-id="0575c-208">设置用户邮箱的委派传递设置</span><span class="sxs-lookup"><span data-stu-id="0575c-208">Set delegation delivery setting for a user's mailbox</span></span>](#set-delegation-delivery-setting-for-a-users-mailbox)

<span data-ttu-id="0575c-209">根据日历所有者首选的委派级别，所有者可以指定接收会议请求和响应的人员，以管理日历上的会议。</span><span class="sxs-lookup"><span data-stu-id="0575c-209">Depending on the level of delegation a calendar owner prefers, the owner can specify who should receive meeting requests and responses to manage meetings on the calendar.</span></span> 

<span data-ttu-id="0575c-210">可通过编程方式获取或设置日历所有者的 [mailboxSettings](/graph/api/resources/mailboxsettings) 的 **delegateMeetingMessageDeliveryOptions** 属性，以指定 Outlook 应将 [eventMessageRequest](/graph/api/resources/eventmessagerequest) 和 [eventMessageResponse](/graph/api/resources/eventmessageresponse) 实例定向到的人员：</span><span class="sxs-lookup"><span data-stu-id="0575c-210">Programmatically, you can get or set the **delegateMeetingMessageDeliveryOptions** property of the calendar owner's [mailboxSettings](/graph/api/resources/mailboxsettings) to specify to whom Outlook should direct [eventMessageRequest](/graph/api/resources/eventmessagerequest) and [eventMessageResponse](/graph/api/resources/eventmessageresponse) instances:</span></span>

- `sendToDelegateOnly`

    <span data-ttu-id="0575c-211">Outlook 仅将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人。</span><span class="sxs-lookup"><span data-stu-id="0575c-211">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to only delegates.</span></span> <span data-ttu-id="0575c-212">这是默认设置。</span><span class="sxs-lookup"><span data-stu-id="0575c-212">This is the default setting.</span></span> <span data-ttu-id="0575c-213">所有者可以通过委派日历中的相应**活动**来查看对会议的响应或对邀请的响应。</span><span class="sxs-lookup"><span data-stu-id="0575c-213">The owner can see responses to a meeting or respond to an invitation through the corresponding **event** in the delegated calendar.</span></span>
- `sendToDelegateAndInformationToPrincipal`

    <span data-ttu-id="0575c-214">Outlook 将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人和日历所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-214">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner.</span></span> <span data-ttu-id="0575c-215">只有委托人才能看到接受和拒绝会议请求的选项。发送给所有者的通知将以一般电子邮件的形式显示。</span><span class="sxs-lookup"><span data-stu-id="0575c-215">Only the delegates see the option to accept or decline a meeting request, and the notification sent to the owner appears like a normal email message.</span></span> <span data-ttu-id="0575c-216">所有者仍可以通过在委派日历中打开**活动**并做出响应来响应会议。</span><span class="sxs-lookup"><span data-stu-id="0575c-216">The owner can still respond to the meeting by opening the **event** in the delegated calendar and responding.</span></span>
- `sendToDelegateAndPrincipal`

    <span data-ttu-id="0575c-217">Outlook 将 **eventMessageRequest** 和 **eventMessageResponse** 实例定向到委托人和日历所有者，他们都可以响应会议请求。</span><span class="sxs-lookup"><span data-stu-id="0575c-217">Outlook to direct **eventMessageRequest** and **eventMessageResponse** instances to delegates and the calendar owner, either of whom can respond to the meeting request.</span></span>

<span data-ttu-id="0575c-218">这是邮箱范围的设置，因此相同的设置适用于邮箱所有者的所有委托人。</span><span class="sxs-lookup"><span data-stu-id="0575c-218">This is a mailbox-wide setting, so the same setting applies to all delegates of the mailbox owner.</span></span>

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="0575c-219">获取用户邮箱的委派传递设置</span><span class="sxs-lookup"><span data-stu-id="0575c-219">Get delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="0575c-220">以下示例将获取日历所有者的 **mailboxSettings**，该所有者仅允许 Outlook 将会议请求和响应定向到日历委托人；即 **delegateMeetingMessageDeliveryOptions** 设置为 `sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="0575c-220">The following example gets the **mailboxSettings** of a calendar owner who lets Outlook direct meeting requests and responses to only calendar delegates; that is, **delegateMeetingMessageDeliveryOptions** is set to `sendToDelegateOnly`.</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[<span data-ttu-id="0575c-222">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "archiveFolder": "AQMkADAwAGVQAAAKfowAAAA==",
    "timeZone": "Pacific Standard Time",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly",
    "dateFormat": "M/d/yyyy",
    "timeFormat": "h:mm tt",
    "automaticRepliesSetting": {
        "status": "disabled",
        "externalAudience": "all",
        "internalReplyMessage": "",
        "externalReplyMessage": "",
        "scheduledStartDateTime": {
            "dateTime": "2019-12-24T05:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2019-12-25T05:00:00.0000000",
            "timeZone": "UTC"
        }
    },
    "language": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "workingHours": {
        "daysOfWeek": [
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone": {
            "name": "Pacific Standard Time"
        }
    }
}
```

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a><span data-ttu-id="0575c-225">设置用户邮箱的委派传递设置</span><span class="sxs-lookup"><span data-stu-id="0575c-225">Set delegation delivery setting for a user's mailbox</span></span>

<span data-ttu-id="0575c-226">以下示例将 **delegateMeetingMessageDeliveryOptions** 属性更新为 `sendToDelegateAndPrincipal`，以让 Outlook 将委派日历的会议请求和响应定向到所有委托人和所有者。</span><span class="sxs-lookup"><span data-stu-id="0575c-226">The following example updates the **delegateMeetingMessageDeliveryOptions** property to `sendToDelegateAndPrincipal`, to have Outlook direct meeting requests and responses of the delegated calendar to all delegates and the owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
Content-type: application/json

{
  "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```
# <a name="c"></a>[<span data-ttu-id="0575c-228">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "patch_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a><span data-ttu-id="0575c-231">删除日历的共享者或委托人</span><span class="sxs-lookup"><span data-stu-id="0575c-231">Delete a sharee or delegate of a calendar</span></span>

<span data-ttu-id="0575c-232">在下面的示例中，Alex 将删除作为“儿童派对”日历共享者的 Megan。</span><span class="sxs-lookup"><span data-stu-id="0575c-232">In the following example, Alex deletes Megan as a sharee of the "Kids parties" calendar.</span></span>


# <a name="http"></a>[<span data-ttu-id="0575c-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="0575c-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[<span data-ttu-id="0575c-234">C#</span><span class="sxs-lookup"><span data-stu-id="0575c-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0575c-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0575c-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0575c-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0575c-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharee-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a><span data-ttu-id="0575c-237">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0575c-237">Next steps</span></span>

<span data-ttu-id="0575c-238">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="0575c-238">Find out more about:</span></span>

- <span data-ttu-id="0575c-239">Outlook 客户端如何支持共享和委派日历：</span><span class="sxs-lookup"><span data-stu-id="0575c-239">How the Outlook clients support sharing and delegating calendars:</span></span>
  - [<span data-ttu-id="0575c-240">与其他人共享 Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="0575c-240">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [<span data-ttu-id="0575c-241">允许其他人作为委托人管理你的邮件和日历</span><span class="sxs-lookup"><span data-stu-id="0575c-241">Allow someone else to manage your mail and calendar as a delegate</span></span>](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [<span data-ttu-id="0575c-242">在 Outlook 网页版中共享日历</span><span class="sxs-lookup"><span data-stu-id="0575c-242">Share your calendar in Outlook on the web</span></span>](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [<span data-ttu-id="0575c-243">Outlook 网页版中的日历委派</span><span class="sxs-lookup"><span data-stu-id="0575c-243">Calendar delegation in Outlook on the web</span></span>](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [<span data-ttu-id="0575c-244">获取共享日历或委托日历中的 Outlook 事件</span><span class="sxs-lookup"><span data-stu-id="0575c-244">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="0575c-245">在共享或委托日历中创建 Outlook 活动</span><span class="sxs-lookup"><span data-stu-id="0575c-245">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="0575c-246">为什么要与 Outlook 日历集成</span><span class="sxs-lookup"><span data-stu-id="0575c-246">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="0575c-247">Microsoft Graph beta 中的[日历 API](/graph/api/resources/calendar)。</span><span class="sxs-lookup"><span data-stu-id="0575c-247">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph beta.</span></span>
