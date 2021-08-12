---
title: 部署、测试和扩展迁移的应用
description: 介绍如何将 Azure Active Directory (Azure AD) 应用迁移到使用 Microsoft Graph API (REST) ;这将讨论步骤 3：部署、测试和扩展。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: c950e8fe97fd6a7e5a269824b1745af08b256c6795bbebb9186f105550233e1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163528"
---
# <a name="deploy-test-and-extend"></a>部署、测试和扩展

这是迁移应用 [的过程的第](migrate-azure-ad-graph-planning-checklist.md)4 步。

1.  **通过测试**

    更新应用后，请全面测试它，以验证它是否正常工作，以及是否未引入任何回归。  

    请确保使用多个环境、数据集和最终用户角色，例如具有不同的角色、权限和职责的凭据。 通过让新的测试用户首次获取应用，以及已同意再次使用应用的现有用户 (，) 整个生命周期。

2.  **部署分步更新**

    请考虑分步部署更新。  向一小组友好用户进行有限推出可帮助识别故障和其他潜在问题。  这还让你有机会监视初始接收和反馈。

    如果初始推出成功，在部署到更大受众时监视进度。

3.  **探索新值**

    现在，你已切换到 Microsoft Graph，那么解锁现在触手可及的更多数据集和功能从未如此简单。 
    Microsoft Graph 支持许多在 Azure AD Graph中不可用的新 Azure AD 数据集和功能，包括： 

    - [Microsoft 365组管理](./office365-groups-concept-overview.md)
    - [外部用户邀请](/graph/api/resources/invitation)
    - 删除[用户和Microsoft 365组](/graph/api/resources/directory)后还原用户和组的能力
    - [有关用户和组的 Webhook 通知](./webhooks.md?toc=.%252fref%252ftoc.json)
    - 标识管理功能，例如：
      - [PRIVILEGEd identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) (PIM) to elevate users to privileged roles only when needed and for a limited time
      - [针对用户](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 访问权限证明的一次性或定期访问评审的访问评审
      - [使组织能够提供有关](/graph/api/resources/agreement) 法律或合规性要求的信息（如免责声明声明）的使用条款
    - 安全功能，例如：
      - [身份风险事件](/graph/api/resources/riskdetection)
      - [风险用户](/graph/api/resources/riskyuser)
    - [更多平台和语言](/graph/sdks/sdks-overview) 中提供了客户端库和示例。 Microsoft Graph SDK 提供了一个可发现接口，可轻松访问你的数据，同时以透明方式处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化。

    Microsoft Graph提供对更多服务的访问权限，而不只是 Azure Active Directory。 这也是提供[服务Microsoft 365 API 网关](./index.yml)。
    定期检查新的数据集和功能。  

    - 查看一些 [合作伙伴解决方案](https://developer.microsoft.com/graph/partners)。
    - 浏览[Microsoft Graph](https://developer.microsoft.com/graph/blogs)博客，获取有关 Microsoft Graph和一些出色的学习系列的最新新闻。
    - 更改 [日志总结了](/graph/changelog) 服务和文档更新。 遵循这些更新将有助于你跟踪 /beta (预览版中引入的新 API) 以及已提升为 v1.0 (GA) 。  这些新 API 可以为你提供向应用添加更多价值和新体验的新方式。  

## <a name="see-also"></a>另请参阅

如果在迁移过程中遇到问题或需要帮助，可以：

- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表
- 向 [Microsoft 问答&问题](/answers/topics/microsoft-graph-applications.html) 
- 查看 Microsoft Graph示例，以对比和比较现有应用程序代码：
  - **使用 REST API** 的应用：浏览 [快速](https://developer.microsoft.com/graph/get-started)入门和示例，选择你选择的平台，然后运行快速入门或搜索相应的示例
  - **使用 .NET 客户端库的应用**：查看 [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) 和/或 [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>后续步骤

- 使用 [快速入门和示例](https://developer.microsoft.com/graph/get-started) 快速入门。
- 利用 [客户端库和 SDK](/graph/sdks/sdks-overview) 开发自定义应用程序 
- 了解[Microsoft Graph](./overview.md)概念和做法。
- 使用[Graph资源管理器](https://aka.ms/ge)尝试 Microsoft Graph。