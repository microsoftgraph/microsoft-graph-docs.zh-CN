---
title: Exchange Web 服务 (EWS) Microsoft Graph API 映射
description: 本文列出了映射到 EWS Graph EWS Exchange的 Microsoft (API) API。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 89aa884baf0ae5d2a67d31f3e28d4c818be2c9af
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516552"
---
# <a name="exchange-web-services-ews-to-microsoft-graph-api-mappings"></a>Exchange Web 服务 (EWS) Microsoft Graph API 映射

本文列出了映射到 EWS Graph EWS Exchange的 Microsoft (API) API。

## <a name="utility-apis"></a>实用程序 API

| EWS API                                                                                             | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------|-----|
| [ConvertId](/exchange/client-developer/web-service-reference/convertid-operation)                   | [翻译Exchange ID](/graph/api/user-translateexchangeids) |
| [ResolveNames](/exchange/client-developer/web-service-reference/resolvenames-operation)             | [列出人员](/graph/api/user-list-people) |
| [GetServerTimeZones](/exchange/client-developer/web-service-reference/getservertimezones-operation) | [获取时区选择](/graph/api/outlookuser-supportedtimezones) |

## <a name="mail-apis"></a>邮件 API

### <a name="messages"></a>消息

| EWS API                                                                             | Microsoft Graph API |
|-------------------------------------------------------------------------------------|-----|
| [CreateItem](/exchange/client-developer/web-service-reference/createitem-operation) | [创建邮件](/graph/api/user-post-messages) |
| [CopyItem](/exchange/client-developer/web-service-reference/copyitem-operation)     | [复制邮件](/graph/api/message-copy) |
| [DeleteItem](/exchange/client-developer/web-service-reference/deleteitem-operation) | [删除邮件](/graph/api/message-delete) |
| [FindItem](/exchange/client-developer/web-service-reference/finditem-operation)     | [列出邮件](/graph/api/user-list-messages) |
| [GetItem](/exchange/client-developer/web-service-reference/getitem-operation)       | [获取邮件](/graph/api/message-get) |
| [MoveItem](/exchange/client-developer/web-service-reference/moveitem-operation)     | [移动邮件](/graph/api/message-move) |
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

### <a name="attachments"></a>Attachments

| EWS API                                                                                         | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------|-----|
| [CreateAttachment](/exchange/client-developer/web-service-reference/createattachment-operation) | [Add attachment](/graph/api/message-post-attachments) |
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

### <a name="out-of-office-oof-settings"></a>Out of Office (OOF) settings

| EWS API                                                                                             | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------|-----|
| [GetUserOofSettings](/exchange/client-developer/web-service-reference/getuseroofsettings-operation) | [获取用户的邮箱设置](/graph/api/user-get-mailboxsettings) |
| [SetUserOofSettings](/exchange/client-developer/web-service-reference/setuseroofsettings-operation) | [更新用户邮箱设置](/graph/api/user-update-mailboxsettings) |

### <a name="notifications"></a>通知

> [!NOTE]
> Microsoft Graph只需订阅推送通知。 如果当前正在使用 [EWS 拉取通知，](/exchange/client-developer/exchange-web-services/how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange)请参阅 [获取邮件增量](/graph/api/message-delta)。

| EWS API                                                                                                    | Microsoft Graph API |
|------------------------------------------------------------------------------------------------------------|-----|
| [GetEvents](/exchange/client-developer/web-service-reference/getevents-operation)                          | [获取邮件增量](/graph/api/message-delta) |
| [订阅](/exchange/client-developer/web-service-reference/subscribe-operation) (推送通知)      | [创建订阅](/graph/api/subscription-post-subscriptions) |
| [取消](/exchange/client-developer/web-service-reference/unsubscribe-operation) (推送通知)  | [删除订阅](/graph/api/subscription-delete) |

### <a name="synchronization"></a>同步

| EWS API                                                                                               | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------------|-----|
| [SyncFolderHierarchy](/exchange/client-developer/web-service-reference/syncfolderhierarchy-operation) | [获取邮件文件夹 Delta](/graph/api/mailfolder-delta) |
| [SyncFolderItems](/exchange/client-developer/web-service-reference/syncfolderitems-operation)         | [获取邮件增量](/graph/api/message-delta) |

## <a name="calendar-apis"></a>日历 API

### <a name="availability"></a>可用性

| EWS API                                                                                               | Microsoft Graph API |
|-------------------------------------------------------------------------------------------------------|-----|
| [GetUserAvailability](/exchange/client-developer/web-service-reference/getuseravailability-operation) | [获取忙/闲日程安排](/graph/api/calendar-getschedule) |

### <a name="reminders"></a>Reminders

<!-- markdownlint-disable MD033 -->
| EWS API                                                                                                   | Microsoft Graph API |
|-----------------------------------------------------------------------------------------------------------|-----|
| [GetReminders](/exchange/client-developer/web-service-reference/getreminders-operation)                   | [提醒视图](/graph/api/user-reminderview) |
| [PerformReminderAction](/exchange/client-developer/web-service-reference/performreminderaction-operation) | [关闭提醒](/graph/api/event-dismissreminder)<br/>[推迟提醒](/graph/api/event-snoozereminder) |
<!-- markdownlint-enable MD033 -->
