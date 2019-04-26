---
title: 使用 Outlook 邮件 REST API
description: Microsoft Graph 可让应用程序获得对个人或组织帐户中用户的 Outlook 邮件数据的授权访问权限。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dc7f1a0fc4ffb26986e3b1adc6b672749b24f27d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525409"
---
# <a name="use-the-outlook-mail-rest-api"></a>使用 Outlook 邮件 REST API

Microsoft Graph 可让你的应用获得授权，访问个人或组织帐户中的用户的 Outlook 邮件数据。使用[适当的委派或应用程序权限](/graph/permissions-reference)，你的应用程序可以访问已登录用户或租户中任何用户的邮件数据。邮件数据可以位于 Exchange Online 上的云中，作为 Office 365 的一部分，或位于[混合部署](/graph/hybrid-rest-support)中的 Exchange 内部部署上。

## <a name="using-the-mail-rest-api"></a>使用邮件 REST API

代表[用户](../resources/user.md)执行可由用户的 **id** 属性（唯一的 GUID）、电子邮件地址或`me`已登录用户的快捷方式别名标识的邮件 API 请求。

电子邮件由[邮件](../resources/message.md)资源表示，放在 [mailFolder](../resources/mailfolder.md) 中。邮件和邮件文件夹由其 **id** 属性标识，可通过 `GET` 操作获取。

>**注意：** 通常，请不要假定邮箱内的**邮件**和 **mailFolder** 具有唯一且不可变的 ID。在执行如复制、移动或发送等某些操作后，它们可能会发生更改。

邮件正文可以是 HTML 格式或文本格式。

你可以使用已知的文件夹名称，如 `Inbox`、`Drafts`、`SentItems` 或 `DeletedItems`，来识别某些对所有用户默认存在的邮件文件夹。 有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。

例如，你可以从已登录用户的 Outlook“**已发送邮件**”文件夹收取邮件，无需事先获取文件夹 ID：

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>常见用例

**邮件**资源公开如**类别**、**conversationId**、**标记**以及**重要性**等属性，这些属性对应于 UI 中的可用功能，允许应用自动化或与内置 Outlook 用户体验集成。

Microsoft Graph API 还提供支持邮件常见用例的方法和操作。

| 用例 | REST 资源 | 另请参阅 |
|:----------|:---------------|:---------|
| **以用户为中心的操作** | | |
| 起草、阅读、答复、转发、发送、更新或删除邮件 | [邮件](../resources/message.md) | [邮件的方法](../resources/message.md#methods) |
| 代表邮箱所有者委托其他用户发送邮件 | [邮件](../resources/message.md) | 正在设置[邮件](../resources/message.md)的**发件人**和**收件人**属性 |
| 让用户先查看更重要的邮件 | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [重点收件箱](../resources/manage-focused-inbox.md) |
| 添加、获取或删除邮件的附件 | [附件](../resources/attachment.md)、 <br> [fileAttachment](../resources/fileattachment.md)、 <br> [itemAttachment](../resources/itemattachment.md)、 <br> [referenceAttachment](../resources/referenceattachment.md)、 <br> [邮件](../resources/message.md) | [附件的方法](../resources/attachment.md#methods) |
| 获取或更新用户的自动答复、区域设置、时区或工作时间 | [mailboxSettings](../resources/mailboxsettings.md)、 <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md)、 <br> [localeInfo](../resources/localeinfo.md)、 <br> [workingHours](../resources/workinghours.md) | [获取用户的邮箱设置](../api/user-get-mailboxsettings.md)、 <br> [更新用户的邮箱设置](../api/user-update-mailboxsettings.md) |
| 获取其他收件人的特殊状态（例如外出）的邮件提醒 | [user](../resources/user.md)、 <br> [mailTips](../resources/mailtips.md) | [获取邮件提醒](../api/user-getmailtips.md) |
| **邮件和文件夹管理** | | |
| 组织邮件文件夹层次结构中的邮件 | [mailFolder](../resources/mailfolder.md)  | [MailFolder 的方法](../resources/mailfolder.md#methods) |
| 搜索和筛选邮件 | [邮件](../resources/message.md) | [查询参数](/graph/query-parameters)  |
| 获取对文件夹中的邮件更改的通知 | [订阅](../resources/subscription.md) | [在 Microsoft Graph 中使用 Webhooks](../resources/webhooks.md) |
| 同步邮件或邮件文件夹层次结构 | [邮件](../resources/message.md) | [获取文件夹中邮件的增量更改](/graph/delta-query-messages) |
| **应用开发** | | |
| 添加自定义应用数据作为邮件的 Internet 邮件头 | [邮件](../resources/message.md) | 向邮件的 **internetMessageHeaders** 属性添加自定义数据。 |
| 通过使用扩展向邮件添加自定义应用数据 | [openTypeExtension](../resources/opentypeextension.md)、 <br>[schemaExtension](../resources/schemaextension.md) | [使用扩展向资源添加自定义数据](/graph/extensibility-overview) |
| 访问半公开的 Outlook MAPI 属性的自定义数据 | [SingleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、 <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Outlook 扩展属性概述](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>后续步骤

邮件 API 可以为你开辟与用户互动的新途径：

- [Outlook 邮件 API 概述](/graph/outlook-mail-concept-overview)
- 向下钻取[邮件](../resources/message.md)和 [mailFolder](../resources/mailfolder.md) 资源的[方法](../resources/message.md#methods)、[属性](../resources/message.md#properties)和[关系](../resources/message.md#relationships)。
- 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。
