---
title: 查看应用身份验证库更改
description: 介绍如何更新身份验证库使用，以将应用从 Azure AD Azure Active Directory (API) 迁移到 Microsoft Graph API。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 9dfd24bb1bf956ee762c0419bce4866816fdc35e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135968"
---
# <a name="review-app-authentication-library-changes"></a>查看应用身份验证库更改

本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。

大多数应用使用身份验证库获取和管理访问令牌，以调用 Microsoft Graph。  Microsoft 提供两个身份验证库：

- [Azure Active Directory ADAL (](/azure/active-directory/develop/active-directory-authentication-libraries)身份验证库) 
- [MICROSOFT 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) 

## <a name="updating-adal"></a>更新 ADAL

如果你的应用当前使用 ADAL，请使用两阶段迁移方法：

1. 更新应用以获取 Microsoft Graph 的访问令牌。 继续使用 ADAL 执行此步骤。 更新 **resourceURL**，其中保存了表示资源 Web API 的 URI，网址为：

    `https://graph.windows.net`  

    收件人：  

    `https://graph.microsoft.com`

    在此更改后，新获取的令牌具有相同的作用域，但访问令牌的访问群体现在是 Microsoft Graph。  

    更新 **resourceURL** 和验证功能后，发布临时更新，让用户启动并运行。

1.  接下来，开始迁移应用以使用 MSAL，这是一个受支持的库，可继续操作，现已弃用 ADAL。

## <a name="migrating-to-msal"></a>迁移到 MSAL

MSAL 与 ADAL 相比提供了多个优势，包括增量同意、更丰富的单一登录体验、个人 Microsoft 帐户支持、使用基于标准的协议等。  

在将应用切换到 MSAL 时，你需要进行一些更改，包括在令牌获取请求中设置 **scopes** 参数：

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

上述表达式将权限范围请求限定为在 Azure 门户中注册应用程序期间配置的权限范围请求，并节省现有用户再次同意应用的权限范围。

有关 [此过程的直接和广泛](https://aka.ms/adal-net-to-msal-net) 帮助，包括常见错误的疑难解答和帮助，请参阅将 ADAL 迁移到 MSAL。

迁移到 MSAL 后，可以动态请求其他范围，并且用户下次使用你的应用时将提示他们提供增量同意。

## <a name="next-steps"></a>后续步骤

- 了解 Azure AD Azure Active Directory (和 Microsoft) Graph 之间的[.NET](migrate-azure-ad-graph-client-libraries.md)客户端库Graph。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
