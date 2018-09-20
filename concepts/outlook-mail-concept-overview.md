# <a name="outlook-mail-api-overview"></a>Outlook 邮件 API 概述

Outlook 是 Office 365 的消息传递通信中心。 它还允许你管理联系人、安排会议、在组织中查找有关用户的信息、启动在线对话、共享文件，以及实现小组协作。

## <a name="why-integrate-with-outlook-mail"></a>为什么与 Outlook 邮件集成？

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>与丰富的功能集成进而服务于数以亿计的客户

与 Outlook 集成意味着可利用客户所喜爱的丰富体验，即在包括移动、Web 和桌面在内的所有设备上提供的针对邮件、[联系人](outlook-contacts-concept-overview.md)、[日历](outlook-calendar-concept-overview.md)的一致、直观体验。

使用 [Microsoft Graph](overview.md)，你只需编写一个应用与 Outlook 进行集成，即可服务于数以亿计的消费者，以及选择 Outlook 作为其电子邮件客户端的数以千万的组织客户。 你可以编写专注于邮件方案的应用，或连接到大量其他 Outlook 和非 Outlook 关系、资源和智能，并实现 Microsoft 云支持的方案。

### <a name="automate-message-organization-and-processing"></a>自动化邮件组织和处理

客户希望 Outlook 帮助他们保持井然有序。 Microsoft Graph 为应用开发人员提供了这些功能，让他们能够构建可优化发现及提高效率和生产率的客户工作流： 

- 客户会以不同的方式组织他们的邮件，一些客户会将所有邮件都放在收件箱中，只需搜索即可，而有些客户会在文件夹中归档邮件。 他们喜欢 Outlook 这种可支持扁平式组织和基于文件夹组织的灵活又直观的方法。 应用可以方便地对特定文件夹或用户整个邮箱中的邮件进行[筛选、搜索或排序](query_parameters.md)。

- Outlook 类别按名称和颜色进行区分。 客户可使用类别标记邮件，以增强组织和发现。 应用可以访问和[定义用户的主类别列表](../api-reference/v1.0/api/outlookuser_post_mastercategories.md)。 此外，该列表可在 Outlook 邮件，以及事件、联系人、任务和组文章中进行共享，为应用开发者开启了创造性的应用场景。 例如，在线培训提供商可以为电子邮件、课程事件设置颜色代码，并跟进用户已注册的各课程的后续作业。

- 此外，应用用户还可更改邮件（或事件或任务）的重要性，或标记邮件以供后续跟进。 （Microsoft Graph 中的标记目前为[预览状态](versioning_and_support.md#beta-version)。）

- 规则 API 将邮件组织提升到了一个新的水平。 应用可以设置[收件箱规则](../api-reference/v1.0/resources/messagerule.md)，以尽快处理传入的邮件并减少电子邮件混乱。 例如，如果邮件主题行包含某些关键字，则应用可以自动将邮件移动到另一个文件夹，并分配类别和重要性，使其易于后续跟进。

### <a name="write-smarter-apps-that-leverage-intelligence"></a>编写利用智能的更智能应用 

使用 Microsoft Graph 向应用用户建议上下文数据：

- 与[重点收件箱](../api-reference/v1.0/resources/manage_focused_inbox.md)和 [@-提及（预览）](../api-reference/beta/api/message_get.md#request-2)集成，让应用用户能够首先阅读和答复与自己相关的邮件。 

- 撰写邮件期间检查[邮件提示](../api-reference/v1.0/resources/mailtips.md)，以获取有关收件人的有用状态信息（如发送自动答复或拥有完整邮箱的收件人）。 邮件提示可以提醒某些条件的应用，以便采取更有效的跟进操作。 

- 使用[人员 API](people_example.md) 提供交互式控件，如应用中的人员选取器。 人员 API 可根据用户通信和协作模式及业务关系建议与用户相关度最高的人员。 

- 为应用用户提供智能文件选取器并建议他们最近与之交互的文件，以便在撰写邮件时以附件形式添加。 [见解（预览）](../api-reference/beta/resources/insights.md)使用高级分析来推荐用户有可能使用的文件、用户最近已查看或已编辑的文件或者与用户共享的文件。


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>在资源或资源实例中存储应用数据

大部分情况下，应用必须将其数据存储在外部数据存储中，并在管理和访问数据时需要开销。 Microsoft Graph 让您在创建或发送新邮件或者答复邮件时将应用程序数据作为 Internet 邮件标头添加。[](../api-reference/v1.0/api/user_post_messages.md#request-2)[](../api-reference/v1.0/api/user_sendmail.md#request-2) 

如果您需要添加并随后更新自定义数据，则可以[在各个资源实例中存储数据](extensibility_overview.md#open-extensions)。 如果适用，可以扩展架构，添加自定义属性，并将类型化的数据存储在 Microsoft Graph 资源中。 你可以使[架构扩展](extensibility_overview.md#schema-extensions)可查找和可共享。 


## <a name="next-steps"></a>后续步骤

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0)中选择和试用 Outlook 邮件示例查询。 选择左侧列中的“显示更多示例”****。 使用菜单打开“Outlook 邮件”****。
- 了解以下信息：

  - [创建和发送邮件](outlook-create-send-messages.md)
  - [组织邮件](outlook-organize-messages.md)的方法
  - 如何[获取共享的邮件](outlook-share-messages-folders.md)

- 查找更多有关[使用邮件 API](../api-reference/v1.0/resources/mail_api_overview.md) 及其在 Microsoft Graph v1.0 中的[用例](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)信息。


