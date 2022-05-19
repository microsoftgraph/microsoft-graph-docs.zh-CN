---
title: 'Exchange Web 服务 (到 Microsoft 图形 API 映射的 EWS) '
description: 本文列出了映射到 Exchange Web 服务 (EWS) API 的 Microsoft Graph API。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 93ecef5daccc29743a74258eae1624e8e78dcd4f
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549608"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange Web 服务 (到 Microsoft 图形 API 映射的 EWS) 

本文列出了映射到 Exchange Web 服务 (EWS) API 的 Microsoft Graph API。

## <a name="utility-apis"></a>实用工具 API

| EWS API                                                                                             | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [转换Exchange ID](/graph/api/user-translateexchangeids) |
| [ResolveNames](/exchange/client-developer/web-service-reference/resolvenames-operation)             | [列出人员](/graph/api/user-list-people) |
| [GetServerTimeZones](/exchange/client-developer/web-service-reference/getservertimezones-operation) | [获取时区选择](/graph/api/outlookuser-supportedtimezones) |

## <a name="mail-apis"></a>邮件 API

### <a name="messages"></a>消息

| EWS API                                                                             | Microsoft Graph API |
|-------------------------------------------------------------------------------------|-----|
| [CreateItem](/exchange/client-developer/web-service-reference/createitem-operation) | [创建邮件](/graph/api/user-post-messages) |
| [CopyItem](/exchange/client-developer/web-service-reference/copyitem-operation)     | [复制消息](/graph/api/message-copy) |
| [DeleteItem](/exchange/client-developer/web-service-reference/deleteitem-operation) | [删除邮件](/graph/api/message-delete) |
| [FindItem](/exchange/client-developer/web-service-reference/finditem-operation)     | [列出邮件](/graph/api/user-list-messages) |
| [GetItem](/exchange/client-developer/web-service-reference/getitem-operation)       | [获取邮件](/graph/api/message-get) |
| [MoveItem](/exchange/client-developer/web-service-reference/moveitem-operation)     | [移动消息](/graph/api/message-move) |
| [SendItem](/exchange/client-developer/web-service-reference/senditem-operation)     | [发送邮件](/graph/api/message-send) 或 [发送邮件](/graph/api/user-sendmail) |
| [UpdateItem](/exchange/client-developer/web-service-reference/updateitem-operation) | [更新邮件](/graph/api/message-update) |

### <a name="folders"></a>Folders

| EWS API                                                                                 | Microsoft Graph API |
|-----------------------------------------------------------------------------------------|-----|
| [CreateFolder](/exchange/client-developer/web-service-reference/createfolder-operation) | [创建邮件文件夹](/graph/api/user-post-mailfolders) |
| [CopyFolder](/exchange/client-developer/web-service-reference/copyfolder-operation)     | [复制邮件文件夹](/graph/api/mailfolder-copy) |
| [DeleteFolder](/exchange/client-developer/web-service-reference/deletefolder-operation) | [删除邮件文件夹](/graph/api/mailfolder-delete) |
| [GetFolder](/exchange/client-developer/web-service-reference/getfolder-operation)       | [获取邮件文件夹](/graph/api/mailfolder-get) |
| [MoveFolder](/exchange/client-developer/web-service-reference/movefolder-operation)     | [移动邮件文件夹](/graph/api/mailfolder-move) |
| [UpdateFolder](/exchange/client-developer/web-service-reference/updatefolder-operation) | [更新邮件文件夹](/graph/api/mailfolder-update) |

### <a name="attachments"></a>附件

| EWS API                                                                                         | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------|-----|
| [CreateAttachment](/exchange/client-developer/web-service-reference/createattachment-operation) | [添加附件](/graph/api/message-post-attachments) |
| [GetAttachment](/exchange/client-developer/web-service-reference/getattachment-operation)       | [获取附件](/graph/api/attachment-get) |
| [DeleteAttachment](/exchange/client-developer/web-service-reference/deleteattachment-operation) | [删除附件](/graph/api/attachment-delete) |

### <a name="rules"></a>Rules

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                         | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------|-----|
| [GetInboxRules](/exchange/client-developer/web-service-reference/getinboxrules-operation)       | [List rules](/graph/api/mailfolder-list-messagerules) |
| [UpdateInboxRules](/exchange/client-developer/web-service-reference/updateinboxrules-operation) | [创建规则](/graph/api/mailfolder-post-messagerules)<br/>[更新规则](/graph/api/messagerule-update)<br/>[删除规则](/graph/api/messagerule-delete) |
<!-- markdownlint-enable MD033 -->

### <a name="mailtips"></a>MailTips

| EWS API                                                                               | Microsoft Graph API |
|---------------------------------------------------------------------------------------|-----|
| [GetMailTips](/exchange/client-developer/web-service-reference/getmailtips-operation) | [获取邮件提醒](/graph/api/user-getmailtips) |

### <a name="out-of-office-oof-settings"></a>Office (OOF) 设置

| EWS API                                                                                             | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------|-----|
| [GetUserOofSettings](/exchange/client-developer/web-service-reference/getuseroofsettings-operation) | [获取用户的邮箱设置](/graph/api/user-get-mailboxsettings) |
| [SetUserOofSettings](/exchange/client-developer/web-service-reference/setuseroofsettings-operation) | [更新用户邮箱设置](/graph/api/user-update-mailboxsettings) |

### <a name="notifications"></a>通知

> [!NOTE]
> Microsoft Graph仅要求订阅推送通知。 如果当前使用的是 [EWS 拉取通知](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange)，请参阅 [“获取消息增量](/graph/api/message-delta)”。

| EWS API                                                                                                    | Microsoft Graph API |
|------------------------------------------------------------------------------------------------------------|-----|
| [GetEvents](/exchange/client-developer/web-service-reference/getevents-operation)                          | [获取消息增量](/graph/api/message-delta) |
| [订阅](/exchange/client-developer/web-service-reference/subscribe-operation) (推送通知)      | [创建订阅](/graph/api/subscription-post-subscriptions) |
| [取消订阅](/exchange/client-developer/web-service-reference/unsubscribe-operation) (推送通知)  | [删除订阅](/graph/api/subscription-delete) |

### <a name="synchronization"></a>同步

| EWS API                                                                                               | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------------|-----|
| [SyncFolderHierarchy](/exchange/client-developer/web-service-reference/syncfolderhierarchy-operation) | [获取邮件文件夹 Delta](/graph/api/mailfolder-delta) |
| [SyncFolderItems](/exchange/client-developer/web-service-reference/syncfolderitems-operation)         | [获取消息增量](/graph/api/message-delta) |

## <a name="calendar-apis"></a>日历 API

### <a name="availability"></a>可用性

| EWS API                                                                                               | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation)<br/>FindAvailableMeetingTimes | [获取忙/闲日程安排](/graph/api/calendar-getschedule)|
 

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [提醒视图](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [关闭提醒](/graph/api/event-dismissreminder)<br/>[推迟提醒](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->

### <a name="permissions"></a>权限

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [提醒视图](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [关闭提醒](/graph/api/event-dismissreminder)<br/>[推迟提醒](/graph/api/event-snoozereminder) |
|CreateSharingPermission，GetSharingPermission | [日历所有者：获取共享或委派信息及权限](outlook-share-or-delegate-calendar.md#calendar-owner-get-sharing-or-delegation-information-and-permissions)|
|UpdateSharingPermission | [获取有关共享者和委托人的日历信息，以及更新各个权限](outlook-share-or-delegate-calendar.md#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions)|
|DeleteSharingPermission| [删除日历的共享或委托](outlook-share-or-delegate-calendar.md#delete-a-sharee-or-delegate-of-a-calendar)|
|GetSharingPermissionInfo | [日历所有者：获取共享或委托日历的属性](outlook-share-or-delegate-calendar.md#get-properties-of-a-shared-or-delegated-calendar)|

### <a name="invitations"></a>邀请
| EWS API                                                                                                   | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------------|-----|
|ActivateSharingInvitation | [在 Outlook 中共享或委派日历](/graph/outlook-share-or-delegate-calendar)|
|GetSharingInvitation | [共享者：直接从日历所有者的邮箱获取共享日历或其事件](outlook-get-shared-events-calendars.md#sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox)|
|DeleteSharingInvitation | [日历所有者：在日历上更新现有共享者或委托人的权限](outlook-share-or-delegate-calendar.md#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)|
|CreateSharingInvitation | [在共享或委托的日历中创建 Outlook 事件](outlook-create-event-in-shared-delegated-calendar.md#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf)|

### <a name="shared-information"></a>共享信息
| EWS API                                                                                                   | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------------|-----|
| GetCalendarSharedInformation，GetConsumerCalendarSharedInformation | [List calendars](/graph/api/user-list-calendars) |
## <a name="groups-apis"></a>组 API

| EWS API                                                                                               | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------------|-----|
| GetUserUnifiedGroups | [List memberof](/graph/api/user-list-memberof) |
| GetUnifiedGroupsSettings | [groupSetting](/graph/api/resources/groupsetting) |
| GetUnifiedGroupDetails | [Get group](/graph/api/group-get) |
| GetUnifiedGroupMembers | [List members](/graph/api/group-list-members) |
| GetUnifiedGroupUnseenCount | [Get group](/graph/api/group-get) |
| SetUnifiedGroupMembershipState | [添加/删除成员/所有者](/graph/api/resources/group) |
| FindUnifiedGroups | [列出组](/graph/api/group-list) |
| SetUnifiedGroupUserSubscribeState | [Subscribe/unsubscribeByMail](/graph/api/group-subscribebymail) |
| UpdateUnifiedGroup | [更新组](/graph/api/group-update) |
| CreateUnifiedGroup | [Create group](/graph/api/group-post-groups) |
| RemoveUnifiedGroup | [删除组](/graph/api/group-delete) |
| SetUnifiedGroupFavoriteState | [Group addFavorite](/graph/api/group-addfavorite) |
| JoinPrivateUnifiedGroup | [Subscribe/unsubscribeByMail](/graph/api/group-subscribebymail) |
| GetDlMembersForUnifiedGroup | [List group members](/graph/api/group-list-members) |
