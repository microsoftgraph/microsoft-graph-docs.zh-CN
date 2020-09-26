---
title: 部署、测试和扩展迁移的应用程序
description: 介绍如何将 Azure Active Directory (Azure AD) 应用程序迁移到使用 Microsoft Graph API (REST) ;这讨论了步骤3：部署、测试和扩展。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 82bc6943f152e287cdb1807de9f15e80b0f91229
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288404"
---
# <a name="deploy-test-and-extend"></a>部署、测试和扩展

这是 [迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的第4步。

1.  **测试 throughly**

    更新应用后，请对其进行全面测试，以验证它是否按预期运行，并且未引入任何回归。  

    请务必使用多个环境、数据集和最终用户角色，例如具有不同角色、权利和责任的凭据。 在整个生命周期中，让新的测试用户首次获取应用程序，以及现有用户 (已) 尝试再次使用应用程序的现有用户。

2.  **部署暂存更新**

    请考虑分阶段部署更新。  仅向一小部分友好用户进行有限的滚动，可帮助确定故障和其他可能 embarrassing 的问题。  这还为您提供了监视初始接收和反馈的机会。

    如果初始滚动很好，请在部署到更大的访问群体时监视进度。

3.  **浏览新值**

    现在，您已将切换到 Microsoft Graph，对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。 
    Microsoft Graph 支持 Azure AD Graph 中不可用的许多新的 Azure AD 数据集和功能，包括： 

    - [Microsoft 365 组管理](./office365-groups-concept-overview.md)
    - [外部用户邀请](/graph/api/resources/invitation?view=graph-rest-1.0)
    - 能够在删除 [用户和 Microsoft 365 组](/graph/api/resources/directory?view=graph-rest-1.0) 之后对其进行还原
    - [用户和组上的 Webhook 通知](./webhooks.md?toc=.%252fref%252ftoc.json&view=graph-rest-1.0)
    - 身份管理功能，如：
      - [特权身份管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) 仅在需要时和在有限的时间段内将用户提升到特权角色
      - [对用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta) 访问权限证明的一次性或定期访问审核
      - 帮助组织提供有关法律或合规性要求的信息（如免责声明通知）[的使用条款](/graph/api/resources/accessreviews-root?view=graph-rest-beta)
    - 安全功能，如：
      - [身份风险事件](/graph/api/resources/identityriskevent?view=graph-rest-1.0)
      - [风险用户](/graph/api/resources/riskyuser?view=graph-rest-1.0)
    - 可在更多平台和语言中使用的[客户端库和示例](./index.yml)。 Microsoft Graph Sdk 提供了一个可发现接口，可在透明地处理令牌获取、重试处理（由于错误和限制、安全重定向处理以及模型序列化和反序列化）而轻松访问数据。

    与 Azure Active Directory 相比，Microsoft Graph 提供了更多的服务访问权限。 这也是 [Microsoft 365 服务的 API 网关](./index.yml)。
    定期检查新的数据集和功能。  

    - 请参阅 [使用 Microsoft Graph 可以执行的操作](/graph/examples)
    - 浏览 [Microsoft graph 博客](/graph/blogs) ，了解有关 Microsoft Graph 的最新新闻和一些出色的学习系列。
    - [更改日志](/greaph/changelog)汇总了服务和文档更新。 按照这些更新，将帮助您跟踪引入到/beta (preview) 的新 Api，以及升级到 (GA) 的新 Api。  这些新 Api 可为你提供新的方法，以向你的应用添加更多价值和新体验。  

## <a name="see-also"></a>另请参阅

如果在迁移过程中遇到问题或需要帮助，可以执行以下操作：

- 再次查看[检查表](migrate-azure-ad-graph-planning-checklist.md)
- 将问题发布到 [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)
- 查看 Microsoft Graph 示例以对比现有应用程序代码并与之进行比较：
  - **使用 REST API 的应用程序**：浏览 [快速入门和示例](https://developer.microsoft.com/graph/get-started)，选择您的选择平台，并在快速启动或搜索相应的示例中运行
  - **使用 .net 客户端库的应用程序**：查看 [控制台-csharp-示例](https://github.com/microsoftgraph/console-csharp-snippets-sample) 和/或 [dotnetcore-示例](https://github.com/microsoftgraph/dotnetcore-console-sample)

## <a name="next-steps"></a>后续步骤

- 使用 [快速入门和示例](/graph/get-started) 快速提高速度。
- 利用 [客户端库和 sdk](https://developer.microsoft.com/graph/get-started) 开发自定义应用程序 
- 浏览 [Microsoft Graph](./overview.md) 概念和实践。
- 使用 [Graph 浏览器](https://aka.ms/ge) 试用 Microsoft Graph。