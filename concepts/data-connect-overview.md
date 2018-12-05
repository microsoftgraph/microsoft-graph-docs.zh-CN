---
title: Microsoft Graph 数据连接 （预览）
description: 'Microsoft Graph 数据连接到您将 Office 365 数据和 Microsoft Azure 资源通过核心数据管道。 您可以使用数据连接来构建智能应用程序的访问由 Microsoft，所有 Microsoft 安全群中有价值的数据使用的最佳的开发工具提供的 Microsoft Graph。 所有企业都感兴趣提高工作效率，这意味着构建提高知识工作者工作效率的产品提供了巨大的机会。 '
ms.openlocfilehash: ebd64bf994564decadd44f29c73c0117a99ce176
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091917"
---
# <a name="microsoft-graph-data-connect-preview"></a>Microsoft Graph 数据连接 （预览）

Microsoft Graph 数据连接到您将 Office 365 数据和 Microsoft Azure 资源通过核心数据管道。 您可以使用数据连接来构建智能应用程序的访问由 Microsoft，所有 Microsoft 安全群中有价值的数据使用的最佳的开发工具提供的 Microsoft Graph。 所有企业都感兴趣提高工作效率，这意味着构建提高知识工作者工作效率的产品提供了巨大的机会。 

您可以利用数据连接，如果您是 Microsoft Graph:

- ISV 构建所有 Office 365 客户的智能应用程序。
- 企业开发人员构建您的组织内部的每个人的智能应用程序访问 Office 365 数据。

## <a name="develop-a-pipeline-with-office-365-data"></a>开发 Office 365 数据管道
您可以使用数据连接创建新类型的应用程序基于 Office 365 数据，同时利用工具在 Microsoft Azure 最佳的 Microsoft Graph。 您可以使用 Azure 数据中心将 Office 365 数据移动到常用的 Azure 数据存储： Azure 数据湖泊 Gen 1 或 2 代 （预览） 或 Azure Blob 存储。 然后，可以处理数据 （例如使用 Azure 数据湖泊分析），或将其移到其他存储，如 Azure SQL 数据库。 然后，您可以使用数据服务应用程序的最终用户方案。

Azure 数据中心管道可以从 Office 365 移动数据之前，数据请求同意发送给客户的 Office 365 管理员指定数据审批者。 仅在数据审批者时开始移动数据。

## <a name="publish-your-app-as-an-azure-managed-application"></a>为 Azure 托管应用程序发布应用程序
开发使用 Microsoft Graph 数据连接的应用程序后，您可以将您的应用程序提供给其他人 （或者在其组织或更广泛地）。 Microsoft Graph 数据连接使用[Azure 托管应用程序](https://docs.microsoft.com/en-us/azure/managed-applications/overview)通过 Microsoft Azure Marketplace 可以向他人公开这些应用程序。 Azure 托管应用程序允许 Isv 和企业开发人员向其客户提供全包式解决方案。 客户部署中其订阅，这些托管应用程序时的供应商 （Isv 和企业开发人员） 管理和支持它们。 应用程序供应商还可以将[策略](https://docs.microsoft.com/en-us/azure/managed-applications/overview#azure-policy)应用于其应用程序，如在 rest、 加密以提供更安全地处理其数据的放心的客户。 应用程序可以发布到[Azure Marketplace](https://docs.microsoft.com/en-us/azure/managed-applications/publish-marketplace-app)或[Azure 服务目录](https://docs.microsoft.com/en-us/azure/managed-applications/publish-service-catalog-app)。

安装应用程序的客户看到服务、 所需的数据、 SKU、 每个应用程序的价格和资源消耗的近似成本的条款。 如果购买者的指定属性，设置资源。 这包括开始提取数据的数据中心管道。 为应用程序说明预计安装，以完成，提供的自述文件如何使用该应用程序，以及如何获得支持。

## <a name="next-steps"></a>后续步骤 
若要开始开发 Microsoft Graph 数据连接应用程序，请参阅[Microsoft Graph 概述数据连接](data-connect-concept-overview.md)。
