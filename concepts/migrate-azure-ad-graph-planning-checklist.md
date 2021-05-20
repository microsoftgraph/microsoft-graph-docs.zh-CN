---
title: 应用迁移规划清单
description: 将应用从 Azure AD Graph迁移到 Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 84d486cd64d838a00998179a25dbba3ea35738eb
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546929"
---
# <a name="app-migration-planning-checklist"></a>应用迁移规划清单

> [!Important]
> Azure AD Graph API 现已弃用。 我们将继续提供技术支持和安全更新，但不再提供功能更新。
> 从 2022 年 6 月 30 开始，我们将停止对 Azure AD Graph将不再提供技术支持或安全更新。 在此时间Graph使用 Azure AD 应用的应用将不再收到来自 Azure AD Graph响应。

使用以下清单规划迁移。

## <a name="step-1-review-the-differences-between-the-apis"></a>步骤 1：查看 API 之间的差异

许多方面，Microsoft Graph类似于早期的 Azure AD Graph。 在许多情况下，只需在代码中更改终结点服务名称和版本，所有内容都应继续工作。

尽管如此，仍有一些差异。 某些资源、属性、方法和核心功能已更改。

具体而言，请查找以下方面的差异：

- [两个服务](migrate-azure-ad-graph-request-differences.md) 之间的请求调用语法
- [功能](migrate-azure-ad-graph-feature-differences.md)差异，如目录扩展、批处理、差异查询等
- [实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型
- [请求](migrate-azure-ad-graph-property-differences.md) 和响应对象的属性
- [方法](migrate-azure-ad-graph-method-differences.md)，包括参数和类型

## <a name="step-2-examine-api-use"></a>步骤 2：检查 API 使用

[检查你的应用使用的](migrate-azure-ad-graph-audit-api-use.md) API、它们所需的权限，并与已知差异列表进行比较。  

验证你的应用所需的 API 在 Microsoft Graph v1.0 中是否通常可用，以及这些 API 是否以相同方式工作。

在某些情况下，新功能和特性旨在取代早期方法。

使用[Graph 资源管理器](https://aka.ms/ge)试验新调用并开发新方法。 为了获得最佳结果，使用测试租户中的测试用户的凭据登录，以便查看 API 对重要数据集执行哪些操作。

## <a name="step-3-review-app-details"></a>步骤 3：查看应用详细信息

- [应用注册](migrate-azure-ad-graph-app-registration.md) 和同意 (更改，这些更改不应) 。
- 令牌获取 [和身份验证库](migrate-azure-ad-graph-authentication-library.md)。
- 对于 .NET 应用程序，请使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。

## <a name="step-4-deploy-test-and-extend-your-app"></a>步骤 4：部署、测试和扩展应用

在为所有人更新应用之前，请确保全面测试并推广到客户受众。

现在，你已切换到 Microsoft Graph，那么解锁现在触手可及的更多数据集和功能从未如此简单。 通过查看 Microsoft Graph 中的一些主要服务和功能，你可以尝试[一下Graph。](./overview-major-services.md)

[Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 现在是建议用于该身份验证库的Microsoft 标识平台。 如果当前正在使用 ADAL ([ADAL](/azure/active-directory/develop/active-directory-authentication-libraries)) ，请计划切换到 MSAL。 请参阅将应用程序迁移到[MSAL (Microsoft 身份验证库) 。 ](/azure/active-directory/develop/msal-migration)

## <a name="next-steps"></a>后续步骤

- 了解开始 [步骤](migrate-azure-ad-graph-request-differences.md) 1：查看 API 差异的请求调用语法。