---
title: 获取共享文件夹或委托文件夹中的 Outlook 邮件
description: 使用 Outlook，客户可以与其他人共享邮件文件夹，并授予对各个文件夹的读取、创建、修改或删除访问权限。 通过 Outlook，客户还可以委托其他用户代表自己执行操作。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 76f54b5cc2db5395b9ca5e50611c4cea4f18b770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557899"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>获取共享文件夹或委托文件夹中的 Outlook 邮件

使用 Outlook，客户可以与其他人共享邮件文件夹，并授予对各个文件夹的“读取”、“创建”、“修改”或“删除”访问权限。 此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定邮件文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。

Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。 此支持还适用于已委托的文件夹。

例如，Garth 已与 John 共享自己的收件箱，并向 John 授予对自己收件箱的读取访问权限。 如果 John 已登录应用并授予委托的权限（Mail.Read.Shared 或 Mail.ReadWrite.Shared），应用便能访问 Garth 的邮件和收件箱，如下所述。

> **注意**通过共享权限（Mail.Read.Shared 或 Mail.ReadWrite.Shared），你可以在共享或委托文件夹中读取或写入邮件。 它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。 若要对租户中共享、委托或任何其他用户的邮件文件夹中的邮件设置更改通知订阅，请使用应用程序权限 Mail.Read。

## <a name="get-a-message-in-the-shared-folder"></a>获取共享文件夹中的邮件

你可以在 Garth 的收件箱中获取特定邮件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 收件箱的 `{id}` 标识的[消息](/graph/api/resources/message?view=graph-rest-1.0)实例。

## <a name="get-all-messages-in-the-shared-folder"></a>获取共享文件夹中的全部邮件

获取 Garth 收件箱中的所有邮件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

成功完成后，你将收到“HTTP 200 正常”消息和 Garth 收件箱中的[消息](/graph/api/resources/message?view=graph-rest-1.0)实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取 Garth 与 John 共享的文件夹（收件箱）。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 收件箱文件夹的 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) 实例。

如果 Garth 已经委派 John 进一步访问他的收件箱，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。

如果 Garth 既未与 John 共享自己的收件箱，也未将自己的邮箱委托给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称便会返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [使用邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。
