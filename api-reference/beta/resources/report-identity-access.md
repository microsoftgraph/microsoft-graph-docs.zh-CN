---
title: 身份和访问权限报告 API 概述
description: 访问身份和访问权限报告，了解企业中的员工如何使用 Azure Active Directory 租户中的应用。
localization_priority: Priority
ms.prod: identity-and-access-reports
author: besiler
doc_type: conceptualPageType
ms.openlocfilehash: 567bfdfd848c2a7f1df19b8aad76a68774a6bf0e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129365"
---
# <a name="identity-and-access-reports-api-overview"></a>身份和访问权限报告 API 概述

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助 Microsoft Graph，你可以通过访问身份和访问权限报告，获取有关企业中的员工如何使用 Azure Active Directory (AD) 租户中的应用的信息。

## <a name="authorization"></a>授权

Microsoft Graph 通过权限控制对资源的访问。 必须指定访问报告资源所需的权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。

## <a name="what-are-identity-and-access-reports"></a>什么是身份和访问权限报告？

以下身份和访问权限报告可帮助你了解租户中的应用程序活动：

- AD FS 应用程序活动
- 应用程序登录
- 注册和使用情况

### <a name="ad-fs-application-activity"></a>AD FS 应用程序活动

AD FS 应用程序活动报告可提供与使用 Active Directory 联合身份验证服务（以下简称“AD FS”）配置的依赖方相关的信息、其聚合的使用情况，以及是否可以将信赖方配置迁移到 Azure Active Directory。 有关详细信息，请参阅 [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) 资源。

### <a name="application-sign-in"></a>应用程序登录

使用摘要报告或提供登录详细信息（例如，登录次数以及在登录过程中是否发生任何错误）的报告，评估应用程序登录使用情况。 有关详细信息，请参阅 [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) 资源。

### <a name="registration-and-usage"></a>注册和使用情况

更好地了解组织中的用户如何使用 Azure AD 功能，如自助密码重置和多重身份验证 (MFA)。 你可以确定对组织而言最有效的身份验证方法、最终用户遇到的错误类型，以及帮助最终用户接受使用自动密码重置和 MFA 所需要的市场活动。 有关详细信息，请参阅[身份验证方法使用情况 API](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)。

## <a name="next-steps"></a>后续步骤

借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。 若要了解详细信息：

- 深入了解对方案最有帮助的资源的方法和属性。
- 在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。


