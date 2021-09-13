---
title: 使用 REST API 访问 Exchange 混合部署中的邮箱（预览版）
description: 在属于 Microsoft 365 的 Exchange Online 中，Microsoft Graph 始终提供对云中客户邮箱的访问权限。
ms.localizationpriority: high
ms.openlocfilehash: 6234d90e23d3db903f63127f94a30c160db1a612
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055750"
---
# <a name="use-rest-apis-to-access-mailboxes-in-exchange-hybrid-deployments-preview"></a>使用 REST API 访问 Exchange 混合部署中的邮箱（预览版）

在作为 Microsoft 365 一部分的 Exchange Online 中，Microsoft Graph 始终提供对云中客户邮箱的访问权限。Exchange 本地服务器的 Exchange 2016 累积更新 3 (CU3) 于 2016 年 9 月发布，增加了对 REST API 与 Microsoft 365 集成的支持。如果你的应用使用 v1.0 的 [邮件](/graph/api/resources/message?view=graph-rest-1.0)、[日历](/graph/api/resources/calendar?view=graph-rest-1.0)或 [联系人](/graph/api/resources/contact?view=graph-rest-1.0) API，则只要部署满足特定的 [要求](#requirements-for-the-rest-api-to-work-in-hybrid-deployments)，现在还可以在 _混合_ 部署中找到无缝的身份验证和应用程序体验，而不论该邮箱是在本地还是在云中。 


当 Microsoft Graph 在后台识别到一个 REST API 调用正在尝试访问混合部署中的本地邮箱时，它会将 REST 请求代理到本地 REST 终结点，然后处理此请求。此发现使得访问 REST API 成为可能。

>**注意：** 在混合部署中使用这些 REST API 的功能目前处于预览阶段。

>只有 v1.0 的邮件、日历和联系人 API 可用于混合部署中的邮箱。其他 v1.0 API 集，如[组](/graph/api/resources/group?view=graph-rest-1.0) API，或者其他版本中的 API 都不能用于上述邮箱。如果尝试使用的 API 不是混合部署中受支持的 API 集，则会收到以下错误消息：

>“此邮箱的 REST API 当前处于预览阶段。可以在 https://dev.outlook.com 中查找有关预览 REST API 的详细信息。”

## <a name="requirements-for-the-rest-api-to-work-in-hybrid-deployments"></a>REST API 用于混合部署的要求

Microsoft Graph 提供开放性（支持 JSON、OAUTH 和 ODATA 等开放标准，从大多数主流平台连接）和灵活性（用户数据的精确、范围严格的访问权限）。 如果贵组织有兴趣启用 Microsoft Graph 应用开发，并且正在使用或考虑混合部署，请注意以下部署要求：

- 邮箱要求

  - 所有将使用 REST API 的本地邮箱必须位于处于 Exchange 2016 CU3 服务器的数据库中。 

- 基础结构要求

  - 所有 Exchange 2016 服务器必须升级到 CU3 或更高版本。  
  - 本地 Active Directory 必须与 Azure Active Directory 同步。
  - 必须将同一负载平衡的数组上与 Exchange 2016 服务器共存的所有 Exchange 2013 服务器从数组中删除。

- 网络要求

  - 从 DNS 的角度看，自动发现命名空间和本地客户端命名空间必须具有 Internet DNS 记录。 
  - 如果具有检查和限制访问的防火墙或应用程序网关，请更新相应的设置，以允许进行发现和访问。


IT 管理员可以在以下资源中找到详细信息：

- [Exchange Server 混合部署](/exchange/exchange-hybrid)
- [2016 年 9 月累积更新版本](https://blogs.technet.microsoft.com/exchange/2016/09/20/released-september-2016-quarterly-exchange-updates/) 
- [针对 REST API 的本地体系结构要求](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)
