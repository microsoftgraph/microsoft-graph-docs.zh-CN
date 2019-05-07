---
title: 查看应用注册、权限和同意迁移问题
description: 介绍从 Azure Active Directory (Azure AD) 到 Microsoft Graph API 的应用注册、权限和同意迁移。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e187fcf35f030413aa98a6cb0e34649532a8b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630277"
---
# <a name="review-app-registration-permissions-and-consent"></a>查看应用注册、权限和同意

本文是*第3步: 查看迁移应用程序的应用程序详细信息的第3步: 查看*该[过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。

对于任何应用程序更新, 有三个要考虑的方面:

- **应用注册**: 您可以继续在应用程序代码中使用现有`appId`的应用注册 ()。  

    您无**** 需重新注册您的应用程序即可迁移到 Microsoft Graph。 只需更新代码, 对其进行大量测试, 然后再部署更新。  

- **权限**: 您可以继续为您的应用程序使用现有配置的权限。 您无需请求新的权限, 因为 Azure AD Graph 权限与 Microsoft Graph 共享。

    例如, 如果现有的应用程序具有_User。 all_和_Group。 read。 all_权限, 这些权限也被隐式授予为 Microsoft Graph 的更新的应用程序。

    如果您的更新还 incudes 使用不适用于 Azure AD Graph 的功能或功能, 则您可能需要请求这些新功能的权限。 如果是这种情况, 您可以切换应用程序以使用 MSAL 和 v2 终结点, 并动态请求其他/增量许可。 在[审阅应用程序身份验证库更改](/graph/migrate-azure-ad-graph-authentication-library)中查找有关切换到 MSAL 的更多详细信息。

- **同意**: 最终用户可以继续使用您的应用程序, 而无需再次向您授予许可。

    已向你的应用程序授予访问其数据的同意的用户可以继续使用你的应用程序以使用 Microsoft Graph, 而不要求再次同意。

简单迁移项目在这些领域中不应遇到任何问题。

但是, 如果您使用新的功能、服务或添加其他功能, 则可能需要新权限, 并且可能需要最终用户同意。  在这种情况下, 会在刷新令牌时请求同意。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Graph 和 Microsoft Graph 之间的[身份验证库](migrate-azure-ad-graph-authentication-library.md)差异。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
