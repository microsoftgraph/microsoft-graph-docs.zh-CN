---
title: 'Dynamics 365 Business Central API 概述 (预览) '
description: 使用 Dynamics 365 Business Central（一种一体式的业务管理解决方案）来管理财务、自动化供应链并使项目保持预算。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 393e2e192ccb6b6d4792d567fce60e87a8832b88
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440899"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business Central API 概述 (预览) 
Dynamics 365 Business Central 是一种一体式的业务管理解决方案，易于使用和适应，可帮助你连接业务并做出更明智的决策。 它提供业务端到端视图，使你能够管理财务、自动化和保护供应链、更智能地销售和改善客户服务、按时保持项目和预算，以及优化运营。

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>为什么要与 Dynamics 365 Business Central 集成？
通过将应用与 Dynamics 365 Business Central 集成，可以创建满足业务需求的体验。 可以创建解决方案，使用户能够执行关键业务任务和功能。 可以使用 Microsoft Graph 访问和管理财务，与业务联系人协作，创建和发送销售和购买文档，并从财务报表中获取见解。

### <a name="synchronize-your-business-applications"></a>同步业务应用程序
许多公司使用不同、断开连接的业务应用程序来管理业务的各种功能。 Microsoft Graph 使你能够连接数据，将这些应用程序整合在一起。 这样便可以轻松地将你的工资单应用程序连接到员工记录、将费用应用程序连接到供应商记录，以及让 CRM 应用程序使客户记录保持最新。 连接数据以使应用程序保持同步。

### <a name="create-custom-apps-to-manage-your-business-processes"></a>创建自定义应用以管理业务流程
每个业务都不同，可以有专门的业务流程。 可以使用为该进程定制的自定义应用简化这些进程。 借助 Microsoft Graph，可以轻松地将这些应用与财务数据集成。 生成可创建销售文档的销售或现场服务应用、创建购买文档的费用应用，或创建一般账本日志的工资单应用，将所有文档保留在财务系统中。

### <a name="gain-insights-from-your-financial-data"></a>从财务数据中获取见解
Microsoft Graph 提供对财务报表的访问权限。 将 BI 工具和应用连接到资产负债表、现金流报表、应收账款和应收账款老化报表，以及试用余额报告，以创建 BI 仪表板，并确保用户有权访问所需的信息。

## <a name="authorization"></a>Authorization
使用 Azure AD v2.0 终结点对 Dynamics 365 Business Central API 进行身份验证。 所有 API 都需要 `Authorization: Bearer {access-token}` 请求标头。 有关授权的详细信息，请参阅 [获取用于调用 Microsoft Graph 的访问令牌](./auth/index.yml)。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph beta 中的 Dynamics 365 Business Central API](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta&preserve-view=true)
