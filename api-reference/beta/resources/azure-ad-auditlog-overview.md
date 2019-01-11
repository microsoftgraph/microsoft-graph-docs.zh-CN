---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 跟踪用户活动和登录指标，并创建审核日志报告可帮助您了解您的用户如何访问和利用 Azure AD 服务。 若要分析的数据，这些报告和创建组织的特定需要的自定义解决方案，请使用 Azure AD Microsoft Graph API。
localization_priority: Priority
ms.openlocfilehash: 07d285ce4e7fbf736900c1d6d4acdf159b451424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826220"
---
# <a name="azure-ad-audit-log-api-overview"></a>Azure AD 审核日志 API 概述

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

Azure Active Directory (Azure AD) 跟踪用户活动和登录指标，并创建审核日志报告可帮助您了解您的用户如何访问和利用 Azure AD 服务。 若要分析的数据，这些报告和创建组织的特定需要的自定义解决方案，请使用 Azure AD Microsoft Graph API。

## <a name="what-are-azure-ad-activity-logs"></a>什么是 Azure AD 活动日志？

Azure AD 提供了两种类型的活动日志：

- 审核日志 
- 登录日志

### <a name="audit-logs"></a>审核日志

审核日志活动报告提供有权访问您的租户中执行每个任务的历史记录。 审核日志报告为您提供的合规性系统活动记录。 在其他中提供的数据使您能够解决常见方案，如：

- 谁将管理组的访问权限授予目录用户？

- 哪些用户登录到的最近收购的应用程序？

- 在目录内进行多少密码重置？

### <a name="sign-in-logs"></a>登录日志

登录活动报告可帮助您确定用户执行的任务报告的审核日志报告。 登录活动报告可帮助您回答以下问题：

- 什么是用户的模式登录？
- 多少用户登录过程的最后一个星期中？
- 这些登录的状态是什么？

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>使用审核日志在 Microsoft Graph 中的 Api 可以做什么？

下面是使用审核日志数据的常用请求：

操作 | URL
:----------|:----
获取用户活动的租户 | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
获取用户登录的租户 | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>是否需要哪些许可证？

审核日志报告是可用于已许可的功能。  如果您有特定功能的许可证，还可以访问其审核日志。

例如，您需要访问自助服务密码审核报告的 Azure AD Premium P1 许可证。  若要了解详细信息，请参阅[Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。

登录报告需要的 Azure AD Premium 许可证。

若要了解详细信息，请参阅[Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。

## <a name="next-steps"></a>后续步骤

- [注册应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)，以满足审核日志必备组件。 
- 了解从[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录项示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。  
- 查看[directoryAudit](directoryaudit.md)资源和操作。
- 查看[次数](signin.md)资源和操作。 
