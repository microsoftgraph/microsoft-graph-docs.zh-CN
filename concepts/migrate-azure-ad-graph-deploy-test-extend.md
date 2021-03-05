---
title: 部署、测试和扩展迁移的应用
description: 介绍如何将 Azure Active Directory (Azure AD) 应用迁移到使用 Microsoft Graph API (REST) ;这将讨论步骤 3：部署、测试和扩展。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 55bca2b1d8499ef7ad788555f55f5f92033d1818
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470611"
---
# <a name="deploy-test-and-extend"></a>部署、测试和扩展

这是迁移应用 [的过程的第](migrate-azure-ad-graph-planning-checklist.md)4 步。

1.  **通过测试**

    更新应用后，请全面测试它，以验证它是否正常工作，以及你尚未引入任何回归。  

    请确保使用多个环境、数据集和最终用户角色，例如具有不同的角色、权限和职责的凭据。 通过让新的测试用户首次获取应用，以及已同意再次使用应用的现有用户 (，) 整个生命周期。

2.  **部署阶段更新**

    请考虑分步部署更新。  向一小组友好用户进行有限推出可帮助识别故障和其他潜在的麻烦问题。  这还让你有机会监视初始接收和反馈。

    如果初始推出成功，在部署到更大受众时监视进度。

3.  **探索新值**

    现在，你已切换到 Microsoft Graph，解锁现在触手可及的更多数据集和功能从未如此简单。 
    Microsoft Graph 支持 Azure AD Graph 中不可用的许多新的 Azure AD 数据集和功能，包括： 

    - [Microsoft 365 组管理](./office365-groups-concept-overview.md)
    - [外部用户邀请](/graph/api/resources/invitation?view=graph-rest-1.0)
    - 删除用户 [和 Microsoft 365](/graph/api/resources/directory?view=graph-rest-1.0) 组后还原它们的能力
    - [有关用户和组的 Webhook 通知](./webhooks.md?toc=.%252fref%252ftoc.json&view=graph-rest-1.0)
    - 标识治理功能，例如：
      - [特权标识管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) 仅在需要时和在有限时段内将用户提升为特权角色
      - [有关用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 访问权限证明的一次性或定期访问评审的访问评审
      - [使组织能够](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 显示法律或合规性要求的信息的使用条款，如免责声明通知
    - 安全功能，例如：
      - [身份风险事件](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [风险用户](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - [更多平台和语言](./index.yml) 中提供了客户端库和示例。 Microsoft Graph SDK 提供了一个可发现接口，在以透明方式处理令牌获取、由于错误和限制而重试处理、安全重定向处理以及模型序列化和反序列化时，可轻松访问你的数据。

    Microsoft Graph 提供对更多服务的访问权限，而不只是 Azure Active Directory。 这也是 Microsoft [365 服务的 API 网关](./index.yml)。
    定期检查新的数据集和功能。  

    - 查看可以使用 [Microsoft Graph 执行哪些功能](/graph/examples)
    - 浏览 [Microsoft Graph 博客](/graph/blogs) ，了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。
    - 更改 [日志汇总](/greaph/changelog) 了服务和文档更新。 遵循这些更新将帮助您跟踪 /beta (预览版中引入的新 API) 以及已提升为 (GA) 。  这些新 API 可以为你提供向应用添加更多价值和新体验的新的方法。  

## <a name="see-also"></a>另请参阅

如果在迁移过程中遇到问题或需要帮助，可以：

- 再次 [查看检查](migrate-azure-ad-graph-planning-checklist.md) 表
- 向 [Microsoft 问答&问题](https://docs.microsoft.com/answers/topics/microsoft-graph-applications.html) 
- 查看 Microsoft Graph 示例以对比和比较现有应用程序代码：
  - **使用 REST API** 的应用：浏览 [快速入门](https://developer.microsoft.com/graph/get-started)和示例、选择选择的平台并运行快速入门或搜索相应示例
  - **使用 .NET 客户端库的应用**：查看 [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) 和/或 [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>后续步骤

- 使用 [快速入门和示例](/graph/get-started) 快速入门。
- 利用 [客户端库和 SDK](https://developer.microsoft.com/graph/get-started) 开发自定义应用程序 
- 探索 [Microsoft Graph](./overview.md) 的概念和做法。
- 使用 [Graph 资源管理器](https://aka.ms/ge) 试验 Microsoft Graph。