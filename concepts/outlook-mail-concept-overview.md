---
title: Outlook 邮件 API 概述
description: Outlook 是 Microsoft 365 的消息传递通信中心。 使用它，还可以管理联系人、安排会议、查找组织用户的相关信息、
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0fcfb1a56e811d7ba63dcd1daed83122132c32bc
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645624"
---
# <a name="outlook-mail-api-overview"></a>Outlook 邮件 API 概述

Outlook 是 Microsoft 365 的消息传递通信中心。有了它，你同样能管理联系人、安排会议、在组织中查找用户相关信息、发起在线对话、共享文件，并实现小组协作。

> [!VIDEO https://www.youtube-nocookie.com/embed/L-gm25wusIQ]

## <a name="why-integrate-with-outlook-mail"></a>为什么与 Outlook 邮件集成？

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>与丰富的功能集成进而服务于数以亿计的客户

与 Outlook 集成意味着可利用客户所喜爱的丰富体验，即在包括移动、Web 和桌面在内的所有设备上提供的针对邮件、[联系人](outlook-contacts-concept-overview.md)、[日历](outlook-calendar-concept-overview.md)的一致、直观体验。

使用 [Microsoft Graph](overview.md)，你只需编写一个应用与 Outlook 进行集成，即可服务于数以亿计的消费者，以及选择 Outlook 作为其电子邮件客户端的数以千万的组织客户。 你可以编写专注于邮件方案的应用，或连接到大量其他 Outlook 和非 Outlook 关系、资源和智能，并实现 Microsoft 云支持的方案。

### <a name="automate-message-organization-and-processing"></a>自动化邮件组织和处理

客户对 Outlook 帮助他们保持井然有序的方式颇为青睐。Microsoft Graph 为应用开发人员提供了这些功能，让他们能够构建可优化发现及提高效率和生产率的客户工作流：

- 客户会以不同的方式组织他们的邮件，一些客户会将所有邮件都放在收件箱中，只需搜索即可，而有些客户会在文件夹中归档邮件。 他们喜欢 Outlook 这种可支持扁平式组织和基于文件夹组织的灵活又直观的方法。 应用可以方便地对特定文件夹或用户整个邮箱中的邮件进行[筛选、搜索或排序](query-parameters.md)。

- Outlook 类别按名称和颜色进行区分。 客户可使用类别标记邮件，以增强组织和发现。 应用可以访问和[定义用户的主类别列表](/graph/api/outlookuser-post-mastercategories)。 此外，该列表可在 Outlook 邮件，以及事件、联系人、任务和组文章中进行共享，为应用开发者开启了创造性的应用场景。 例如，在线培训提供商可以为电子邮件、课程事件设置颜色代码，并跟进用户已注册的各课程的后续作业。

- 此外，应用用户还可更改邮件（或事件或任务）的重要性，或标记邮件以供后续跟进。 （Microsoft Graph 中的标记目前为[预览状态](versioning-and-support.md#beta-version)。）

- 规则 API 将邮件组织提升到了一个新的水平。 应用可以设置[收件箱规则](/graph/api/resources/messagerule)，以尽快处理传入的邮件并减少电子邮件混乱。 例如，如果邮件主题行包含某些关键字，则应用可以自动将邮件移动到另一个文件夹，并分配类别和重要性，使其易于后续跟进。

- 许多客户使用采用 MIME 格式发送和接收邮件的电子邮件客户端。 即使 Outlook 不会以 MIME 格式保存邮件，应用也可以[以 MIME 格式获取 Outlook 邮件正文](outlook-get-mime-message.md)，[以 MIME 格式发送 Outlook 邮件](outlook-send-mime-message.md)，附加 S/MIME 数字签名，并以 S/MIME 加密邮件内容。

### <a name="write-smarter-apps-that-leverage-intelligence"></a>编写利用智能的更智能应用

使用 Microsoft Graph 向应用用户建议上下文数据：

- 与[重点收件箱](/graph/api/resources/manage-focused-inbox)和 [@提及（预览版）](/graph/api/message-get?view=graph-rest-beta&preserve-view=true#example-2-get-all-mentions-in-a-specific-message)集成，让应用用户能够先阅读和答复与自己相关的邮件。

- 一边查看[邮件提示](/graph/api/resources/mailtips)，一边仍能撰写邮件，以获取收件人的实用状态信息（如收件人正在发送自动答复或邮箱已满）。 邮件提示可以提醒应用注意特定条件，以便采取更高效的跟进操作。

- 使用[人员 API](people-example.md) 提供交互式控件，如应用中的人员选取器。 人员 API 可根据用户通信和协作模式及业务关系建议与用户相关度最高的人员。

- 为应用用户提供智能文件选取器并建议他们最近与之交互的文件，以便在撰写邮件时以附件形式添加。 [见解](/graph/api/resources/officegraphinsights)使用高级分析来推荐用户有可能使用的文件、用户最近查看或编辑的文件，或者与用户共享的文件。


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>在资源或资源实例中存储应用数据

大部分情况下，应用需要将数据存储在外部数据存储中，并承担数据管理和访问开销。 借助 Microsoft Graph，可以在[创建](/graph/api/user-post-messages#example-2-create-message-draft-that-includes-custom-message-headers)或[发送](/graph/api/user-sendmail#example-2-create-a-message-with-custom-internet-message-headers-and-send-the-message)新邮件或邮件回复时，直接将应用数据添加为 Internet 邮件头。

如果需要添加并随后更新自定义数据，可以[在各个资源实例中存储数据](extensibility-overview.md#open-extensions)。 也可以在适当情况下扩展架构、添加自定义属性，并在 Microsoft Graph 资源中存储类型化数据。 可以让此类[架构扩展](extensibility-overview.md#schema-extensions)可供发现和共享。

## <a name="where-is-the-data"></a>数据在什么位置？

[!INCLUDE [outlook-mailbox-type-support](../includes/outlook-mailbox-type-support.md)]

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 Outlook 邮件 API](/graph/api/resources/mail-api-overview)
- [Microsoft Graph beta 中的 Outlook 邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-beta&preserve-view=true)


## <a name="next-steps"></a>后续步骤

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0)中选择和试用 Outlook 邮件示例查询。 选择左侧列中的“显示更多示例”。 使用菜单打开“Outlook 邮件”。
- 了解以下信息：

  - [创建和发送邮件](outlook-create-send-messages.md)
  - [邮件整理](outlook-organize-messages.md)方法
  - [获取邮件的 MIME 内容](outlook-get-mime-message.md)
  - [将大文件附加到 Outlook 邮件或事件](outlook-large-attachments.md)
  - [获取共享邮件](outlook-share-messages-folders.md)
  - 如何[从其他用户身份发送邮件](outlook-send-mail-from-other-user.md)
  - [获取 Outlook 资源的不可变标识符](outlook-immutable-id.md)
  - [发送含有 MIME 内容的电子邮件](outlook-send-mime-message.md)

- 详细了解如何使用 Microsoft Graph v1.0 中的[邮件 API](/graph/api/resources/mail-api-overview) 及其[用例](/graph/api/resources/mail-api-overview#common-use-cases)。


