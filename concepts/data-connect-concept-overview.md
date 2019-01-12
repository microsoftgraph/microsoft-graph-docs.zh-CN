---
title: Microsoft Graph 数据连接（预览）概述
description: Microsoft Graph 包含有关工作人员及其工作区的丰富数据，包括有关人员如何工作以及他们如何沟通、协作和管理时间的信息。 Microsoft Graph 数据连接将此数据提供给 Microsoft Azure，从而使用户可以访问使用此数据的最佳开发和托管工具。 这使客户能够受益于创新或行业特定的应用程序，这些应用程序可以提高他们的工作效率，同时他们又可以完全掌控其 Microsoft Graph 数据。 Microsoft 不断引入客户期望的更加安全的控件。
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 8d12b35dfaa8b5a787d373c55ffbaafe2f69ac1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969077"
---
# <a name="overview-of-microsoft-graph-data-connect-preview"></a>Microsoft Graph 数据连接（预览）概述
Microsoft Graph 包含有关工作人员及其工作区的丰富数据，包括有关人员如何工作以及他们如何沟通、协作和管理时间的信息。 Microsoft Graph 数据连接将此数据提供给 Microsoft Azure，从而使用户可以访问使用此数据的最佳开发和托管工具。 这使客户能够受益于创新或行业特定的应用程序，这些应用程序可以提高他们的工作效率，同时他们又可以完全掌控其 Microsoft Graph 数据。 Microsoft 不断引入客户期望的更加安全的控件。

## <a name="why-use-microsoft-graph-data-connect"></a>为什么使用 Microsoft Graph 数据连接？
Office 365 管理员必须仔细考虑移动和管理大量组织数据所固有的挑战。 Microsoft Graph 数据连接旨在为管理员提供对其数据的新控制；可以使用该数据生成创建数据驱动见解的应用。 

### <a name="enable-granular-consent"></a>启用具体同意

在 Microsoft Graph 同意模型中，管理员或用户只能授予或拒绝应用程序访问特定的预定义实体集的请求。 例如，对 Mail.Read 的请求包含对支持 Outlook 邮件的固定实体集的读取访问权限，其中包括具有其所有属性的整个 [message](/graph/api/resources/message?view=graph-rest-1.0) 实例。 相比之下，Microsoft Graph 数据连接允许更具体的同意，允许应用程序请求访问实体中的特定属性，或筛选这些属性中的数据。 在授予访问权限之前，管理员必须明确批准访问 Microsoft Graph 数据。 请求必须指定所请求的访问权限的级别，并说明数据策略实施、请求的原因以及所请求数据的架构。 因此，应用程序只能使用对其功能运行至关重要的数据，并排除不相关的内容。 例如，应用可能会使用电子邮件标题，但排除正文内容和附件。 

### <a name="provide-data-governance"></a>提供数据治理
Microsoft 正在促使 Microsoft Graph 和 Azure 之间就客户数据状态进行丰富的连接通信。 通过 Microsoft Graph 数据连接生成应用时，可以指定一组要遵循的详细策略。 然后，Office 365 管理员可以查看并同意这些策略。 这种做法可最大限度地减少符合性管理开销。 获得同意后，Microsoft 会监视应用程序是否遵守策略。 如果应用程序违反（或试图违反）组织建立的策略，Microsoft 将停止向该应用程序传输数据。 

### <a name="get-access-to-data-at-scale"></a>大规模访问数据
丰富的应用程序需要访问大量数据，通常来自于组织中许多用户同时进行访问。 使用传统的事务性数据模型，你需要生成复杂的基础结构并进行数千次 API 调用以协调此数据交付。 Microsoft Graph 数据连接使用 Azure 数据工厂的强大功能，通过几个简单的步骤，以可重复的日程安排将组织中的 Office 365 数据传递给应用程序。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

[设置](data-connect-get-started.md) Microsoft Graph 数据连接，并参阅[使用 Azure 分析和 Office 365 数据生成智能应用程序](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)。


## <a name="next-steps"></a>后续步骤
要开始使用，请参阅 [Microsoft Graph 数据连接入门](data-connect-get-started.md)。
