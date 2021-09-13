---
title: Business Central API 概述
description: 概述为什么想要将解决方案与业务中心 API 集成。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a4b932b2cbc25f967bd0e881c56f1acc0c9382d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137404"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business Central API overview (preview) 
Dynamics 365 Business Central 是一个一切一切业务管理解决方案，易于使用和适应，有助于连接业务并做出更智能的决策。 它提供你的企业端到端视图，让你能够管理财务、自动化并保护供应链、更智能地销售和改进客户服务、使项目及时且预算不足以及优化运营。

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>为什么与 Dynamics 365 Business Central 集成？
通过将应用与 Dynamics 365 Business Central 集成，可以创建跨业务需求的体验。 您可以创建使用户能够执行关键业务任务和功能的解决方案。 可以使用 Microsoft Graph访问和管理你的财务、与业务联系人合作、创建和发送销售和采购文档，以及从财务报告中获取见解。

### <a name="synchronize-your-business-applications"></a>同步业务应用程序
许多公司使用不同的断开连接的业务应用程序来管理各种业务功能。 Microsoft Graph使您可以连接数据以将这些应用程序汇集在一起。 这使得将工资单应用程序连接到员工记录、将费用应用程序连接到供应商记录以及让您的 CRM 应用程序使客户记录保持最新变得容易。 连接数据以保持应用程序同步。

### <a name="create-custom-apps-to-manage-your-business-processes"></a>创建自定义应用以管理业务流程
每个企业各不相同，可以具有专门的业务流程。 这些流程可以通过为流程定制的自定义应用来简化。 Microsoft Graph可轻松将这些应用与你的财务数据集成。 生成可现场服务销售文档的销售或采购应用程序、用于创建采购文档的费用应用或用于创建总帐明细表的工资单应用，将你的所有文档都保留到财务系统中。

### <a name="gain-insights-from-your-financial-data"></a>从财务数据获取见解
Microsoft Graph 提供对财务报表的访问权限。 连接商业智能工具和应用程序资产负债表、现金流明细表、应付款和应收帐款及试用余额报表，以创建 BI 仪表板并确保用户有权访问其需要的信息。

## <a name="authorization"></a>Authorization
使用 Azure AD v2.0 终结点对 Dynamics 365 商业中心 API 进行身份验证。 所有 API 都需要请求 `Authorization: Bearer {access-token}` 标头。 有关授权详细信息，请参阅[获取访问令牌以调用 Microsoft Graph。](./auth/index.yml)

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

请参阅[Microsoft Graph beta 中的 Dynamics 365 Business Central API。](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)


## <a name="next-steps"></a>后续步骤
详细了解 Microsoft 商业中心支持的业务中心[API](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta) Graph。
