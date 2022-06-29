---
title: 使用 Microsoft 365 Lighthouse API 管理多个客户租户
description: Microsoft Graph 中的Microsoft 365 Lighthouse可帮助 MSP 远程管理使用Microsoft 365 商业高级版的客户的设备、数据和用户。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 8a59b310ef6ae5b5d50b423fc013b25bede133f4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440689"
---
# <a name="manage-multiple-customer-tenants-using-the-microsoft-365-lighthouse-api"></a>使用 Microsoft 365 Lighthouse API 管理多个客户租户

Microsoft 365 Lighthouse是一个管理门户，允许托管服务提供商 (MSP) 远程管理多个客户租户。 它可帮助 MSP 大规模保护和管理设备、数据和用户，使中小型企业 (SMB) 使用Microsoft 365 商业高级版的客户。

Microsoft 365 Lighthouse可帮助 MSP 简化Microsoft 365 商业高级版客户租户的载入。 它为 MSP 提供了跨其所有客户租户环境的多租户视图的便利性。 它可以建议为 MSP 的 SMB 客户定制安全配置基线。 借助Microsoft 365 Lighthouse，MSP 可以扩展其客户租户的管理，专注于最重要的内容，快速查找和调查风险，并采取措施帮助客户租户进入健康且安全的状态。

> [!NOTE]  
> 本文档介绍 _Microsoft Graph_ 中提供的Microsoft 365 Lighthouse API。 类似的产品/服务 Azure Lighthouse 通过使用 Azure 平台中内置的全面可靠的管理工具，帮助服务提供商为 _Azure_ 服务提供托管服务。 若要了解详细信息， [请参阅什么是 Azure Lighthouse](/azure/lighthouse/overview)。

## <a name="why-integrate-with-microsoft-365-lighthouse"></a>为什么要与Microsoft 365 Lighthouse集成？

作为 MSP，可以使用 Microsoft Graph 中的 Microsoft 365 Lighthouse API 深入了解已识别的风险，并采取措施帮助客户进入健康且安全的状态。

### <a name="devices"></a>设备

可以使用 Lighthouse API 执行以下设备任务：

- 分析 [设备符合性趋势](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) ，以便更好地了解设备符合性如何随着时间推移而发展为客户。
- 了解已在客户中创建了哪些 [设备符合性策略](/graph/api/resources/managedtenants-manageddevicecompliance) 以及策略的状态。

### <a name="threat-management"></a>威胁管理

可以使用 Lighthouse API 执行以下威胁管理任务：

- 深入了解客户注册进行管理的 Windows 设备上存在的 [恶意软件](/graph/api/resources/managedtenants-windowsdevicemalwarestate) 状态。
- 查看在客户之间注册进行管理的 Windows 设备的[保护状态](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true)，以确保使用Windows Defender的设备处于正常状态。

### <a name="users"></a>用户

可以使用 Lighthouse API 执行以下用户任务：

- 发现客户中 [存在风险的用户](/graph/api/resources/riskyuser) 。
- 查看 [凭据用户注册摘要](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) ，了解客户中哪些用户注册了多重身份验证和自助密码重置。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

请参阅 [Microsoft Graph (预览) 中的Microsoft 365 Lighthouse API](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true)。

> [!NOTE]
> Microsoft 365 Lighthouse API 是在 OData 子名空间中定义的。 `microsoft.graph.managedTenants`


## <a name="next-steps"></a>后续步骤

- 详细了解[Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true)门户。
- 了解 Lighthouse API [的最新新功能和更新](/graph/whats-new-overview) 。
- 浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
