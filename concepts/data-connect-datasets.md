---
title: Microsoft Graph 数据连接支持的数据集、区域和接收器
description: 介绍可与 Microsoft Graph 数据连接结合使用的受支持数据集和目标存储类型。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: fd4fbac34f4b03a3802de4834f0c02045d57c4ea
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547623"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Microsoft Graph 数据连接支持的数据集、区域和接收器

Microsoft Graph 数据连接支持 Microsoft Azure 中的各种数据集、数据区域和存储位置。 本主题介绍支持的数据集和如何访问数据集架构、支持的 Microsoft 365 和 Microsoft Azure 区域，以及数据连接通过 Azure 数据工厂使用的存储位置。

如果希望为其他数据集、区域或接收器请求支持，请在 [Microsoft 365 开发人员平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) 上告知我们。

## <a name="datasets"></a>数据集

数据连接现在支持以下数据集。若要查看每个数据集的架构，请在 Azure 数据工厂中创建新数据集，然后使用“架构”选项卡查看。 

|数据集名称|说明|
|-------------|-----------|
|BasicDataSet_v0.Contact_v0|包含每个用户的通讯录中的联系信息。 这些实体的架构类似于 [Microsoft Graph 个人联系人架构](/graph/api/resources/contact)。| 
|BasicDataSet_v0.Event_v0|包含每个用户的日历中的事件。 这些实体的架构类似于 [Microsoft Graph 日历事件架构](/graph/api/resources/event)。| 
|BasicDataSet_v0.Message_v0|包含每个用户的邮箱中的邮件。 这些实体的架构类似于 [Microsoft Graph 邮件架构](/graph/api/resources/message)。| 
|BasicDataSet_v0.SentItem_v0|包含从每个用户的邮箱中发送的邮件。 这些实体的架构类似于 [Microsoft Graph 邮件架构](/graph/api/resources/message)。| 
|BasicDataSet_v0.User_v0|包含用户信息（显示名称、用户主体名称等）。| 
|BasicDataSet_v0.MailboxSettings_v0|包含每个用户的邮箱设置。 这些实体的架构对应于 [Microsoft Graph 邮箱设置架构](/graph/api/resources/mailboxsettings)。| 
|BasicDataSet_v0.MailFolder_v0|包含每个用户的邮箱中的邮件文件夹。 这些实体的架构对应于 [Microsoft Graph 邮件文件夹架构](/graph/api/resources/mailfolder)。|
|BasicDataSet_v0.Manager_v0|包含每个用户的经理的用户信息。 这些实体的架构对应于 [Microsoft Graph 用户架构](/graph/api/resources/user)。|
|BasicDataSet_v0.DirectReport_v0|包含直接向每个用户报告的员工的相关用户信息。 这些实体的架构对应于 [Microsoft Graph 用户架构](/graph/api/resources/user)。|
|BasicDataSet_v0.CalendarView_v0|包含事件。这些实体的架构对应于 [Microsoft Graph 用户架构](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/events)。|
|BasicDataSet_v0.User_v1|此表包含用户信息。 这些实体的架构对应于 [Microsoft Graph 用户架构](/graph/api/resources/user)。|
|BasicDataSet_v0.Contact_v1|包含每个用户的通讯录中的联系信息。 这些实体的架构对应于 [Microsoft Graph 个人联系人架构](/graph/api/resources/contact)。|
|BasicDataSet_v0.Event_v1|包含每个用户的日历中的事件。 这些实体的架构对应于 [Microsoft Graph 日历事件架构](/graph/api/resources/event)。|
|BasicDataSet_v0.Message_v1|包含每个用户的邮箱中的邮件。 这些实体的架构对应于 [Microsoft Graph 邮件架构](/graph/api/resources/message)。|
|BasicDataSet_v0.SentItem_v1|包含从每个用户的邮箱中发送的邮件。 这些实体的架构对应于 [Microsoft Graph 邮件架构](/graph/api/resources/message)。|

## <a name="regions"></a>地区

数据连接支持从各种不同的 Microsoft 365 区域提取数据。 若要成功将数据从 Microsoft 365 数据中心转移到 Microsoft Azure 存储，Azure 数据工厂实例和 Azure 存储位置均必须映射到支持的 Microsoft 365 数据位置区域。 下表指明了支持哪些 Microsoft 365 区域，以及数据移动所需的对应 Azure 区域。 

| Office 区域                    | Azure 区域                                |
|----------------------------------|---------------------------------------------|
| **北美**                | 美国东部<br/>美国东部 2<br/>美国中部<br/>美国中北部<br/>美国中南部<br/>美国中西部<br/>美国西部<br/>美国西部 2|
| **欧洲**                       | 北欧<br/>西欧|
| **亚太地区**                 | 东亚<br/>东南亚|
| **澳大利亚**                    | 澳大利亚东部<br/>澳大利亚东南部|

## <a name="sinks"></a>接收器

接收器是数据工厂用于在 Azure 存储中放置数据的输出位置。 数据连接支持以下接收器存储类型：

- Azure Data Lake Storage Gen 2
- Azure 存储 Blob
- Azure Data Lake Storage Gen 1

接收器具有以下特点： 

- 输出文件将采用 JSON 行的格式。 输出格式是固定的，并且不支持修改输出的格式。 但是，你可以使用 Azure 数据工厂将数据连接管道的结果复制到另一个存储机制（例如 Azure SQL DB）中。
- 对于使用 Microsoft 365 作为来源的复制活动中的所有接收器类型，服务主体身份验证是唯一支持的身份验证机制。
- 使用 Azure 存储 Blob 作为接收器时，你必须确保应用程序对 Azure 存储 Blob 位置具有存储 Blob 数据参与者访问权限。

## <a name="next-steps"></a>后续步骤

有关如何创建数据连接管道作为 Azure 数据工厂的一部分的详细信息，请参阅 [Azure 数据工厂 Office 365 连接器文档](/azure/data-factory/connector-office-365)。