---
title: Microsoft Graph 数据连接（预览）
description: 'Microsoft Graph 数据连接可通过核心数据管道为你提供 Office 365 数据和 Microsoft Azure 资源。 你可以使用 Microsoft Graph 数据连接来构建智能应用程序，以使用 Microsoft 提供的最佳开发工具访问 Microsoft 安全云中的所有有价值数据。 所有企业都对提高工作效率充满兴趣，这意味着构建能够提高知识型员工作效率的产品会带来巨大的机遇。 '
ms.openlocfilehash: ebd64bf994564decadd44f29c73c0117a99ce176
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091917"
---
# <a name="microsoft-graph-data-connect-preview"></a>Microsoft Graph 数据连接（预览）

Microsoft Graph 数据连接可通过核心数据管道为你提供 Office 365 数据和 Microsoft Azure 资源。 你可以使用 Microsoft Graph 数据连接来构建智能应用程序，以使用 Microsoft 提供的最佳开发工具访问 Microsoft 安全云中的所有有价值数据。 所有企业都对提高工作效率充满兴趣，这意味着构建能够提高知识型员工作效率的产品会带来巨大的机遇。 

要想利用 Microsoft Graph 数据连接，你需要是：

- 一个为所有 Office 365 客户构建智能应用程序的 ISV。
- 一名为组织内部的每个人构建智能应用程序以访问 Office 365 数据的企业开发人员。

## <a name="develop-a-pipeline-with-office-365-data"></a>使用 Office 365 数据开发管道
你可以使用 Microsoft Graph 数据连接，基于 Office 365 数据，同时利用 Microsoft Azure 中的最佳工具来创建新型应用程序。 你可以使用 Azure 数据工厂将 Office 365 数据移动到热门 Azure 数据存储中：Azure Data Lake Gen 1 或 Gen 2（预览版）或 Azure Blob 存储。 然后，可以对数据进行处理（例如，使用 Azure Data Lake Analytics）或将其移动到其他存储中，例如 Azure SQL 数据库。 由此，你便可以使用该数据为应用程序的最终用户应用场景提供服务。

在 Azure 数据工厂管道从 Office 365 移动数据前，系统会向客户的 Office 365 管理员指定的数据批准者发送数据请求许可。 只有在获得数据批准者的批准后才会开始移动数据。

## <a name="publish-your-app-as-an-azure-managed-application"></a>将你的应用发布为 Azure 托管应用程序
使用 Microsoft Graph 数据连接完成应用程序的开发后，你可以将该应用程序提供给其他人（可以是组织中的成员，也可以是更广泛层面的人员）。 Microsoft Graph 数据连接使用 [Azure 托管应用程序](https://docs.microsoft.com/zh-CN/azure/managed-applications/overview)将这些应用程序通过 Microsoft Azure 市场提供给其他人。 Azure 托管应用程序允许 ISV 和企业开发人员为他们的客户提供现成解决方案。 客户可在他们的订阅中部署这些托管应用程序，而供应商（ISV 和企业开发人员）则可对其进行管理和提供支持。 应用程序供应商也可以向其应用程序应用[策略](https://docs.microsoft.com/zh-CN/azure/managed-applications/overview#azure-policy)，例如静态加密，从而让他们的客户因其数据处理方式更加安全而安心无忧。 可以将应用程序发布到 [Azure 市场](https://docs.microsoft.com/zh-CN/azure/managed-applications/publish-marketplace-app)或 [Azure 服务目录](https://docs.microsoft.com/zh-CN/azure/managed-applications/publish-service-catalog-app)。

安装该应用程序的客户将会看到服务条款、所需数据、每个应用程序 SKU 的价格以及资源消耗的大致成本。 当购买者指定了这些属性时，系统将对资源进行设置。 这包括开始提取数据的数据工厂管道。 为应用程序提供一个自述文件，以说明何时可以完成安装，如何使用该应用程序以及如何获得支持。

## <a name="next-steps"></a>后续步骤 
若要开始开发 Microsoft Graph 数据连接应用程序，请参阅 [Microsoft Graph 数据连接概述](data-connect-concept-overview.md)。
