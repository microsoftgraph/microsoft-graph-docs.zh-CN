---
title: 部署、测试和扩展迁移的应用程序
description: '介绍如何将 Azure Active Directory (Azure AD) 应用迁移为使用 Microsoft Graph API (REST);这讨论了步骤 3: 部署、测试和扩展。'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b5236f6b7be140e1040a3169edded6e162b5e7a
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645252"
---
# <a name="deploy-test-and-extend"></a>部署、测试和扩展

这是[迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的第4步。

1.  **测试 throughly**

    更新应用后, 请对其进行全面测试, 以验证它是否按预期运行, 并且未引入任何回归。  

    请务必使用多个环境、数据集和最终用户角色, 例如具有不同角色、权利和责任的凭据。 通过让新的测试用户首次获取应用程序以及尝试再次使用应用程序的现有用户 (已有权), 完成整个生命周期。

2.  **部署暂存更新**

    请考虑分阶段部署更新。  仅向一小部分友好用户进行有限的滚动, 可帮助确定故障和其他可能 embarrassing 的问题。  这还为您提供了监视初始接收和反馈的机会。

    如果初始滚动很好, 请在部署到更大的访问群体时监视进度。

3.  **浏览新值**

    现在, 您已将切换到 Microsoft Graph, 对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。 定期检查新的数据集和功能。  

    - 请参阅[使用 Microsoft Graph 可以执行的操作](/graph/examples)
    - 浏览[Microsoft graph 博客](/graph/blogs), 了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。
    - [更改日志](/greaph/changelog)汇总了服务和文档更新。 按照这些更新, 将帮助您跟踪引入到/beta (预览) 的新 Api 以及升级为 v1.0 (GA) 的新 Api。  这些新 Api 可为你提供新的方法, 以向你的应用添加更多价值和新体验。  

## <a name="see-also"></a>另请参阅

如果在迁移过程中遇到问题或需要帮助, 可以执行以下操作:

- 再次查看[检查表](migrate-azure-ad-graph-overview.md)
- 将问题发布到[StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)
- 查看 Microsoft Graph 示例以对比现有应用程序代码并与之进行比较:
  - **使用 REST API 的应用程序**: 浏览[快速入门和示例](https://developer.microsoft.com/graph/get-started), 选择您的选择平台, 并在快速启动或搜索相应的示例中运行
  - **使用 .net 客户端库的应用程序**: 查看[控制台-csharp-示例](https://github.com/microsoftgraph/console-csharp-snippets-sample)和/或[dotnetcore-示例](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>后续步骤

- 使用[快速入门和示例](/graph/get-started)快速提高速度。
- 利用[客户端库和 sdk](https://developer.microsoft.com/graph/get-started)开发自定义应用程序 
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
