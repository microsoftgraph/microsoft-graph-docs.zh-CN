---
title: 应用迁移规划清单
description: 将应用程序从 Azure AD Graph 迁移到 Microsoft Graph 的清单
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 5470366e3b61cde18b52246483a46485f3f00c68
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288662"
---
# <a name="app-migration-planning-checklist"></a>应用迁移规划清单

> [!Important]
> Azure AD Graph API 现已弃用。 我们将继续提供技术支持和安全更新，但不会再提供功能更新。
> 从2022年6月30日起，我们将结束对 Azure AD Graph 的支持，将不再提供技术支持或安全更新。 此后使用 Azure AD Graph 的应用程序将不再接收来自 Azure AD Graph 终结点的响应。

使用以下检查表来规划迁移。

## <a name="step-1-review-the-differences-between-the-apis"></a>步骤1：查看 Api 之间的差异

在许多方面，Microsoft Graph 类似于早期的 Azure AD Graph。 在很多情况下，只需更改代码中的终结点服务名称和版本，一切都应继续有效。

尽管如此，也存在差异。 某些资源、属性、方法和核心功能已更改。

具体来说，请查找以下领域中的差异：

- 在两个服务之间[请求调用语法](migrate-azure-ad-graph-request-differences.md)
- [功能差异](migrate-azure-ad-graph-feature-differences.md)，如目录扩展、批处理、差异查询等
- [实体资源名称](migrate-azure-ad-graph-resource-differences.md) 及其类型
- 请求和响应对象的[属性](migrate-azure-ad-graph-property-differences.md)
- [方法](migrate-azure-ad-graph-method-differences.md)（包括参数和类型）

## <a name="step-2-examine-api-use"></a>步骤2：检查 API 使用情况

检查您的应用程序使用[的 api](migrate-azure-ad-graph-audit-api-use.md) 、所需的权限，并与已知差异的列表进行比较。  

验证应用程序所需的 Api 在 Microsoft Graph v1.0 中通常可用，并且这些 Api 的工作方式相同。

在某些情况下，新功能和功能旨在取代早期的方法。

使用 [Graph 浏览器](https://aka.ms/ge) 体验新的呼叫并开发新的方法。 为获得最佳结果，请使用测试租户中的测试用户的凭据登录，以便您可以看到 API 对重要数据集执行的操作。

## <a name="step-3-review-app-details"></a>步骤3：查看应用程序详细信息

- [应用注册](migrate-azure-ad-graph-app-registration.md) 和许可更改 () 不应为 "无"。
- 令牌获取和 [身份验证库](migrate-azure-ad-graph-authentication-library.md)。
- 对于 .NET 应用程序，使用 [客户端库](migrate-azure-ad-graph-client-libraries.md)。

## <a name="step-4-deploy-test-and-extend-your-app"></a>步骤4：部署、测试和扩展应用程序

在更新您的应用程序以供每个人更新之前，请确保全面测试并向客户访问群体转移您的部署。

现在，您已将切换到 Microsoft Graph，对现在可以轻松解锁的更多数据集和功能的方法也变得更加轻松了。 您可以通过查看一些 [示例](/graph/examples)来了解可能的情况。

如果你当前使用的是 [AD 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) ，请考虑切换到 [Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 。

## <a name="next-steps"></a>后续步骤

- 了解开始步骤1：检查 API 差异的 [请求调用语法](migrate-azure-ad-graph-request-differences.md) 。