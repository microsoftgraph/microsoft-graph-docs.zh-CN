---
title: Azure Active Directory (Azure AD) Graph 应用迁移清单
description: 使用此清单将应用从 Azure Active Directory (Azure AD) Graph 迁移到 Microsoft Graph。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: ca3625d7462d1801dc5056f6f65246495aee1e56
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577698"
---
# <a name="azure-ad-graph-app-migration-planning-checklist"></a>Azure AD Graph 应用迁移规划清单

使用以下清单规划从 Azure Active Directory (Azure AD) Graph 到 Microsoft Graph 的迁移。

## <a name="step-1-review-the-differences-between-the-apis"></a>步骤 1：查看 API 之间的差异

在许多方面，Microsoft Graph 类似于早期的 Azure AD Graph。 在许多情况下，只需更改代码中的终结点服务名称和版本，所有操作都应继续工作。

尽管如此，还是存在差异。 某些资源、属性、方法和核心功能已更改。

具体而言，请在以下方面查找差异：

- 两个服务之间的[请求调用语法](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)，例如目录扩展、批处理、差异查询等
- [实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型
- 请求和响应对象的[属性](migrate-azure-ad-graph-property-differences.md)
- [方法](migrate-azure-ad-graph-method-differences.md)，包括参数和类型

## <a name="step-2-examine-api-use"></a>步骤 2：检查 API 使用情况

检查应用使用的 [API](migrate-azure-ad-graph-audit-api-use.md) 及其所需的权限，并与已知差异列表进行比较。  

验证应用所需的 API 是否在 Microsoft Graph v1.0 中正式发布，并且这些 API 的工作方式相同。

在某些情况下，新功能和功能旨在取代早期方法。

使用 [Graph 资源管理器](https://aka.ms/ge) 试验新调用并开发新方法。 为了获得最佳结果，请使用测试租户中测试用户的凭据登录，以便了解 API 对重要数据集的作用。

## <a name="step-3-review-app-details"></a>步骤 3：查看应用详细信息

- [应用注册](migrate-azure-ad-graph-app-registration.md) 和许可更改 (不应) 。
- 令牌获取和 [身份验证库](migrate-azure-ad-graph-authentication-library.md)。
- 对于 .NET 应用程序，请使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。

## <a name="step-4-deploy-test-and-extend-your-app"></a>步骤 4：部署、测试和扩展应用

在为所有人更新应用之前，请确保全面测试，并向客户受众推出。

现在，你已切换到 Microsoft Graph，现在解锁更多数据集和功能（现在触手可及）从未如此简单。 可以通过查看 Microsoft Graph 中的一些 [主要服务和功能](./overview-major-services.md)来了解可能实现的功能。

[Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 现在推荐用于Microsoft 标识平台的身份验证库。 如果当前使用的是 [Azure Active Directory 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) ，请计划切换到 MSAL。 请参阅有关将 [应用程序迁移到 Microsoft 身份验证库 (MSAL) 的进一 ](/azure/active-directory/develop/msal-migration)步指南。

## <a name="next-steps"></a>后续步骤

- 了解启动步骤 1 的 [请求调用语法](migrate-azure-ad-graph-request-differences.md) ：查看 API 差异。
