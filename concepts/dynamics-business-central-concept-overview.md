---
title: Business Central API 概述
description: 概述为什么要将您的解决方案与业务中心 Api 集成。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 27e9a13b41ce2b8e46321eef2afc4e103248281b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951185"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business 中央 API 概述 (预览)
Dynamics 365 Business Central 是一个易于使用和调整的一体式业务管理解决方案, 可帮助您连接业务并做出更明智的决策。 它提供了业务的端到端视图, 使您能够管理财务、自动化和保护供应链、更智能化地销售和改进客户服务、使项目按时完成并在预算范围之内, 并优化您的操作。

## <a name="why-integrate-with-dynamics-365-business-central"></a>为什么要与 Dynamics 365 业务中心集成？
通过将应用与 Dynamics 365 业务中心集成, 可以创建满足业务需求的经验。 您可以创建可让用户执行关键业务任务和功能的解决方案。 您可以使用 Microsoft Graph 访问和管理您的财务、与业务联系人合作、创建和发送销售和采购文档, 并从财务报表获取见解。

### <a name="synchronize-your-business-applications"></a>同步业务应用程序
许多公司使用不同的断开连接的业务应用程序来管理企业的各种功能。 通过 Microsoft Graph, 可以连接数据以将这些应用程序一起引入。 这使您可以轻松地将工资应用程序连接到员工记录, 将您的费用应用程序连接到供应商记录, 并让您的 CRM 应用程序保持您的客户记录保持最新。 连接数据以保持应用程序同步。

### <a name="create-custom-apps-to-manage-your-business-processes"></a>创建用于管理业务流程的自定义应用程序
每个企业都不同, 并且可以有专门的业务流程。 可以使用针对此过程量身定制的自定义应用程序简化这些过程。 使用 Microsoft Graph, 可以轻松地将这些应用与财务数据集成。 建立 sales 或 field service 应用程序来创建销售文档、创建采购文档的费用应用程序或创建总帐日志的工资应用程序是可行的, 并将所有文档保留在财务系统中。

### <a name="gain-insights-from-your-financial-data"></a>深入了解你的财务数据
Microsoft Graph 提供了对财务报告的访问权限。 将 BI 工具和应用程序连接到资产负债表、现金流量表、应付帐款和应收帐款帐龄报告和试用余额报告, 以创建 BI 仪表板, 并确保用户有权访问他们所需的信息。

## <a name="authorization"></a>Authorization
使用 Azure AD v2。0终结点对 Dynamics 365 Business Central Api 进行身份验证。 所有 Api 都需要`Authorization: Bearer {access-token}`请求标头。 有关授权的详细信息, 请参阅[获取访问令牌以调用 Microsoft Graph](/graph/auth)。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

请参阅[Dynamics 365 Business CENTRAL API In Microsoft Graph beta 版](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)。


## <a name="next-steps"></a>后续步骤
了解有关 Microsoft Graph 中支持的[业务中心 API 和使用案例](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)的详细信息。
