---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标，并创建审核日志报告，帮助你了解用户如何访问和利用 Azure AD 服务。 使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。
localization_priority: Priority
ms.openlocfilehash: 8bda9aff36ad8b46fbec3096008c2d5227058ef1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339047"
---
# <a name="azure-ad-audit-log-api-overview"></a>Azure AD 审核日志 API 概述

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标，并创建审核日志报告，帮助你了解用户如何访问和利用 Azure AD 服务。 使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。

## <a name="what-are-azure-ad-activity-logs"></a>什么是 Azure AD 活动日志？

Azure AD 提供了两种类型的活动日志：

- 审核日志 
- 登录日志

### <a name="audit-logs"></a>审核日志

通过审核日志活动报告，你可以访问在租户中执行的每项任务的历史记录。 审核日志报告为你提供了系统合规活动的记录。 除此之外，提供的数据还可让你了解常见情景，例如：

- 谁向管理员组授予了访问目录用户的权限？

- 哪些用户正在登录最近购买的应用程序？

- 在目录中进行了多少次密码重置？

### <a name="sign-in-logs"></a>登录日志

登录活动报告可帮助你确定负责执行审核日志报告所报告的任务的人员。 登录活动报告可帮助你回答如下问题：

- 用户的登录模式是什么？
- 上周有多少用户进行了登录？
- 这些登录的状态如何？

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>可以使用 Microsoft Graph 中的审核日志 API 做什么？

以下是处理审核日志数据的常见请求：

操作 | URL
:----------|:----
获取租户用户活动 | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
获取租户用户登录信息 | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

审核日志报告适用于已获得许可的功能。  如果你拥有特定功能的许可证，则还可以访问其审核日志。

例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。  若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。

登录报告需要 Azure AD Premium 许可证。

若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。

## <a name="next-steps"></a>后续步骤

- [注册你的应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足审核日志先决条件。 
- 了解[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。  
- 审查 [directoryAudit](directoryaudit.md) 资源和操作。
- 审查 [signIn](signin.md) 资源和操作。 
