---
title: 概述 Microsoft Graph 数据连接 （预览）
description: Microsoft Graph 包含有关工作者和其工作区中，包括有关人员的工作方式以及它们进行通信信息丰富的数据、 协作和管理自己的时间。 Microsoft Graph 数据连接到 Microsoft Azure，使您可以访问最佳开发和承载工具来处理这些数据将此数据。 这使客户能够从创新或行业特定应用程序，它们将保留其 Microsoft Graph 数据的完全控制时提高工作效率，受益。 Microsoft 客户的更多安全控件沿推向。
ms.openlocfilehash: cce6046c9ed9b57171e998b1cb17c4e92fa0fcb5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091834"
---
# <a name="overview-of-microsoft-graph-data-connect-preview"></a>概述 Microsoft Graph 数据连接 （预览）
Microsoft Graph 包含有关工作者和其工作区中，包括有关人员的工作方式以及它们进行通信信息丰富的数据、 协作和管理自己的时间。 Microsoft Graph 数据连接到 Microsoft Azure，使您可以访问最佳开发和承载工具来处理这些数据将此数据。 这使客户能够从创新或行业特定应用程序，它们将保留其 Microsoft Graph 数据的完全控制时提高工作效率，受益。 Microsoft 客户的更多安全控件沿推向。

## <a name="why-use-microsoft-graph-data-connect"></a>为何使用 Microsoft Graph 数据连接？
Office 365 管理员必须仔细考虑中移动并管理重要的其组织的数据量固有挑战。 数据连接的 Microsoft Graph 旨在使管理员可以通过其数据; 新控件您可以使用该数据构建的应用程序创建数据驱动的见解。 

### <a name="enable-granular-consent"></a>启用粒度同意

在 Microsoft Graph 许可模型中，管理员或用户仅可以授予或拒绝访问的实体的特定的预定义设置应用程序的请求。 例如，Mail.Read 请求包含对一组固定支持 Outlook 邮件，包括其所有属性使用的整个[邮件](/graph/api/resources/message?view=graph-rest-1.0)实例的实体的读取权限。 相比之下，Microsoft Graph 数据连接允许更精细的同意，允许应用程序请求到实体中的特定属性的访问或筛选这些属性中的数据。 管理员必须授予明确批准访问 Microsoft Graph 数据之前被授予访问权限。 请求必须指定的访问级别请求和描述数据策略实施，请求，并请求的数据的架构的原因。 因此，应用程序可使用数据所必需的功能，并排除不相关的内容。 例如，应用程序可能使用电子邮件标头，但排除正文内容和附件。 

### <a name="provide-data-governance"></a>提供数据管理
Microsoft 促进丰富的、 连接和之间的通信 Microsoft Graph Azure 相对于状态的客户数据。 时您构建的应用程序通过 Microsoft Graph 数据连接，则可以指定一组详细要遵守的策略。 Office 365 管理员可以然后查看并同意这些策略。 这种做法最小化合规性管理开销。 当给定同意时，Microsoft 监视应用程序的遵守策略。 如果应用程序违反 （或尝试违反） 建立组织的策略，Microsoft 将停止于该应用程序的数据流。 

### <a name="get-access-to-data-at-scale"></a>规模获取对数据的访问
丰富的应用程序通常从多个用户同时在组织中大量数据，需要访问。 与传统的事务处理数据模型，您需要构建一个复杂的基础结构，并使数千个 API 调用协调此数据传递。 Microsoft Graph 数据连接使用 Azure 数据中心的强大功能将您的组织中的 Office 365 数据传递到应用程序，可重复计划，只需少量的简单步骤。

## <a name="api-reference"></a>API 参考
正在寻找此服务的 API 参考？

[设置](data-connect-get-started.md)Microsoft Graph 数据连接，并查看[使用 Azure 分析和 Office 365 数据来构建智能应用程序](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)。


## <a name="next-steps"></a>后续步骤
若要开始，请参阅[入门 Microsoft Graph 数据连接](data-connect-get-started.md)。
