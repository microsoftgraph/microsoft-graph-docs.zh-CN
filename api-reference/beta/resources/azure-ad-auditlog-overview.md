---
title: 活动报告 API 概述
description: 使用 Microsoft Graph 中的活动报告 API 访问 Azure Active Directory 创建的报告，跟踪租户中的用户活动。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: khotz
ms.openlocfilehash: 39c84c9dc5973f28c4e148582c056da9b1e60842
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403865"
---
# <a name="activity-reports-api-overview"></a>活动报告 API 概述

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 可跟踪用户活动和创建报告，以帮助你了解用户如何访问和使用 Azure AD 服务。 使用 Microsoft Graph API for Azure AD 分析这些报告中的数据，并根据组织的特定需求创建自定义解决方案。

## <a name="what-are-activity-reports"></a>什么是活动报告？

Azure AD 提供以下三种类型的活动报告：

- 目录审核 
- 登录
- 预配

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

### <a name="provisioning"></a>预配

预配报告可帮助你查看 Azure AD 预配服务执行的所有操作。 预配报告可帮助你了解以下情况：

- 在 ServiceNow 中成功创建了哪些组？
- 从 Amazon Web 服务导入了哪些角色？
- 哪些用户从 Workday 创建失败？

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a>可以使用 Microsoft Graph 中的活动报告做什么？

以下是处理报告数据的常见请求：

操作 | URL
:----------|:----
获取租户用户活动 | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
获取租户用户登录信息 | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
获取预配日志 | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

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
- 审查 [provisioningObjectSummary](provisioningobjectsummary.md) 资源。