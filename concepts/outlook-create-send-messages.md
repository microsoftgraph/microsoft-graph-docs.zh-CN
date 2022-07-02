---
title: 使用 Outlook 邮件 API 自动创建、发送、处理邮件
description: 电子邮件由 Microsoft Graph 中 Outlook 邮件 API 中的邮件资源表示。 你可以创建和发送邮件、检查收件人状态等。
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 63470b3910837e08baee01881a070b9ee708c9bd
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556183"
---
# <a name="automate-creating-sending-and-processing-messages"></a>自动创建、发送和处理邮件

电子邮件通过 Microsoft Graph 中的[邮件](/graph/api/resources/message)资源表示。

默认情况下，邮件由 **ID** 属性中的唯一条目 ID 标识。 当最初创建、保存为草稿或发送邮件时，存储提供程序会为邮件分配一个条目 ID。 默认情况下，当将邮件复制或移动到另一个文件夹、存储空间或 .PST 文件时，该 ID 会发生变化。 可以通过当前 ID 引用邮件，以便后续处理。

## <a name="create-and-send-mail"></a>创建和发送邮件

在 Outlook 中，你可以在同一 [sendMail](/graph/api/user-sendmail) 操作中创建和发送电子邮件，或者可以[创建](/graph/api/user-post-messages)草稿，然后[添加内容](/graph/api/message-update)并[发送](/graph/api/message-send)此草稿。

同样，在回复电子邮件时，也可以使用相同的操作（[答复](/graph/api/message-reply)、[全部答复](/graph/api/message-replyall)或[转发](/graph/api/message-forward)）创建和发送响应。 或者，你可以为响应（[答复](/graph/api/message-createreply)、[全部答复](/graph/api/message-createreplyall)或[转发](/graph/api/message-createforward)）创建草稿，[添加内容](/graph/api/message-update)），然后稍后[发送](/graph/api/message-send)此草稿。

要以编程方式区分草稿和已发送邮件，请选中 **isDraft** 属性。

默认情况下，草稿邮件保存在 `Drafts` 文件夹中，已发送邮件保存在 `Sent Items` 文件夹中。 为方便起见，可以通过相应的[已知文件夹名称](/graph/api/resources/mailfolder)来识别 Drafts 文件夹和 SentItems 文件夹。

### <a name="set-the-from-and-sender-properties"></a>设置 from 和 sender 属性

撰写邮件时，在大多数情况下，Outlook 会将 **from** 和 **sender** 属性设置为同一登录用户。可以在以下方案中更新这些属性：

- 如果 Exchange 管理员已将邮箱的 **sendAs** 权限分配给其他一些用户，可以更改 **from** 属性。为此，管理员可以在 Azure 门户中选择邮箱所有者的 **邮箱权限**，也可以使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet。然后，可以编程方式将 **from** 属性设置为，对相应邮箱拥有 **sendAs** 权限的用户之一。
- 如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **Sender** 属性。邮箱所有者可以在 Outlook 中委派。当代理代表邮箱所有者发送邮件时，Outlook 将 **Sender** 属性设置为代理的帐户，而 **from** 属性仍保持为邮箱所有者。可以通过编程方式将 **Sender** 属性设置为拥有该邮箱代理权限的用户。

## <a name="use-mailtips-to-check-recipient-status-and-save-time-preview"></a>使用邮件提醒检查收件人状态并节省时间（预览版）

使用 [邮件提醒](/graph/api/resources/mailtips) 以在发送电子邮件之前做出明智决策。邮件提醒可以告诉你信息，例如收件人的邮箱仅限于特定发件人，或者向该收件人发送电子邮件需要审批。


## <a name="read-messages-with-control-over-the-body-format-returned"></a>阅读邮件并控制返回的正文格式

可以通过引用邮件 ID 来[阅读邮箱中的邮件](/graph/api/message-get)：

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

或者，也可以[获取特定文件夹中的邮件](/graph/api/user-list-messages)。 例如，阅读单点登录用户的“草稿”文件夹中的邮件：

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

Outlook 邮件正文可以是 HTML 或文本，其中 HTML 作为 GET 响应中返回的默认邮件正文类型。

获取邮件时，你可以指定以下请求标头以文本格式返回 **body** 和 **uniqueBody** 属性：

```http
Prefer: outlook.body-content-type="text"
```

你可以指定以下标头（或直接跳过标头），以 HTML 格式获取邮件正文：

```http
Prefer: outlook.body-content-type="html"
```

当指定任一标头时，成功的响应将包含相应的 `Preference-Applied` 标头：

- 对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`
- 对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`

默认情况下，如果正文是 HTML 格式，那么在 REST 响应中返回正文内容之前，Outlook 将删除嵌入 **body** 属性中的任何具有潜在不安全性的 HTML（例如 JavaScript）。

若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrate-with--social-gesture-preview"></a>与“@”社交手势集成（预览版）

@-mention 是提醒用户邮件中是否有提到他们的通知。 [mention](/graph/api/resources/mention?view=graph-rest-beta&preserve-view=true)资源使应用能够在电子邮件中设置和获取常见的在线社交手势，即“@”前缀。
可以执行下列操作：

- 在[创建邮件](/graph/api/user-post-messages?view=graph-rest-beta&preserve-view=true#request-2)时创建 @-mention
- [获取用户邮箱中包含用户 @-mention 的所有邮件](/graph/api/user-list-messages?view=graph-rest-beta&preserve-view=true#request-2)
- [获取所有 @-mention 就形成一封邮件](/graph/api/message-get?view=graph-rest-beta&preserve-view=true#request-2)

## <a name="other-shared-capabilities"></a>其他共享的功能

利用以下在 Microsoft Graph 实体之间共享的常用功能：

- 发生一种或多种类型的更改时（如创建或更新邮件），订阅邮件的[更改通知](/graph/api/resources/webhooks)。
- [跟踪文件夹中邮件的增量更改](delta-query-messages.md)。
- 创建[开放扩展](extensibility-overview.md#4-open-extensions)或[架构扩展](extensibility-overview.md#3-schema-extensions)，以将自定义数据添加到邮件实例。
- 当 Outlook MAPI 属性尚未通过 Microsoft Graph API 元数据公开时，在邮件实例中创建[扩展属性](/graph/api/resources/extended-properties-overview)以存储这些属性的自定义数据。

## <a name="next-steps"></a>后续步骤

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [获取 MIME 内容（预览版）](outlook-get-mime-message.md)
- [获取共享邮件](outlook-share-messages-folders.md)
- [从其他用户身份发送 Outlook 邮件](outlook-send-mail-from-other-user.md)
- [获取 Outlook 资源的不可变标识符](outlook-immutable-id.md)
- 在 Microsoft Graph v1.0 中 [使用邮件 API](/graph/api/resources/mail-api-overview) 及其 [用例](/graph/api/resources/mail-api-overview#common-use-cases)
