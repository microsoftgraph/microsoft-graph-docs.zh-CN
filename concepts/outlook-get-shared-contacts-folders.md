---
title: 获取共享文件夹中的 Outlook 联系人
description: 在 Outlook 中，客户可以共享联系人文件夹并提供对文件夹的访问权限。 Outlook 还允许客户委托其他用户代表客户行事。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: outlook
ms.openlocfilehash: 7be7fb4ddf0d91b74c936b01df4e6bfbdd02ee44
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444353"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>获取共享文件夹中的 Outlook 联系人

使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的读取、创建、修改或删除访问权限。 Outlook 还允许客户委托其他用户代表客户采取行动，并访问特定文件夹或客户的整个邮箱;这也称为 Outlook 中的 *委派* 。

Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。 此支持还适用于已委托的邮箱中的文件夹。

例如，Garth 已与 John 共享自定义联系人文件夹并向 John 授予读取权限。 如果 John 已登录到你的应用，并 (Contacts.Read.Shared 或 Contacts.ReadWrite.Shared) 提供了委派权限，则你的应用能够访问 Garth 的自定义联系人文件夹和该文件夹中的联系人。 有关详细信息，请参阅以下部分。

> [!NOTE]
> Contacts.Read.Shared 或 Contacts.ReadWrite.Shared () 共享权限允许你在共享或委派的文件夹中读取或写入联系人。 它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。 若要对租户中共享、委托或任何其他用户的联系人文件夹中的联系人设置更改通知订阅，请使用应用程序权限 Contacts.Read。

## <a name="get-a-contact-in-the-shared-folder"></a>获取共享文件夹中的联系人

可在 Garth 已与 John 共享的自定义联系人文件夹中获取特定联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 共享联系人文件夹的 `{id}` 标识的[联系人](/graph/api/resources/contact)实例。

## <a name="get-all-contacts-in-the-shared-folder"></a>获取共享文件夹中的所有联系人

获取 Garth 共享联系人文件夹中的所有联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

成功完成后，你将收到“HTTP 200 正常”消息和 Garth 共享联系人文件夹中的[联系人](/graph/api/resources/contact)实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取 Garth 已与 John 共享的联系人文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 共享联系人文件夹的 [contactFolder](/graph/api/resources/contactfolder) 实例。

如果 Garth 已向 John 委托其整个邮箱，则将适用相同的 GET 功能。

如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为何要与 Outlook 个人联系人集成](outlook-contacts-concept-overview.md)
- Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact)。
