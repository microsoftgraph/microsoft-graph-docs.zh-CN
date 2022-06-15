---
title: Microsoft Graph Data Connect 支持的数据集、区域和接收器
description: 了解可用于 Microsoft Graph Data Connect 的支持的数据集、Microsoft 365 区域和接收器存储类型。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: b9138bfe4bbbb664deeea463745a264116035fb1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094027"
---
# <a name="datasets-regions-and-sinks-supported-by-microsoft-graph-data-connect"></a>Microsoft Graph Data Connect 支持的数据集、区域和接收器

Microsoft Graph 数据连接支持 Microsoft Azure 中的各种数据集、数据区域和存储位置。 本文介绍受支持的数据集以及如何访问数据集架构、支持的Microsoft 365和Microsoft Azure区域，以及 Data Connect 通过Azure 数据工厂利用的存储位置。

## <a name="datasets"></a>数据集

Microsoft Graph Data Connect 当前支持以下数据集。若要查看每个数据集的架构，请在Azure 数据工厂中创建一个新的数据集，并使用“架构”选项卡查看它。

| 数据集名称 | 说明 | 示例 | 架构 |
|--------------|-------------|--------|--------|
| BasicDataSet_v0.CalendarView_v0    | 包含日历视图中的事件。                                        | [CalendarView_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.CalendarView_v0.json)      | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/CalendarView_v0.md) |
| BasicDataSet_v0.Contact_v0         | 包含每个用户的通讯簿中的可用信息。                  | [Contact_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v0.json)                | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v0.md) |
| BasicDataSet_v0.Contact_v1         | 包含每个用户的通讯录中的联系信息。                        | [Contact_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v1.json)                | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v1.md) |
| BasicDataSet_v0.DirectReport_v0    | 包含直接向每个用户报告的员工的相关用户信息。   | [DirectReport_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.DirectReport_v0.json)      | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DirectReport_v0.md) |
| BasicDataSet_v0.Event_v0           | 包含用户的日历事件中的信息。                            | [Event_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v0.json)                    | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v0.md) |
| BasicDataSet_v0.Event_v1           | 包含每个用户的日历中的事件。                                       | [Event_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v1.json)                    | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v1.md) |
| BasicDataSet_v0.Inbox_v1      | 包含每个用户的收件箱中的邮件文件夹。                                | [Inbox_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Inbox_v1.json)          | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Inbox_v1.md) |
| BasicDataSet_v0.MailboxSettings_v0 | 包含每个用户的邮箱设置。                                        | [MailboxSetting_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailboxSettings_v0.json) | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailboxSettings_v0.md) |
| BasicDataSet_v0.MailFolder_v0      | 包含每个用户的邮箱中的邮件文件夹。                                | [MailFolder_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailFolder_v0.json)          | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailFolder_v0.md) |
| BasicDataSet_v0.Manager_v0         | 包含每个用户的经理的用户信息。                            | [Manager_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Manager_v0.json)                | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Manager_v0.md) |
| BasicDataSet_v0.Message_v0         | 包含来自用户邮箱的电子邮件消息。                                       | [Message_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v0.json)                | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v0.md) |
| BasicDataSet_v0.Message_v1         | 包含每个用户邮箱中的电子邮件消息。                                       | [Message_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v1.json)                | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v1.md) |
| BasicDataSet_v0.SentItem_v0        | 包含从每个用户的邮箱中发送的邮件。                               | [SentItem_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v0.json)              | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v0.md) |
| BasicDataSet_v0.SentItem_v1        | 包含从每个用户的邮箱中发送的邮件。                                | [SentItem_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v1.json)              | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v1.md) |
| BasicDataSet_v0.TeamChat_v1        | 包含一对一和群组聊天消息的 [Teams 聊天消息](https://support.microsoft.com/office/first-things-to-know-about-chat-in-microsoft-teams-88ed0a06-6b59-43a3-8cf7-40c01f2f92f2)。 此数据集不包括用户显式删除的聊天消息。     | [TeamChat_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.TeamChat_v1.json)              | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/TeamChat_v1.md) |
| BasicDataSet_v0.User_v0            | 包含用户信息（显示名称、用户主体名称以及其他信息）。 | [User_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v0.json)                      | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v0.md) |
| BasicDataSet_v0.User_v1            | 包含用户信息。                                                         | [User_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v1.json)                      | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v1.md) |
| DocumentSharingDataset_v0_Preview            | 包含有关文档权限共享的信息。                                                         | [DocumentSharingDataset_v0_Preview](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/DocumentSharingDataset_v0_Preview.json)                      | [架构](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DocumentSharingDataset_v0_Preview.md) |

## <a name="regions"></a>地区

Microsoft Graph Data Connect 支持从各种Microsoft 365区域提取数据。 若要将数据从Microsoft 365数据中心成功移动到Microsoft Azure存储，Azure 数据工厂实例和 Azure 存储位置必须都映射到受支持的区域，以获取Microsoft 365数据的位置。 

下表指明了支持哪些 Microsoft 365 区域，以及数据移动所需的对应 Azure 区域。

| Office 区域      | Azure 区域                                                   |
| ------------------ | ---------------------------------------------------------------|
| **亚太地区**   | <ul><li>东亚</li><li>东南亚</li></ul>             |
| **澳大利亚**      | <ul><li>澳大利亚东部</li><li>澳大利亚东南部</li></ul>   |
| **欧洲**         | <ul><li>北欧</li><li>西欧</li></ul>             |
| **北美**  | <ul><li>美国中部</li><li>美国东部</li><li>美国东部 2</li><li>美国中北部</li><li>美国中南部</li><li>美国中西部</li><li>美国西部</li><li>美国西部 2</li></ul>                                            |
| **英国** | <ul><li>英国南部</li><li>英国西部</li></ul>                     |

## <a name="sinks"></a>接收器

接收器是Azure 数据工厂用于将数据放置在 Azure 存储中的输出位置。 数据连接支持以下接收器存储类型：

- [Azure Data Lake Storage Gen1](/azure/data-lake-store/data-lake-store-overview)
- [Azure Data Lake Storage Gen2](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure 存储 Blob](/azure/storage/blobs/storage-blobs-overview)

接收器具有以下特点：

- 输出文件采用 JSON 行格式。 输出格式是固定的，并且不支持修改输出的格式。 但是，可以使用Azure 数据工厂将数据连接管道的结果复制到另一个存储机制（如 Azure SQL 数据库）。
- 对于使用 Microsoft 365 作为来源的复制活动中的所有接收器类型，服务主体身份验证是唯一支持的身份验证机制。
- 使用 Azure 存储 Blob 作为接收器时，你必须确保应用程序对 Azure 存储 Blob 位置具有存储 Blob 数据参与者访问权限。

## <a name="see-also"></a>另请参阅

- [适用于 Microsoft 365 数据的 Azure 数据工厂连接器](/azure/data-factory/connector-office-365)
- [策略和计费](data-connect-policies.md)
