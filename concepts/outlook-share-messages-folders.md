---
title: 获取一个共享或委派文件夹中的 Outlook 邮件
description: 这些主题还具有类似部分-列表事件、 获取事件、 获取日历、 联系人列表、 获取联系人和获取联系人文件夹。
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091842"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>获取一个共享或委派文件夹中的 Outlook 邮件

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Outlook 允许客户与另一个共享邮件文件夹，并提供"的读取"、"创建"、"修改"删除"对单个文件夹的访问。 Outlook 还允许委派另一个用户操作代表客户，和访问特定的邮件文件夹或客户的整个邮箱; 客户这也称为是在 Outlook 中的"委派"。

Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。 支持还适用于已委派的文件夹。

例如，Garth 具有共享 John 并且授予对 Garth 的收件箱读取访问权限。 如果 John 已登录到您的应用程序，并提供委派的权限 （Mail.Read.Shared 或 Mail.ReadWrite.Shared），您的应用程序都将能够访问 Garth 的邮件和 Garth 的收件箱，如下所述。

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

如果 Garth 不具有与 John、 共享其收件箱也有他代理其邮箱到 John，这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [使用邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。