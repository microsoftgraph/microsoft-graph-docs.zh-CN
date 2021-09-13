---
title: 部署、测试和扩展迁移的应用
description: 介绍如何将 Azure Active Directory (Azure AD) Graph 应用迁移到使用 Microsoft Graph API (REST) ;这将讨论步骤 3：部署、测试和扩展。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ec5b9b80ed42e1701619cca9153d7562b663d08f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135975"
---
# <a name="deploy-test-and-extend"></a>部署、测试和扩展

这是迁移应用 [的过程的第](migrate-azure-ad-graph-planning-checklist.md)4 步。

1.  **通过测试**

    更新应用后，请全面测试它，以验证它是否正常工作，以及是否未引入任何回归。  

    请确保使用多个环境、数据集和最终用户角色，例如具有不同的角色、权限和职责的凭据。 通过让新的测试用户首次获取应用，以及已经同意再次使用应用的现有用户 (，) 整个生命周期。

2.  **部署分步更新**

    请考虑分步部署更新。  向一小组友好用户进行有限推出可帮助识别故障和其他潜在问题。  这还让你有机会监视初始接收和反馈。

    如果初始推出成功，在部署到更大受众时监视进度。

3.  **探索新值**

    现在，你已切换到 Microsoft Graph，那么解锁现在触手可及的更多数据集和功能从未如此简单。 
    Microsoft Graph 支持许多Azure Active Directory (Azure AD) Azure AD Azure Active Directory (中不可用的数据集和功能) Graph。

    Microsoft Graph提供对更多服务的访问权限，而不只是 Azure Active Directory。 它也是[提供服务Microsoft 365 API 网关](./index.yml)。
    定期检查新的数据集和功能。  

    - 请参阅 Microsoft Graph 中[的主要服务和Graph。](overview-major-services.md)
    - 查看一些 [合作伙伴解决方案](https://developer.microsoft.com/graph/partners)。
    - 浏览[Microsoft Graph](https://developer.microsoft.com/graph/blogs)博客，获取有关 Microsoft Graph和一些出色的学习系列的最新新闻。
    - 更改 [日志总结了](/graph/changelog) 服务和文档更新。 遵循这些更新将有助于你跟踪 /beta (预览版中引入的新 API) 以及已提升为 v1.0 (GA) 。  这些新 API 可以为你提供向应用添加更多价值和新体验的新方式。  

## <a name="see-also"></a>另请参阅

如果在迁移过程中遇到问题或需要帮助，可以：

- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表
- 在问答上向[Microsoft Graph发布&问题](/answers/topics/microsoft-graph-applications.html) 
- 查看 Microsoft Graph示例，以对比和比较现有应用程序代码：
  - **使用 REST API** 的应用：浏览 [快速](https://developer.microsoft.com/graph/get-started)入门和示例，选择你选择的平台，然后运行快速入门或搜索适当的示例
  - **使用 .NET 客户端库的应用**：查看 [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) 或 [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>后续步骤

- 使用 [快速入门和示例](https://developer.microsoft.com/graph/get-started) 来快速入门。
- 利用 [客户端库和 SDK](/graph/sdks/sdks-overview) 开发自定义应用程序 
- 了解[Microsoft Graph](./overview.md)概念和做法。
- 使用[Graph 资源管理器](https://aka.ms/ge)试用 Microsoft Graph。
