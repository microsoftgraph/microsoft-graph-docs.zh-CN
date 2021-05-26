---
title: Microsoft Graph 数据连接支持的数据集、区域和接收器
description: 介绍可与 Microsoft Graph 数据连接结合使用的受支持数据集和目标存储类型。
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 949f48feec3c0120faf52d992b25cf7438dda577
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629369"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Microsoft Graph 数据连接支持的数据集、区域和接收器

Microsoft Graph 数据连接支持 Microsoft Azure 中的各种数据集、数据区域和存储位置。 本主题介绍支持的数据集和如何访问数据集架构、支持的 Microsoft 365 和 Microsoft Azure 区域，以及数据连接通过 Azure 数据工厂使用的存储位置。

## <a name="datasets"></a>数据集

数据连接现在支持以下数据集。若要查看每个数据集的架构，请在 Azure 数据工厂中创建新数据集，然后使用“架构”选项卡查看。

<!-- Fernando's note: Some samples are pending, but Nik will update by 5/20 in the GitHub repo. -->
| 数据集名称                       | 说明                                                                        | 示例 |
| ---------------------------------- | ---------------------------------------------------------------------------------- | ------ |
| BasicDataSet_v0.CalendarView_v0    | 包含日历视图中的事件。                                        | [CalendarView_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.CalendarView_v0.json) |
| BasicDataSet_v0.Contact_v0         | 包含每个用户的通讯簿中的可用信息。                  | 即将发布！       |
| BasicDataSet_v0.Contact_v1         | 包含每个用户的通讯录中的联系信息。                        | [Contact_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v1.json)       |
| BasicDataSet_v0.DirectReport_v0    | 包含直接向每个用户报告的员工的相关用户信息。   | [DirectReport_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.DirectReport_v0.json)       |
| BasicDataSet_v0.Event_v0           | 包含用户的日历事件中的信息。                            | 即将发布！       |
| BasicDataSet_v0.Event_v1           | 包含每个用户的日历中的事件。                                       | [Event_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v1.json)       |
| BasicDataSet_v0.MailboxSettings_v0 | 包含每个用户的邮箱设置。                                        | [MailboxSetting_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailboxSettings_v0.json)       |
| BasicDataSet_v0.MailFolder_v0      | 包含每个用户的邮箱中的邮件文件夹。                                | [MailFolder_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailFolder_v0.json)       |
| BasicDataSet_v0.Manager_v0         | 包含每个用户的经理的用户信息。                            | [Manager_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Manager_v0.json)       |
| BasicDataSet_v0.Message_v0         | 包含来自用户邮箱的邮件。                                       | 即将发布！       |
| BasicDataSet_v0.Message_v1         | 包含每个用户的邮箱中的邮件。                                       | [Message_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v1.json)       |
| BasicDataSet_v0.SentItem_v0        | 包含从每个用户的邮箱中发送的邮件。                               | 即将发布！       |
| BasicDataSet_v0.SentItem_v1        | 包含从每个用户的邮箱中发送的邮件。                                | [SentItem_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v1.json)       |
| BasicDataSet_v0.User_v0            | 包含用户信息（显示名称、用户主体名称以及其他信息）。 | 即将发布！       |
| BasicDataSet_v0.User_v1            | 包含用户信息。                                                         | [User_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v1.json)       |

## <a name="regions"></a>地区

数据连接支持从各种不同的 Microsoft 365 区域提取数据。 若要成功将数据从 Microsoft 365 数据中心转移到 Microsoft Azure 存储，Azure 数据工厂实例和 Azure 存储位置均必须映射到支持的 Microsoft 365 数据位置区域。 下表指明了支持哪些 Microsoft 365 区域，以及数据移动所需的对应 Azure 区域。

| Office 区域      | Azure 区域                                                                                                                                                               |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **亚太地区**   | <ul><li>东亚</li><li>东南亚</li></ul>                                                                                                                         |
| **澳大利亚**      | <ul><li>澳大利亚东部</li><li>澳大利亚东南部</li></ul>                                                                                                               |
| **欧洲**         | <ul><li>北欧</li><li>西欧</li></ul>                                                                                                                         |
| **北美**  | <ul><li>美国中部</li><li>美国东部</li><li>美国东部 2</li><li>美国中北部</li><li>美国中南部</li><li>美国中西部</li><li>美国西部</li><li>美国西部 2</li></ul> |
| **英国** | <ul><li>英国南部</li><li>英国西部</li></ul>                                                                                                                                 |

## <a name="sinks"></a>接收器

接收器是数据工厂用于在 Azure 存储中放置数据的输出位置。 数据连接支持以下接收器存储类型：

- [Azure Data Lake Storage Gen 1](https://docs.microsoft.com/azure/data-lake-store/data-lake-store-overview)
- [Azure Data Lake Storage Gen 2](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure 存储 Blob](/azure/storage/blobs/storage-blobs-overview)

接收器具有以下特点：

- 输出文件将采用 JSON 行的格式。 输出格式是固定的，并且不支持修改输出的格式。 但是，你可以使用 Azure 数据工厂将数据连接管道的结果复制到另一个存储机制（例如 Azure SQL DB）中。
- 对于使用 Microsoft 365 作为来源的复制活动中的所有接收器类型，服务主体身份验证是唯一支持的身份验证机制。
- 使用 Azure 存储 Blob 作为接收器时，你必须确保应用程序对 Azure 存储 Blob 位置具有存储 Blob 数据参与者访问权限。

## <a name="see-also"></a>另请参阅

- [适用于 Microsoft 365 数据的 Azure 数据工厂连接器](https://docs.microsoft.com/azure/data-factory/connector-office-365)
- [策略和计费](data-connect-policies.md)
