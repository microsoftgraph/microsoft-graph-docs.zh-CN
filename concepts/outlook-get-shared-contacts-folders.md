---
title: 获取一个共享文件夹中的 Outlook 联系人
description: " 这也是 "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091792"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>获取一个共享文件夹中的 Outlook 联系人

Outlook 允许客户与另一个共享文件夹，并提供"的读取"、"创建"、"修改"删除"的各个联系人文件夹的访问。 Outlook 还允许委派另一个用户操作代表客户，和访问特定的文件夹或客户的整个邮箱; 客户这也称为是在 Outlook 中的"委派"。

以编程方式，Microsoft Graph 支持具有已由其他用户共享的联系人文件夹中获取联系人，以及获取共享的文件夹本身。 支持也适用于委派邮箱中的文件夹。

例如，Garth 具有共享 John 自定义联系人文件夹，并且授予 John 读取访问权限。 如果 John 已登录到您的应用程序，并提供委派的权限 （Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），您的应用程序都将能够访问 Garth 的自定义联系人文件夹和如下所述的文件夹中的联系人。

## <a name="get-a-contact-in-the-shared-folder"></a>共享文件夹中获取联系人

您可以与 John 共享 Garth 的自定义联系人文件夹中获取特定的联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

在操作成功完成，您将获取 HTTP 200 确定和[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例由标识`{id}`Garth 的共享联系人文件夹中。

## <a name="get-all-contacts-in-the-shared-folder"></a>获取共享文件夹中的所有联系人

获取 Garth 的共享联系人文件夹中的所有联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

在操作成功完成，您将获取 HTTP 200 确定和共享联系人文件夹中 Garth 的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)的实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取与 John 共享 Garth 联系人文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

在操作成功完成，您将获取 HTTP 200 确定，并表示 Garth 的[contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)实例共享联系人文件夹。

如果 Garth 具有委派 John 其整个邮箱，应用相同的 GET 功能。

如果 Garth 不具有与 John、 共享联系人文件夹，也没有有他代理其邮箱到 John，这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么集成 Outlook 个人联系人](outlook-contacts-concept-overview.md)
- Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact?view=graph-rest-1.0) 。