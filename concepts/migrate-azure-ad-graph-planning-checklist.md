---
title: 应用迁移规划清单
description: 将应用程序从 Azure AD Graph 迁移到 Microsoft Graph 的清单
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59114221b91f6dc1800f9f1601cb2e2c06709ff8
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926783"
---
# <a name="app-migration-planning-checklist"></a>应用迁移规划清单

使用以下检查表来规划迁移：

## <a name="step-1-review-the-differences-between-the-apis"></a>步骤1：查看 Api 之间的差异

在许多方面，Microsoft Graph 类似于早期的 Azure AD Graph。 在很多情况下，只需更改代码中的终结点服务名称和版本，一切都应继续有效。

尽管如此，也存在差异。 某些资源、属性、方法和核心功能已更改。

具体来说，请查找以下领域中的差异：

- 在两个服务之间[请求调用语法](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)，如目录扩展、批处理、差异查询等
- [实体资源名称](migrate-azure-ad-graph-resource-differences.md)及其类型
- 请求和响应对象的[属性](migrate-azure-ad-graph-property-differences.md)
- [方法](migrate-azure-ad-graph-method-differences.md)（包括参数和类型）

## <a name="step-2-examine-api-use"></a>步骤2：检查 API 使用情况

检查您的应用程序使用[的 api](migrate-azure-ad-graph-audit-api-use.md) 、所需的权限，并与已知差异的列表进行比较。  

验证应用程序所需的 Api 在 Microsoft Graph v1.0 中通常可用，并且这些 Api 的工作方式相同。

在某些情况下，新功能和功能旨在取代早期的方法。

使用[Graph 浏览器](https://aka.ms/ge)体验新的呼叫并开发新的方法。 为获得最佳结果，请使用测试租户中的测试用户的凭据登录，以便您可以看到 API 对重要数据集执行的操作。

## <a name="step-3-review-app-details"></a>步骤3：查看应用程序详细信息

- [应用注册](migrate-azure-ad-graph-app-registration.md)和同意更改（应为 "无"）。
- 令牌获取和[身份验证库](migrate-azure-ad-graph-authentication-library.md)。
- 对于 .NET 应用程序，使用[客户端库](migrate-azure-ad-graph-client-libraries.md)。

## <a name="step-4-deploy-test-and-extend-your-app"></a>步骤4：部署、测试和扩展应用程序

在更新您的应用程序以供每个人更新之前，请确保全面测试并向客户访问群体转移您的部署。

现在，您已将切换到 Microsoft Graph，对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。 您可以通过查看一些[示例](/graph/examples)来了解可能的情况。

如果你当前使用的是[AD 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)（ADAL），请考虑切换到[Microsoft 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)（MSAL）。

## <a name="next-steps"></a>后续步骤

- 了解用于启动步骤1：审阅 API 差异的[resquest 调用语法](migrate-azure-ad-graph-request-differences.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
- 若要了解有关进度更新和时间线的详细信息，请参阅[Microsoft Graph 或 AZURE AD Graph](https://developer.microsoft.com/en-us/graph/blogs/microsoft-graph-or-azure-ad-graph/)。
