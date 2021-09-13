---
title: 获取共享文件夹中的 Outlook 联系人
description: 使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的读取、创建、修改或删除访问权限。 通过 Outlook，客户还可以委托其他用户代表自己执行操作。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: outlook
ms.openlocfilehash: 3c1673dd6b551d1626187ee120ccc5e08550933b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135926"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>获取共享文件夹中的 Outlook 联系人

使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的“读取”、“创建”、“修改”或“删除”访问权限。 此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。

Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。 此支持还适用于已委托的邮箱中的文件夹。

例如，Garth 已与 John 共享自定义联系人文件夹并向 John 授予读取权限。 如果 John 已登录应用并提供委托的权限（Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），应用便能访问 Garth 的自定义联系人文件夹和该文件夹中的联系人，如下所述。

> **注意** 通过共享权限（Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），你可以在共享或委托文件夹中读取或写入联系人。 它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。 若要对租户中共享、委托或任何其他用户的联系人文件夹中的联系人设置更改通知订阅，请使用应用程序权限 Contacts.Read。

## <a name="get-a-contact-in-the-shared-folder"></a>获取共享文件夹中的联系人

可在 Garth 已与 John 共享的自定义联系人文件夹中获取特定联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 共享联系人文件夹的 `{id}` 标识的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例。

## <a name="get-all-contacts-in-the-shared-folder"></a>获取共享文件夹中的所有联系人

获取 Garth 共享联系人文件夹中的所有联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

成功完成后，你将收到“HTTP 200 正常”消息和 Garth 共享联系人文件夹中的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取 Garth 已与 John 共享的联系人文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 共享联系人文件夹的 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) 实例。

如果 Garth 已向 John 委托其整个邮箱，则将适用相同的 GET 功能。

如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为何要与 Outlook 个人联系人集成](outlook-contacts-concept-overview.md)
- Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact?view=graph-rest-1.0)。
