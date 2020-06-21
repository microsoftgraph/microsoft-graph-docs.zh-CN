---
title: Microsoft Graph 已知问题
description: 本文介绍了 Microsoft Graph 的已知问题。
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 98c61991ec99b1f7776c03f5fa5bc2400b5950a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744054"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="bd752-103">Microsoft Graph 已知问题</span><span class="sxs-lookup"><span data-stu-id="bd752-103">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="bd752-104">本文介绍了 Microsoft Graph 的已知问题。</span><span class="sxs-lookup"><span data-stu-id="bd752-104">This article describes known issues with Microsoft Graph.</span></span> 

<span data-ttu-id="bd752-105">若要报告已知问题，请参阅[Microsoft Graph 支持](https://developer.microsoft.com/graph/support)页面。</span><span class="sxs-lookup"><span data-stu-id="bd752-105">To report a known issue, see the [Microsoft Graph support](https://developer.microsoft.com/graph/support) page.</span></span>

<span data-ttu-id="bd752-106">有关 Microsoft Graph API 的最新更新的信息，请参阅[Microsoft graph 更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="bd752-106">For information about the latest updates to the Microsoft Graph API, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="bookings"></a><span data-ttu-id="bd752-107">Bookings</span><span class="sxs-lookup"><span data-stu-id="bd752-107">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="bd752-108">查询 bookingBusinesses 时出现 ErrorExceededFindCountLimit</span><span class="sxs-lookup"><span data-stu-id="bd752-108">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="bd752-109">当组织拥有多个预订业务且提出请求的帐户不是管理员时，获取 `bookingBusinesses` 列表会失败，并显示以下错误代码：</span><span class="sxs-lookup"><span data-stu-id="bd752-109">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="bd752-110">解决方法是，可以通过加入 `query` 参数来限制请求返回的业务集，例如：</span><span class="sxs-lookup"><span data-stu-id="bd752-110">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a><span data-ttu-id="bd752-111">日历</span><span class="sxs-lookup"><span data-stu-id="bd752-111">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="bd752-112">访问共享日历</span><span class="sxs-lookup"><span data-stu-id="bd752-112">Accessing a shared calendar</span></span>

<span data-ttu-id="bd752-113">使用以下操作尝试访问其他用户共享的日历中的事件时：</span><span class="sxs-lookup"><span data-stu-id="bd752-113">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET /users/{id}/calendars/{id}/events
```

<span data-ttu-id="bd752-114">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`.</span><span class="sxs-lookup"><span data-stu-id="bd752-114">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`.</span></span> <span data-ttu-id="bd752-115">The error occurs because:</span><span class="sxs-lookup"><span data-stu-id="bd752-115">The error occurs because:</span></span>

- <span data-ttu-id="bd752-116">过去，日历共享的实现方法有两种。为了加以区分，将它们称为“旧”方法和“新”方法。</span><span class="sxs-lookup"><span data-stu-id="bd752-116">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="bd752-117">新方法当前可用于通过查看或编辑权限共享日历，但无法通过委派权限进行共享。</span><span class="sxs-lookup"><span data-stu-id="bd752-117">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="bd752-118">只有使用**新**方法共享日历后，才能使用日历 REST API 查看或编辑共享日历。</span><span class="sxs-lookup"><span data-stu-id="bd752-118">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="bd752-119">如果使用**旧**方法共享日历，则无法使用日历 REST API 查看或编辑此类日历（或其事件）。</span><span class="sxs-lookup"><span data-stu-id="bd752-119">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="bd752-120">如果日历是通过查看或编辑权限共享，但使用的是旧方法，现在可以修复错误，手动将日历共享升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="bd752-120">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="bd752-121">随着时间的推移，Outlook 将把所有共享日历（包括通过委托权限共享的日历）自动升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="bd752-121">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="bd752-122">若要手动将共享日历升级为使用新方法，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="bd752-122">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="bd752-123">收件人删除以前与他们共享的日历。</span><span class="sxs-lookup"><span data-stu-id="bd752-123">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="bd752-124">日历所有者在 Outlook 网页版、iOS 版或 Android 版中重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="bd752-124">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="bd752-125">The recipient re-accepts the shared calendar using Outlook on the web.</span><span class="sxs-lookup"><span data-stu-id="bd752-125">The recipient re-accepts the shared calendar using Outlook on the web.</span></span> <span data-ttu-id="bd752-126">(It will be possible to use other Outlook clients soon.)</span><span class="sxs-lookup"><span data-stu-id="bd752-126">(It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="bd752-127">收件人可以在 Outlook iOS 版或 Android 版中查看共享日历，从而验证是否已成功使用新方法重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="bd752-127">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="bd752-128">A calendar shared with you in the new approach appears as just another calendar in your mailbox.</span><span class="sxs-lookup"><span data-stu-id="bd752-128">A calendar shared with you in the new approach appears as just another calendar in your mailbox.</span></span> <span data-ttu-id="bd752-129">You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar.</span><span class="sxs-lookup"><span data-stu-id="bd752-129">You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar.</span></span> <span data-ttu-id="bd752-130">As an example:</span><span class="sxs-lookup"><span data-stu-id="bd752-130">As an example:</span></span>

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="bd752-131">在用户邮箱中添加和访问基于 ICS 的日历</span><span class="sxs-lookup"><span data-stu-id="bd752-131">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="bd752-132">目前，还有部分支持基于 Internet 日历订阅 (ICS) 的日历：</span><span class="sxs-lookup"><span data-stu-id="bd752-132">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="bd752-133">你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。</span><span class="sxs-lookup"><span data-stu-id="bd752-133">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="bd752-134">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars.</span><span class="sxs-lookup"><span data-stu-id="bd752-134">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars.</span></span> <span data-ttu-id="bd752-135">You cannot store or access the ICS URL in the calendar resource.</span><span class="sxs-lookup"><span data-stu-id="bd752-135">You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="bd752-136">还可以[列出基于 ICS 的日历事件](/graph/api/calendar-list-events?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="bd752-136">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="attaching-large-files-to-events"></a><span data-ttu-id="bd752-137">将大型文件附加到事件</span><span class="sxs-lookup"><span data-stu-id="bd752-137">Attaching large files to events</span></span>
<span data-ttu-id="bd752-138">尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。</span><span class="sxs-lookup"><span data-stu-id="bd752-138">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="bd752-139">使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) 才会成功。</span><span class="sxs-lookup"><span data-stu-id="bd752-139">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="bd752-140">Microsoft Teams 的 onlineMeetingUrl 属性支持</span><span class="sxs-lookup"><span data-stu-id="bd752-140">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="bd752-141">目前，Skype 会议[事件](/graph/api/resources/event?view=graph-rest-1.0)的 **onlineMeetingUrl** 属性指明联机会议 URL。</span><span class="sxs-lookup"><span data-stu-id="bd752-141">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="bd752-142">不过，对于 Microsoft Teams 会议事件，此属性设置为 NULL。</span><span class="sxs-lookup"><span data-stu-id="bd752-142">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

<span data-ttu-id="bd752-143">Beta 版本提供了一种变通方法，可以使用 [事件](/graph/api/resources/event?view=graph-rest-beta) 的 **onlineMeetingProvider** 属性来验证提供程序是否为 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="bd752-143">The beta version offers a workaround, where you can use the **onlineMeetingProvider** property of an [event](/graph/api/resources/event?view=graph-rest-beta) to verify if the provider is Microsoft Teams.</span></span> <span data-ttu-id="bd752-144">通过**事件**的 \*\*\*\* 属性，可以访问 **joinUrl**。</span><span class="sxs-lookup"><span data-stu-id="bd752-144">Through the **onlineMeeting** property of the **event**, you can access the **joinUrl**.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="bd752-145">更改通知</span><span class="sxs-lookup"><span data-stu-id="bd752-145">Change notifications</span></span>

### <a name="additional-notifications-for-users"></a><span data-ttu-id="bd752-146">其他用户通知</span><span class="sxs-lookup"><span data-stu-id="bd752-146">Additional notifications for users</span></span>

<span data-ttu-id="bd752-147">对于“**changeType**”设置为“**updated**” 的“**user**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”的通知：在创建和软删除用户时**已更新**。</span><span class="sxs-lookup"><span data-stu-id="bd752-147">[Subscriptions](/graph/api/resources/subscription) to changes for **user** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on user creation and user soft deletion.</span></span>

### <a name="additional-notifications-for-groups"></a><span data-ttu-id="bd752-148">其他组通知</span><span class="sxs-lookup"><span data-stu-id="bd752-148">Additional notifications for groups</span></span>

<span data-ttu-id="bd752-149">对于“**changeType**”设置为“**updated**” 的“**group**”，[订阅](/graph/api/resources/subscription)以上更改还将收到“**changeType**”通知：在创建和软删除组时**已更新**。</span><span class="sxs-lookup"><span data-stu-id="bd752-149">[Subscriptions](/graph/api/resources/subscription) to changes for **group** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on group creation and group soft deletion.</span></span>

## <a name="cloud-communications"></a><span data-ttu-id="bd752-150">云通信</span><span class="sxs-lookup"><span data-stu-id="bd752-150">Cloud communications</span></span> 

<span data-ttu-id="bd752-151">对于通过云通信 API 创建的频道会议，Microsoft Teams 客户端不会显示“**查看会议详细信息**”菜单。</span><span class="sxs-lookup"><span data-stu-id="bd752-151">The Microsoft Teams client does not show the **View Meeting details**  menu for channel meetings created via the cloud communications API.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="bd752-152">云解决方案提供商应用</span><span class="sxs-lookup"><span data-stu-id="bd752-152">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="bd752-153">CSP 应用必须使用 Azure AD 终结点</span><span class="sxs-lookup"><span data-stu-id="bd752-153">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="bd752-154">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers.</span><span class="sxs-lookup"><span data-stu-id="bd752-154">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers.</span></span> <span data-ttu-id="bd752-155">Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span><span class="sxs-lookup"><span data-stu-id="bd752-155">Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="bd752-156">对 CSP 应用的预授权不适用于一些客户租户</span><span class="sxs-lookup"><span data-stu-id="bd752-156">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="bd752-157">在某些情况下，对 CSP 应用的预授权可能不适用于一些客户租户。</span><span class="sxs-lookup"><span data-stu-id="bd752-157">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="bd752-158">对于使用委派权限的应用，首次将此应用用于新客户租户时，登录后可能会看到以下错误：`AADSTS50000: There was an error issuing a token`。</span><span class="sxs-lookup"><span data-stu-id="bd752-158">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="bd752-159">对于使用应用权限的应用，应用可以获取令牌，但在调用 Microsoft Graph 时会意外看到“拒绝访问”消息。</span><span class="sxs-lookup"><span data-stu-id="bd752-159">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="bd752-160">我们正在努力工作，以尽快解决此问题，让预授权适用于所有客户租户。</span><span class="sxs-lookup"><span data-stu-id="bd752-160">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="bd752-161">同时，若要取消阻止开发和测试，可使用以下解决方法。</span><span class="sxs-lookup"><span data-stu-id="bd752-161">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="bd752-162">**NOTE:** This is not a permanent solution and is only intended to unblock development.</span><span class="sxs-lookup"><span data-stu-id="bd752-162">**NOTE:** This is not a permanent solution and is only intended to unblock development.</span></span>  <span data-ttu-id="bd752-163">This workaround will not be required once the aforementioned issue is fixed.</span><span class="sxs-lookup"><span data-stu-id="bd752-163">This workaround will not be required once the aforementioned issue is fixed.</span></span>  <span data-ttu-id="bd752-164">This workaround does not need to be undone once the fix is in place.</span><span class="sxs-lookup"><span data-stu-id="bd752-164">This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="bd752-165">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window.</span><span class="sxs-lookup"><span data-stu-id="bd752-165">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window.</span></span> <span data-ttu-id="bd752-166">You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="bd752-166">You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="bd752-167">创建 Microsoft Graph 服务主体。</span><span class="sxs-lookup"><span data-stu-id="bd752-167">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a><span data-ttu-id="bd752-168">联系人</span><span class="sxs-lookup"><span data-stu-id="bd752-168">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="bd752-169">仅 beta 版支持组织联系人。</span><span class="sxs-lookup"><span data-stu-id="bd752-169">Organization contacts available in only beta</span></span>

<span data-ttu-id="bd752-170">Only personal contacts are currently supported.</span><span class="sxs-lookup"><span data-stu-id="bd752-170">Only personal contacts are currently supported.</span></span> <span data-ttu-id="bd752-171">Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span><span class="sxs-lookup"><span data-stu-id="bd752-171">Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="bd752-172">默认联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="bd752-172">Default contacts folder</span></span>

<span data-ttu-id="bd752-173">在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="bd752-173">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="bd752-174">A fix will be made available.</span><span class="sxs-lookup"><span data-stu-id="bd752-174">A fix will be made available.</span></span> <span data-ttu-id="bd752-175">Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span><span class="sxs-lookup"><span data-stu-id="bd752-175">Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="bd752-176">在上面的查询中：</span><span class="sxs-lookup"><span data-stu-id="bd752-176">In the above query:</span></span>

1. <span data-ttu-id="bd752-177">`/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](/graph/api/resources/contact?view=graph-rest-1.0) 的属性。</span><span class="sxs-lookup"><span data-stu-id="bd752-177">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="bd752-178">附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="bd752-178">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="bd752-179">在 beta 版中通过联系人文件夹访问联系人</span><span class="sxs-lookup"><span data-stu-id="bd752-179">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="bd752-180">目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，进而阻止访问[联系人](/graph/api/resources/contact?view=graph-rest-beta)，如以下 2 个方案所示。</span><span class="sxs-lookup"><span data-stu-id="bd752-180">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="bd752-181">从用户的顶级 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) 访问联系人。</span><span class="sxs-lookup"><span data-stu-id="bd752-181">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="bd752-182">Accessing a contact contained in a child folder of a **contactFolder**.</span><span class="sxs-lookup"><span data-stu-id="bd752-182">Accessing a contact contained in a child folder of a **contactFolder**.</span></span>  <span data-ttu-id="bd752-183">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span><span class="sxs-lookup"><span data-stu-id="bd752-183">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="bd752-184">或者，如下所示，只需指定联系人 ID 即可[获取](/graph/api/contact-get?view=graph-rest-beta)此联系人，因为在 `/beta` 版中 GET /contacts 适用于用户邮箱中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="bd752-184">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a><span data-ttu-id="bd752-185">Delta 查询</span><span class="sxs-lookup"><span data-stu-id="bd752-185">Delta query</span></span>

* <span data-ttu-id="bd752-186">跟踪关系更改时，OData 上下文有时无法正确返回。</span><span class="sxs-lookup"><span data-stu-id="bd752-186">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="bd752-187">架构扩展（旧版）未使用 $select 语句返回，而是在无 $select 的情况下返回。</span><span class="sxs-lookup"><span data-stu-id="bd752-187">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="bd752-188">客户端无法跟踪开放扩展或已注册的架构扩展的更改。</span><span class="sxs-lookup"><span data-stu-id="bd752-188">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="extensions"></a><span data-ttu-id="bd752-189">扩展</span><span class="sxs-lookup"><span data-stu-id="bd752-189">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="bd752-190">不支持更改跟踪</span><span class="sxs-lookup"><span data-stu-id="bd752-190">Change tracking is not supported</span></span>

<span data-ttu-id="bd752-191">开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。</span><span class="sxs-lookup"><span data-stu-id="bd752-191">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="bd752-192">同时创建资源和开放扩展</span><span class="sxs-lookup"><span data-stu-id="bd752-192">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="bd752-193">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**.</span><span class="sxs-lookup"><span data-stu-id="bd752-193">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**.</span></span> <span data-ttu-id="bd752-194">You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span><span class="sxs-lookup"><span data-stu-id="bd752-194">You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="bd752-195">创建资源实例的同时添加架构扩展数据</span><span class="sxs-lookup"><span data-stu-id="bd752-195">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="bd752-196">不能在创建 **contact**、**event**、**message** 或 **post** 实例的同一个操作中指定架构扩展。</span><span class="sxs-lookup"><span data-stu-id="bd752-196">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="bd752-197">必须先创建资源实例，然后再对此实例执行 `PATCH`，从而添加架构扩展和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="bd752-197">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="bd752-198">每资源实例最多可以添加 100 个架构扩展属性值</span><span class="sxs-lookup"><span data-stu-id="bd752-198">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="bd752-199">目录资源（如**设备**、**组**和**用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。</span><span class="sxs-lookup"><span data-stu-id="bd752-199">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="bd752-200">并非所有实体类型都支持对架构扩展属性进行筛选</span><span class="sxs-lookup"><span data-stu-id="bd752-200">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="bd752-201">Outlook 实体类型不支持对架构扩展属性进行筛选（使用 `$filter` 表达式）- **联系人**、**事件**、**消息**或**帖子**。</span><span class="sxs-lookup"><span data-stu-id="bd752-201">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="files-onedrive"></a><span data-ttu-id="bd752-202">文件 (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="bd752-202">Files (OneDrive)</span></span>

* <span data-ttu-id="bd752-203">在通过浏览器访问个人站点之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 401 响应。</span><span class="sxs-lookup"><span data-stu-id="bd752-203">First time access to a user's personal drive through Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="groups"></a><span data-ttu-id="bd752-204">组</span><span class="sxs-lookup"><span data-stu-id="bd752-204">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="bd752-205">组和 Microsoft Teams 的权限</span><span class="sxs-lookup"><span data-stu-id="bd752-205">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="bd752-206">Microsoft Graph 为组和 Microsoft Teams 公开了两个用于访问 API 的权限（[*Group.Read.All*](permissions-reference.md#group-permissions) 和 [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)）。</span><span class="sxs-lookup"><span data-stu-id="bd752-206">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="bd752-207">管理员必须同意授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="bd752-207">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="bd752-208">今后，我们计划新增用户可同意授予的组和团队权限。</span><span class="sxs-lookup"><span data-stu-id="bd752-208">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="bd752-209">Also, only the API for core group administration and management supports access using delegated or app-only permissions.</span><span class="sxs-lookup"><span data-stu-id="bd752-209">Also, only the API for core group administration and management supports access using delegated or app-only permissions.</span></span> <span data-ttu-id="bd752-210">All other features of the group API support only delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="bd752-210">All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="bd752-211">同时支持委派权限和仅限应用权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="bd752-211">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="bd752-212">创建和删除组</span><span class="sxs-lookup"><span data-stu-id="bd752-212">Creating and deleting groups</span></span>
* <span data-ttu-id="bd752-213">获取和更新与组管理或管理相关的组属性</span><span class="sxs-lookup"><span data-stu-id="bd752-213">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="bd752-214">组[目录设置](/graph/api/resources/directoryobject?view=graph-rest-1.0)、类型和同步</span><span class="sxs-lookup"><span data-stu-id="bd752-214">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="bd752-215">组所有者和成员</span><span class="sxs-lookup"><span data-stu-id="bd752-215">Group owners and membership</span></span>
* <span data-ttu-id="bd752-216">获取组对话和线索</span><span class="sxs-lookup"><span data-stu-id="bd752-216">Getting group conversations and threads</span></span>

<span data-ttu-id="bd752-217">仅支持委派权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="bd752-217">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="bd752-218">组事件、照片</span><span class="sxs-lookup"><span data-stu-id="bd752-218">Group events, photo</span></span>
* <span data-ttu-id="bd752-219">外部发件人、被接受或拒绝的发件人、组订阅</span><span class="sxs-lookup"><span data-stu-id="bd752-219">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="bd752-220">用户收藏夹和未看计数</span><span class="sxs-lookup"><span data-stu-id="bd752-220">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="bd752-221">策略</span><span class="sxs-lookup"><span data-stu-id="bd752-221">Policy</span></span>

<span data-ttu-id="bd752-222">使用 Microsoft Graph 创建并命名 Office 365 组会忽略通过 Outlook Web App 配置的所有 Office 365 组策略。</span><span class="sxs-lookup"><span data-stu-id="bd752-222">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="bd752-223">设置 allowExternalSenders 属性</span><span class="sxs-lookup"><span data-stu-id="bd752-223">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="bd752-224">目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。</span><span class="sxs-lookup"><span data-stu-id="bd752-224">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="bd752-225">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="bd752-225">Using delta query</span></span>

<span data-ttu-id="bd752-226">有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="bd752-226">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="identity-and-access--application-and-service-principal-apis"></a><span data-ttu-id="bd752-227">身份和访问 | 应用程序和服务主体 API</span><span class="sxs-lookup"><span data-stu-id="bd752-227">Identity and access | Application and service principal APIs</span></span>

<span data-ttu-id="bd752-228">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development.</span><span class="sxs-lookup"><span data-stu-id="bd752-228">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development.</span></span> <span data-ttu-id="bd752-229">The following is a summary of current limitations and in-development API features.</span><span class="sxs-lookup"><span data-stu-id="bd752-229">The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="bd752-230">当前限制：</span><span class="sxs-lookup"><span data-stu-id="bd752-230">Current limitations:</span></span>

* <span data-ttu-id="bd752-231">只有在所有更改完成后，一些应用属性（如 appRoles 和 addIns）才可用。</span><span class="sxs-lookup"><span data-stu-id="bd752-231">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="bd752-232">只能注册多租户应用。</span><span class="sxs-lookup"><span data-stu-id="bd752-232">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="bd752-233">更新应用仅限于在首次 beta更新后注册的应用。</span><span class="sxs-lookup"><span data-stu-id="bd752-233">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="bd752-234">Azure Active Directory 用户可以注册应用并添加其他所有者。</span><span class="sxs-lookup"><span data-stu-id="bd752-234">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="bd752-235">支持 OpenID Connect 和 OAuth 协议。</span><span class="sxs-lookup"><span data-stu-id="bd752-235">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="bd752-236">无法向应用分配策略。</span><span class="sxs-lookup"><span data-stu-id="bd752-236">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="bd752-237">无法对需要 appId 的 ownedObjects 执行操作（例如，users/{id|userPrincipalName}/ownedObjects/{id}/...）</span><span class="sxs-lookup"><span data-stu-id="bd752-237">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="bd752-238">处于开发阶段的功能：</span><span class="sxs-lookup"><span data-stu-id="bd752-238">In development:</span></span>

* <span data-ttu-id="bd752-239">可以注册单租户应用。</span><span class="sxs-lookup"><span data-stu-id="bd752-239">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="bd752-240">更新 servicePrincipal。</span><span class="sxs-lookup"><span data-stu-id="bd752-240">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="bd752-241">将现有 Azure AD 应用迁移到更新后的模型中。</span><span class="sxs-lookup"><span data-stu-id="bd752-241">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="bd752-242">支持 appRoles、预授权客户端、可选声明、组成员身份声明和品牌塑造</span><span class="sxs-lookup"><span data-stu-id="bd752-242">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="bd752-243">Microsoft 帐户 (MSA) 用户可以注册应用。</span><span class="sxs-lookup"><span data-stu-id="bd752-243">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="bd752-244">支持 SAML 和 WsFed 协议。</span><span class="sxs-lookup"><span data-stu-id="bd752-244">Support for SAML and WsFed protocols.</span></span>

## <a name="identity-and-access--conditional-access"></a><span data-ttu-id="bd752-245">身份和访问 | 条件访问</span><span class="sxs-lookup"><span data-stu-id="bd752-245">Identity and access | Conditional access</span></span>

### <a name="permissions"></a><span data-ttu-id="bd752-246">权限</span><span class="sxs-lookup"><span data-stu-id="bd752-246">Permissions</span></span>

<span data-ttu-id="bd752-247">目前调用 POST 和 PATCH API 需要 Policy.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="bd752-247">Currently, the Policy.Read.All permission is required to call POST and PATCH APIs.</span></span> <span data-ttu-id="bd752-248">将来可以通过 Policy.ReadWrite.ConditionalAccess 权限读取目录中的策略。</span><span class="sxs-lookup"><span data-stu-id="bd752-248">In the future, the Policy.ReadWrite.ConditionalAccess permission will enable you to read policies from the directory.</span></span>

## <a name="json-batching"></a><span data-ttu-id="bd752-249">JSON 批处理</span><span class="sxs-lookup"><span data-stu-id="bd752-249">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="bd752-250">无嵌套批处理</span><span class="sxs-lookup"><span data-stu-id="bd752-250">No nested batch</span></span>

<span data-ttu-id="bd752-251">JSON 批处理请求中不得包含任何嵌套批处理请求。</span><span class="sxs-lookup"><span data-stu-id="bd752-251">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="bd752-252">所有单个请求必须同步</span><span class="sxs-lookup"><span data-stu-id="bd752-252">All individual requests must be synchronous</span></span>

<span data-ttu-id="bd752-253">All requests contained in a batch request must be executed synchronously.</span><span class="sxs-lookup"><span data-stu-id="bd752-253">All requests contained in a batch request must be executed synchronously.</span></span> <span data-ttu-id="bd752-254">If present, the `respond-async` preference will be ignored.</span><span class="sxs-lookup"><span data-stu-id="bd752-254">If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="bd752-255">无事务</span><span class="sxs-lookup"><span data-stu-id="bd752-255">No transactions</span></span>

<span data-ttu-id="bd752-256">Microsoft Graph does not currently support transactional processing of individual requests.</span><span class="sxs-lookup"><span data-stu-id="bd752-256">Microsoft Graph does not currently support transactional processing of individual requests.</span></span> <span data-ttu-id="bd752-257">The `atomicityGroup` property on individual requests will be ignored.</span><span class="sxs-lookup"><span data-stu-id="bd752-257">The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="bd752-258">URI 必须相对</span><span class="sxs-lookup"><span data-stu-id="bd752-258">URIs must be relative</span></span>

<span data-ttu-id="bd752-259">Always specify relative URIs in batch requests.</span><span class="sxs-lookup"><span data-stu-id="bd752-259">Always specify relative URIs in batch requests.</span></span> <span data-ttu-id="bd752-260">Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span><span class="sxs-lookup"><span data-stu-id="bd752-260">Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="bd752-261">限制批处理大小</span><span class="sxs-lookup"><span data-stu-id="bd752-261">Limit on batch size</span></span>

<span data-ttu-id="bd752-262">JSON 批处理请求目前限定为 20 个单独请求。</span><span class="sxs-lookup"><span data-stu-id="bd752-262">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="bd752-263">简化的依赖项</span><span class="sxs-lookup"><span data-stu-id="bd752-263">Simplified dependencies</span></span>

<span data-ttu-id="bd752-264">Individual requests can depend on other individual requests.</span><span class="sxs-lookup"><span data-stu-id="bd752-264">Individual requests can depend on other individual requests.</span></span> <span data-ttu-id="bd752-265">Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span><span class="sxs-lookup"><span data-stu-id="bd752-265">Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="bd752-266">平行 - 没有单独的请求在 `dependsOn` 属性中声明依赖项。</span><span class="sxs-lookup"><span data-stu-id="bd752-266">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="bd752-267">串行 - 所有单独请求都依赖于之前的单独请求。</span><span class="sxs-lookup"><span data-stu-id="bd752-267">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="bd752-268">相同 - 在 `dependsOn` 属性中声明依赖项的所有单独请求均声明了相同的依赖项。</span><span class="sxs-lookup"><span data-stu-id="bd752-268">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="bd752-269">随着 JSON 批处理技术日臻成熟，这些限制将会被取消。</span><span class="sxs-lookup"><span data-stu-id="bd752-269">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="mail-outlook"></a><span data-ttu-id="bd752-270">邮件 (Outlook)</span><span class="sxs-lookup"><span data-stu-id="bd752-270">Mail (Outlook)</span></span>

### <a name="attaching-large-files-to-messages"></a><span data-ttu-id="bd752-271">将大型文件附加到邮件</span><span class="sxs-lookup"><span data-stu-id="bd752-271">Attaching large files to messages</span></span>
<span data-ttu-id="bd752-272">尝试[将大型文件附加](outlook-large-attachments.md)到共享或委派的邮箱中的 Outlook 邮件或事件时，具有委派权限的应用将返回 `HTTP 403 Forbidden`。</span><span class="sxs-lookup"><span data-stu-id="bd752-272">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="bd752-273">使用委派权限，仅当邮件或事件在已登录用户的邮箱中时，[createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) 才会成功。</span><span class="sxs-lookup"><span data-stu-id="bd752-273">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="bd752-274">用于创建草稿的注释参数</span><span class="sxs-lookup"><span data-stu-id="bd752-274">The comment parameter for creating a draft</span></span>

<span data-ttu-id="bd752-275">用于创建答复或转发草稿的**注释**参数（[createReply](/graph/api/message-createreply?view=graph-rest-1.0)、[createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0)、[createForward](/graph/api/message-createforward?view=graph-rest-1.0)）不会成为最终的邮件草稿正文的一部分。</span><span class="sxs-lookup"><span data-stu-id="bd752-275">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="bd752-276">GET 消息返回 Microsoft Teams 中的聊天</span><span class="sxs-lookup"><span data-stu-id="bd752-276">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="bd752-277">在 v1 和 beta 终结点中，`GET /users/id/messages` 的响应包含出现在团队或通道范围外的用户的 Microsoft Teams 聊天。</span><span class="sxs-lookup"><span data-stu-id="bd752-277">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="bd752-278">这些聊天消息具有“即时信息”作为其主题。</span><span class="sxs-lookup"><span data-stu-id="bd752-278">These chat messages have "IM" as their subject.</span></span>

## <a name="teamwork-microsoft-teams"></a><span data-ttu-id="bd752-279">团队合作 (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="bd752-279">Teamwork (Microsoft Teams)</span></span>

### <a name="get-teams-is-not-supported"></a><span data-ttu-id="bd752-280">不支持 GET /teams</span><span class="sxs-lookup"><span data-stu-id="bd752-280">GET /teams is not supported</span></span>

<span data-ttu-id="bd752-281">若要获取团队列表，请参阅[列出所有团队](teams-list-all-teams.md)和[列出你的团队](/graph/api/user-list-joinedteams?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="bd752-281">To get a list of teams, see [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0).</span></span>

### <a name="post-teams-is-only-available-in-beta"></a><span data-ttu-id="bd752-282">POST /teams 仅适用于 beta 版</span><span class="sxs-lookup"><span data-stu-id="bd752-282">POST /teams is only available in beta</span></span>
<span data-ttu-id="bd752-283">若要在 v1.0 中创建团队，请参阅[创建团队](/graph/api/team-put-teams?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="bd752-283">To create teams in v1.0, see [create team](/graph/api/team-put-teams?view=graph-rest-1.0).</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="bd752-284">“列出所有团队”没有列出的团队</span><span class="sxs-lookup"><span data-stu-id="bd752-284">Missing teams in list all teams</span></span>

<span data-ttu-id="bd752-285">[列出所有团队](teams-list-all-teams.md)没有列出过去创建但 Microsoft Teams 用户最近未使用的一些团队。</span><span class="sxs-lookup"><span data-stu-id="bd752-285">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="bd752-286">新团队会被列出。</span><span class="sxs-lookup"><span data-stu-id="bd752-286">New teams will be listed.</span></span>
<span data-ttu-id="bd752-287">一些旧团队没有包含“Team”的 **resourceProvisioningOptions** 属性，但新创建的团队和在 Microsoft Teams 中被访问的团队有此属性。</span><span class="sxs-lookup"><span data-stu-id="bd752-287">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="bd752-288">今后，我们将对尚未在 Microsoft Teams 中打开的现有团队设置 **resourceProvisioningOptions**。</span><span class="sxs-lookup"><span data-stu-id="bd752-288">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="users"></a><span data-ttu-id="bd752-289">用户</span><span class="sxs-lookup"><span data-stu-id="bd752-289">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="bd752-290">创建后无法即时访问</span><span class="sxs-lookup"><span data-stu-id="bd752-290">No instant access after creation</span></span>

<span data-ttu-id="bd752-291">Users can be created immediately through a POST on the user entity.</span><span class="sxs-lookup"><span data-stu-id="bd752-291">Users can be created immediately through a POST on the user entity.</span></span> <span data-ttu-id="bd752-292">An Office 365 license must first be assigned to a user, in order to get access to Office 365 services.</span><span class="sxs-lookup"><span data-stu-id="bd752-292">An Office 365 license must first be assigned to a user, in order to get access to Office 365 services.</span></span> <span data-ttu-id="bd752-293">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="bd752-293">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span></span> <span data-ttu-id="bd752-294">During this time, apps will receive a 404 HTTP error response.</span><span class="sxs-lookup"><span data-stu-id="bd752-294">During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="bd752-295">照片限制</span><span class="sxs-lookup"><span data-stu-id="bd752-295">Photo restrictions</span></span>

<span data-ttu-id="bd752-296">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span><span class="sxs-lookup"><span data-stu-id="bd752-296">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span></span> <span data-ttu-id="bd752-297">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.</span><span class="sxs-lookup"><span data-stu-id="bd752-297">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.</span></span>
<span data-ttu-id="bd752-298">Failure to read or update a photo, in this case, would result in the following error:</span><span class="sxs-lookup"><span data-stu-id="bd752-298">Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a><span data-ttu-id="bd752-299">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="bd752-299">Using delta query</span></span>

<span data-ttu-id="bd752-300">有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="bd752-300">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="bd752-301">调用登录会话返回了错误的 HTTP 代码</span><span class="sxs-lookup"><span data-stu-id="bd752-301">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="bd752-302">[用户: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) 返回 `204 No content` 响应表示成功调用；如果请求出现任何错误，则返回 HTTP 错误代码（4xx 或 5xx）。</span><span class="sxs-lookup"><span data-stu-id="bd752-302">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="bd752-303">但是，由于服务问题，此 API 会返回 `200 OK` 和始终为 true 的布尔值参数。</span><span class="sxs-lookup"><span data-stu-id="bd752-303">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="bd752-304">在此问题得到修复之前，简单建议开发人员将所有 2xx 返回代码看作此 API 成功。</span><span class="sxs-lookup"><span data-stu-id="bd752-304">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

### <a name="incomplete-objects-when-using-getbyids-request"></a><span data-ttu-id="bd752-305">使用 getByIds 请求时对象完整</span><span class="sxs-lookup"><span data-stu-id="bd752-305">Incomplete objects when using getByIds request</span></span>

<span data-ttu-id="bd752-306">使用[获取 ID 列表中的目录对象](/graph/api/directoryobject-getbyids?view=graph-rest-1.0)请求对象应返回完整对象。</span><span class="sxs-lookup"><span data-stu-id="bd752-306">Requesting objects using [Get directory objects from a list of IDs](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) should return full objects.</span></span> <span data-ttu-id="bd752-307">但是，当前返回的 v1.0 端点上的[用户](/graph/api/resources/user?view=graph-rest-1.0)对象具有一组有限的属性。</span><span class="sxs-lookup"><span data-stu-id="bd752-307">However, currently [user](/graph/api/resources/user?view=graph-rest-1.0) objects on the v1.0 endpoint are returned with a limited set of properties.</span></span> <span data-ttu-id="bd752-308">作为临时解决方法，当您将该操作与 `$select` 查询选项结合使用时, 将返回更完整的[用户](/graph/api/resources/user?view=graph-rest-1.0)对象。</span><span class="sxs-lookup"><span data-stu-id="bd752-308">As a temporary workaround, when you use the operation in combination with the `$select` query option, more complete [user](/graph/api/resources/user?view=graph-rest-1.0) objects will be returned.</span></span> <span data-ttu-id="bd752-309">此行为不符合 OData 规范。</span><span class="sxs-lookup"><span data-stu-id="bd752-309">This behavior is not in accordance with the OData specifications.</span></span> <span data-ttu-id="bd752-310">由于此行为可能在将来更新，因此仅在你提供 `$select=` 以及感兴趣的所有属性时，并且仅当此解决方法的未来重大更改可接受时，才使用此解决方法。</span><span class="sxs-lookup"><span data-stu-id="bd752-310">Because this behavior might be updated in the future, use this workaround only when you provide `$select=` with all the properties you are interested in, and only if future breaking changes to this workaround are acceptable.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="bd752-311">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="bd752-311">Query parameter limitations</span></span>

* <span data-ttu-id="bd752-312">不支持多个命名空间。</span><span class="sxs-lookup"><span data-stu-id="bd752-312">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="bd752-313">在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行 GET 操作和投影。</span><span class="sxs-lookup"><span data-stu-id="bd752-313">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="bd752-314">`@odata.bind` is not supported.</span><span class="sxs-lookup"><span data-stu-id="bd752-314">`@odata.bind` is not supported.</span></span>  <span data-ttu-id="bd752-315">This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span><span class="sxs-lookup"><span data-stu-id="bd752-315">This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="bd752-316">使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`。</span><span class="sxs-lookup"><span data-stu-id="bd752-316">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="bd752-317">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="bd752-317">`$expand`:</span></span>
  * <span data-ttu-id="bd752-318">不支持 `nextLink`</span><span class="sxs-lookup"><span data-stu-id="bd752-318">No support for `nextLink`</span></span>
  * <span data-ttu-id="bd752-319">不支持 1 级以上扩展</span><span class="sxs-lookup"><span data-stu-id="bd752-319">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="bd752-320">不支持其他参数（`$filter`、`$select`）</span><span class="sxs-lookup"><span data-stu-id="bd752-320">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="bd752-321">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="bd752-321">`$filter`:</span></span>
  * <span data-ttu-id="bd752-322">`/attachments` 终结点不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="bd752-322">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="bd752-323">如果存在，将忽略 `$filter` 参数。</span><span class="sxs-lookup"><span data-stu-id="bd752-323">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="bd752-324">不支持跨工作负载筛选。</span><span class="sxs-lookup"><span data-stu-id="bd752-324">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="bd752-325">`$search`:</span><span class="sxs-lookup"><span data-stu-id="bd752-325">`$search`:</span></span>
  * <span data-ttu-id="bd752-326">全文搜索仅对实体子集（如邮件）可用。</span><span class="sxs-lookup"><span data-stu-id="bd752-326">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="bd752-327">不支持跨工作负载搜索。</span><span class="sxs-lookup"><span data-stu-id="bd752-327">Cross-workload searching is not supported.</span></span>


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="bd752-328">只有 Office 365 REST 或 Azure AD Graph API 才具有的功能</span><span class="sxs-lookup"><span data-stu-id="bd752-328">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="bd752-329">某些功能尚未在 Microsoft Graph 中提供。</span><span class="sxs-lookup"><span data-stu-id="bd752-329">Some functionality is not yet available in Microsoft Graph.</span></span> <span data-ttu-id="bd752-330">如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](https://docs.microsoft.com/previous-versions/office/office-365-api/)。</span><span class="sxs-lookup"><span data-stu-id="bd752-330">If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://docs.microsoft.com/previous-versions/office/office-365-api/).</span></span> <span data-ttu-id="bd752-331">有关 Azure Active Directory 的信息，请参阅[将 Azure AD Graph 应用迁移到 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)。</span><span class="sxs-lookup"><span data-stu-id="bd752-331">For Azure Active Directory, see [Migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span> 
