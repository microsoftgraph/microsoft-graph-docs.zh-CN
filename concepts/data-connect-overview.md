---
title: Microsoft Graph 数据连接
description: 'Microsoft Graph 数据连接可通过核心数据管道为你提供 Office 365 数据和 Microsoft Azure 资源。 你可以使用 Microsoft Graph 数据连接来构建智能应用程序，以使用 Microsoft 提供的最佳开发工具访问 Microsoft 安全云中的所有有价值数据。 所有企业都对提高工作效率充满兴趣，这意味着构建能够提高知识型员工作效率的产品会带来巨大的机遇。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: 42a35f9d96b375ea4139ece3e5b15e11d300598c
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969184"
---
# <a name="microsoft-graph-data-connect"></a>Microsoft Graph 数据连接

Microsoft Graph 数据连接通过工具集为你提供 Office 365 数据和 Microsoft Azure 资源。 你可以使用 Microsoft Graph 数据连接来构建智能应用程序，以使用 Microsoft 提供的最佳开发工具访问 Microsoft 安全云中的所有有价值数据。 所有企业都对提高工作效率充满兴趣，这意味着构建能够提高知识型员工作效率的产品会带来巨大的机遇。

> [!VIDEO https://www.youtube-nocookie.com/embed/J1WGFRGnc7g]

如果你同意 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=/graph/context)和 [Microsoft 隐私声明](https://go.microsoft.com/fwlink/p/?LinkId=123161)，并且是下述人员之一，则可利用 Microsoft Graph 数据连接：

- 一个 ISV，它用于为所有 Office 365 客户构建智能应用程序。
- 一名企业开发人员，他为组织内部用户构建可访问 Office 365 数据的智能应用程序。

## <a name="develop-a-pipeline-with-office-365-data"></a>使用 Office 365 数据开发管道
你可以使用 Microsoft Graph 数据连接，基于 Office 365 数据，同时利用 Microsoft Azure 中的最佳工具来创建新型应用程序。 可使用 Azure 数据工厂将 Office 365 数据移动到热门 Azure 数据存储中：Azure Data Lake Gen 1/Gen 2 或 Azure Blob 存储。 然后，可以对数据进行处理（例如，使用 Azure Data Lake Analytics）或将其移动到其他存储中，例如 Azure SQL 数据库。 由此，你便可以使用该数据为应用程序的最终用户应用场景提供服务。

在 Azure 数据工厂管道从 Office 365 移动数据前，系统会向客户的 Office 365 管理员指定的数据批准者发送数据请求许可。 只有在获得数据批准者的批准后才会开始移动数据。

## <a name="publish-your-app-as-an-azure-managed-application"></a>将应用发布为 Azure 托管应用程序
通过 Microsoft Graph 数据连接完成应用程序的开发后，可将该应用程序提供给其他人（可在组织内部提供，也可更广泛地提供）。 Microsoft Graph 数据连接使用 [Azure 托管应用程序](https://docs.microsoft.com/azure/managed-applications/overview)将这些应用程序通过 Microsoft Azure 市场提供给其他人。 Azure 托管应用程序允许 ISV 和企业开发人员为他们的客户提供现成解决方案。 客户可在他们的订阅中部署这些托管应用程序，而供应商（ISV 和企业开发人员）则可对其进行管理和提供支持。 应用程序供应商也可以向其应用程序应用[策略](https://docs.microsoft.com/azure/managed-applications/overview#azure-policy)，例如静态加密，从而让他们的客户因其数据处理方式更加安全而安心无忧。 可以将应用程序发布到 [Azure 市场](https://docs.microsoft.com/azure/managed-applications/publish-marketplace-app)或 [Azure 服务目录](https://docs.microsoft.com/azure/managed-applications/publish-service-catalog-app)。

安装该应用程序的客户可看到服务条款、所需数据、每个应用程序 SKU 的价格以及资源消耗的大致成本。 当购买者指定了所需部署属性时，系统将对资源进行预配。 这包括开始提取数据的数据工厂管道。 为应用程序提供一个自述文件，以说明何时可以完成安装，如何使用该应用程序以及如何获得支持。

## <a name="next-steps"></a>后续步骤
若要开始开发 Microsoft Graph 数据连接应用程序，请参阅 [Microsoft Graph 数据连接概述](data-connect-concept-overview.md)。
