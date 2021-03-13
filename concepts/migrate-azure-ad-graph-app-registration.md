---
title: 查看应用注册、权限和同意迁移问题
description: 介绍应用注册、权限和许可从 Azure Active Directory (Azure AD) Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 1ba0ad7c7b0826dae7c5d971f7580784447ec708
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760698"
---
# <a name="review-app-registration-permissions-and-consent"></a>查看应用注册、权限和许可

本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。

对于任何应用更新，有三个方面需要考虑：

- **应用注册**：可以在应用程序代码中继续使用现有 () `appId` 注册帐户。  

    你 **不需要** 重新注册应用以迁移到 Microsoft Graph。 只需更新代码，进行大量测试，然后部署更新。  

- **权限**：应该将配置的权限更改为等效的 Microsoft Graph 权限。 为 Azure AD Graph 授予的委派权限也会隐式视为为 Microsoft Graph 授予。 需要再次 (应用程序) 应用程序角色的应用程序权限。

    如果你的更新还表明使用了对 Azure AD Graph 不可用的特性或功能，你可能需要请求获取这些新功能的权限。 如果是这样，你可以将应用切换为使用 MSAL 和 v2 终结点，并动态请求其他/增量同意。 查看应用身份验证库更改，查找有关切换到 MSAL [的更多详细信息](./migrate-azure-ad-graph-authentication-library.md)。

- **同意**：已授予委派权限 (或已由管理员) 授予同意的最终用户无需再次授予同意即可继续使用你的应用。

    已同意你的应用访问其数据的用户可以在应用更新为使用 Microsoft Graph 后继续使用它，无需再次请求同意。 将提示新用户征得同意。

简单迁移项目应不会在这些方面遇到任何问题。

但是，如果您使用新功能、服务或添加其他功能，您可能需要新的权限，并且可能需要最终用户同意。  在这种情况下，刷新令牌时将请求同意。

## <a name="next-steps"></a>后续步骤

- 了解 [Azure](migrate-azure-ad-graph-authentication-library.md) AD Graph 和 Microsoft Graph 之间的身份验证库差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
