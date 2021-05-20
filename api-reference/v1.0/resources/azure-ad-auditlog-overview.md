---
title: 活动报告 API 概述
description: 使用 Microsoft Graph 中的活动报告 API 访问 Azure Active Directory 创建的报告，跟踪租户中的用户活动。
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 28d09cfe7dcb78480e02e5a2a23893495eb6655f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546208"
---
# <a name="activity-reports-api-overview"></a>活动报告 API 概述

命名空间：microsoft.graph

Azure Active Directory (Azure AD) 可跟踪用户活动和创建报告，以帮助你了解用户如何访问和使用 Azure AD 服务。 使用 Microsoft Graph API for Azure AD 分析这些报告中的数据，并根据组织的特定需求创建自定义解决方案。

这些活动报告的可用性受 Azure AD 的数据保留策略管理。 有关详细信息，请参阅 [数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)。

## <a name="what-are-azure-ad-activity-logs"></a>什么是 Azure AD 活动日志？

Azure AD 提供以下三种类型的活动报告：

- 目录审核
- 登录

### <a name="directory-audits"></a>目录审核

借助目录审核报告，你可以获取租户中执行的每项任务的历史记录。 目录审核报告为你提供了系统合规活动的记录。 除此之外，提供的数据还可让你了解常见情景，例如：

- 谁向管理员组授予了访问目录用户的权限？
- 哪些用户正在登录最近购买的应用程序？
- 在目录中进行了多少次密码重置？

### <a name="sign-ins"></a>登录

登录活动报告可帮助你确定负责执行目录审核所报告的任务的人员。 登录报告可帮助你回答如下问题：

- 用户的登录模式是什么？
- 上周有多少用户进行了登录？
- 这些登录的状态如何？

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>可以使用 Microsoft Graph 中的审核日志 API 做什么？

以下是处理审核日志数据的常见请求：

Operation | URL
:----------|:----
获取租户用户活动 | [GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
获取租户用户登录信息 | [GET https://graph.microsoft.com/v1.0/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a>需要哪些许可证？

活动报告适用于已获得许可的功能。 如果你拥有特定功能的许可证，则还可以访问报告。

例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。  若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。

登录报告需要 Azure AD Premium 许可证。

若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。

## <a name="next-steps"></a>后续步骤

- [注册你的应用程序](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足报告先决条件。 
- 了解[审核日志](/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。  
- 审查 [directoryAudit](directoryaudit.md) 资源和操作。
- 审查 [signIn](signin.md) 资源和操作。 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
