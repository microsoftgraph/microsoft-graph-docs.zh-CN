---
title: Microsoft 365 LighthouseAPI 概述
description: Microsoft 365 Lighthouse 是一个管理门户，可帮助托管服务提供商 (MSP) 为使用 Microsoft 365 商业高级版 的中小型商业 (SMB) 客户大规模保护和管理设备、数据和用户。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 2c05851c8cffb445feb49b089112516f6d2133373490a150d0176d7a51d670b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236932"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a>使用应用程序 API 进行多租户Microsoft 365 Lighthouse概述

Microsoft 365 Lighthouse是一个管理门户，它允许托管服务提供商 (MSP) 远程管理多个客户租户。 它可帮助使用 SMB 的中小型商业 (SMB) 级 MSP 大规模保护和管理Microsoft 365 商业高级版。

Microsoft 365 Lighthouse可帮助 MSP 简化客户租户Microsoft 365 商业高级版的载入。 它提供 MSP，方便跨所有客户租户环境查看多租户。 它可推荐为 MSP 的 SMB 客户定制的安全配置基线。 借助 Microsoft 365 Lighthouse，MSP 可以扩展其客户租户的管理，重点关注最重要的内容，快速查找和调查风险，并采取措施帮助其客户租户进入健康、安全的状态。

> [!NOTE]  
> 本文档与 Microsoft Microsoft 365 Lighthouse 上提供的 Graph _API 有关_。 类似产品 Azure Lighthouse 通过使用内置于 Azure 平台的全面而稳固的管理工具，帮助服务提供商为 _Azure_ 服务提供托管服务。 若要了解更多信息，请参阅[什么是 Azure Lighthouse。](/azure/lighthouse/overview)

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>为什么与Microsoft 365 Lighthouse？

作为 MSP，您可以使用 Microsoft Graph 中的 Microsoft 365 Lighthouse API 深入了解已识别的风险，并采取措施帮助客户进入健康、安全的状态。

### <a name="devices"></a>设备

可以使用 Lighthouse API 执行以下设备任务：

- 分析 [设备合规性趋势](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) ，以更好地了解设备合规性如何随着时间的推移而发展。
- 了解 [已在整个客户](/graph/api/resources/managedtenants-manageddevicecompliance) 中创建哪些设备合规性策略以及策略的状态。

### <a name="threat-management"></a>威胁管理

可以使用 Lighthouse API 执行以下威胁管理任务：

- 深入了解客户注册用于管理的[](/graph/api/resources/managedtenants-windowsdevicemalwarestate)Windows 设备上存在恶意软件的状态。
- 查看[注册用于](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true)Windows客户管理的设备的保护状态，以确保使用这些Windows Defender的设备都运行正常。

### <a name="users"></a>用户

可以使用 Lighthouse API 执行以下用户任务：

- 在 [客户中发现](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) 有风险的用户。
- 查看 [凭据用户注册摘要](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) ，了解你的客户中哪些用户注册了多重身份验证和自助服务密码重置。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

请参阅[microsoft Microsoft 365 Lighthouse 预览版中的 Graph (API) 。 ](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true)

> [!NOTE]
> 该Microsoft 365 Lighthouse API 在 OData 子名称空间中定义 `microsoft.graph.managedTenants` 。


## <a name="next-steps"></a>后续步骤

- 详细了解 Microsoft 365 Lighthouse[门户。](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true)
- 了解 Lighthouse [](/graph/whats-new-overview) API 的最新新功能和更新。
- 浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
