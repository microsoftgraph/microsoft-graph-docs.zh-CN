---
title: Outlook 个人联系人 API 概述
description: 使用 Microsoft Graph 中的 Outlook 个人联系人 API 管理电子邮件、安排会议、查找用户信息、共享文件和组协作。
author: angelgolfer-ms
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9054e2741821778571bd5358c0856ee5677d07fc
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556092"
---
# <a name="outlook-personal-contacts-api-overview"></a>Outlook 个人联系人 API 概述

Outlook 联系人可让你存储个人联系人的数据，并且属于Microsoft 365 中 Outlook 邮件中心的一部分。 通过 Outlook，可以管理电子邮件、安排会议、在组织中查找有关用户的信息、启动在线对话、共享文件，以及实现小组协作。

## <a name="why-integrate-with-outlook-personal-contacts"></a>为何要与 Outlook 个人联系人集成？

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>为亿万客户补充邮件和日历应用场景

亿万消费者和数千万组织客户选择 Outlook 作为他们的电子邮件客户端。 通过让客户在 Outlook 中维护一个方便、集成的联系人数据存储，联系人为邮件和日历提供了一项补充功能。 对于开发者而言，利用[邮件](outlook-mail-concept-overview.md)或[日历](outlook-calendar-concept-overview.md)的丰富功能，就意味着通过用户的联系人数据开发更丰富的应用场景。

### <a name="automate-contact-organization"></a>自动执行联系人组织

通过联系人 API，可以保持客户的组织性，与客户通过 Outlook 自己执行此操作等效：

- 与客户体验类似，可以创建 [contact](/graph/api/resources/contact) 实例并将其分配给 [contactFolder](/graph/api/resources/contactfolder) 对象。
- 通过联系人 API，可以采用一致的方式分配类别联系人及事件、消息、任务和组帖子，从而增强组织和发现。 此外，可以[定义用户的主类别列表](/graph/api/outlookuser-post-mastercategories)，从而开发其他创造性方案。
- 你可以对[联系人](/graph/api/resources/contact)设置一个标志以进行跟进。 （Microsoft Graph 中的标记目前为[预览状态](versioning-and-support.md#beta-version)。）

### <a name="share-contact-information"></a>共享联系人信息

通过联系人 API，使你能够获得已登录用户或将其联系人共享或委派给已登录用户的用户的联系人项目。 例如，如果 Garth 与 John 共享联系人文件夹，或者如果 Garth 向 John 委派了访问权限，则来自 John 的[委派权限](auth/auth-concepts.md#microsoft-graph-permissions)将授予你对 Garth 共享日历和内容的读取访问权限。

### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>利用 Microsoft Graph 中的人员 API 更好地利用所有人员数据

你可以对 Outlook [联系人](/graph/api/resources/contact)使用典型 CRUD 操作来创建和管理联系人。 作为 Microsoft Graph 的一部分，还可以使用[人员 API](people-example.md)，查看用户的 Outlook 联系人，以及社交网络、组织目录和最近通信中的人员，并返回有关所有这些来源中人员的与用户相关度最大的信息。 在人员选取器应用场景中利用这一额外智能。

### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>利用 Microsoft Graph 中的其他共享功能和便利

- **contact** 实体支持与存储在 Exchange Online 或 Azure Active Directory 中的用户照片相同的 [profilePhoto](/graph/api/resources/profilephoto) 实体实现的联系人照片。 这消除了在联系人与用户个人资料照片之间进行转换的开销。
- 你可以通过订阅[更改通知](/graph/api/resources/webhooks)和[跟踪对联系人和联系人文件夹所做的更改](delta-query-overview.md)，使应用本地存储保持同步。
- 可以将联系人实例中的应用存储扩展为[开放扩展](extensibility-overview.md#4-open-extensions)，或者将强类型化的自定义数据添加到联系人架构中作为[架构扩展](extensibility-overview.md#3-schema-extensions)。

## <a name="where-is-the-data"></a>数据在什么位置？

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 Outlook 联系人 API](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的 Outlook 联系人 API](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0)中选择和试用联系人示例查询。 选择左侧列中的“显示更多示例”。 使用菜单启用“个人联系人”。
- 了解如何：
  - [获取 Outlook 资源的不可变标识符](outlook-immutable-id.md)
  - [获取共享联系人](outlook-get-shared-contacts-folders.md)
