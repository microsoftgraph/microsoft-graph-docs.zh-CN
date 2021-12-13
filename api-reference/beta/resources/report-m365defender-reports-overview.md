---
title: 报告属于 Microsoft Defender for Office 365 的攻击模拟培训的 API 概述
description: 本节介绍了访问属于 Microsoft Defender for Office 365 的安全报告的 API。
ms.localizationpriority: high
author: Gopal-MSFT
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 76d41d429145da44d7d094d3a0d310a7e6a0c142
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424754"
---
# <a name="reports-api-overview-for-attack-simulation-training-as-part-of-microsoft-defender-for-office-365"></a>报告属于 Microsoft Defender for Office 365 的攻击模拟培训的 API 概述

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

本节介绍了 Microsoft Defender for Office 365 的报告功能，具体来说是访问租户参与攻击模拟培训报告的 API。 攻击模拟培训会设置良性网络攻击模拟以培训租户中的用户，从而提高其意识，并帮助识别易受攻击的用户。

## <a name="what-role-do-the-attack-simulation-reports-play-in-enterprise-defense"></a>攻击模拟报告在企业防御中的作用是什么?

攻击模拟报告有助于租户管理员识别安全知识差距，从而进一步培训用户以降低其对攻击的易感性。 攻击模拟培训服务是 [Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true) 的一部分，可以保护组织免于电子邮件、链接(URL)以及协作工具带来的恶意威胁。

Microsoft Defender for Office 365 属于 [Microsoft 365 Defender](/microsoft-365/security/defender/microsoft-365-defender?view=o365-worldwide&preserve-view=true) 套件，其中包含以下服务:

- [Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)
- [Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/overview)
- [Microsoft Defender for Identity](/defender-for-identity/)
- [Microsoft Defender for Cloud Apps](/cloud-app-security/)

Microsoft 365 Defender 是一种统一的企业防御套件，有助于检测安全风险、调查对组织的攻击以及自动防止有害活动。 其提供了中心管理员门户([https://security.microsoft.com/](https://security.microsoft.com))，该门户将保护、检测、调查以及响应 _电子邮件_、_协作_、_标识_ 和 _设备_ 威胁相结合。

要访问攻击模拟培训，请打开 Microsoft 365 Defender 门户，转到 **电子邮件与协作** > **攻击模拟培训**。


## <a name="authorization"></a>授权

Microsoft Graph 通过权限控制对资源的访问。 必须指定访问报告资源所需的权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference) 和 [报告权限](/graph/permissions-reference#reports-permissions)。

## <a name="what-kinds-of-data-do-the-reports-return"></a>报告会返回哪些类型的数据?

| 数据类型          | 资源                                | API         |
|:---------------------- |:--------------------------------------- |:------------|
| 租户中易受攻击的重复违规者 | [attackSimulationRepeatOffender](attacksimulationrepeatoffender.md) | [getAttackSimulationRepeatOffenders](../api/reportroot-getattacksimulationrepeatoffenders.md) |
| 租户中每个用户的模拟数据和结果 | [attackSimulationSimulationUserCoverage](attacksimulationsimulationusercoverage.md) | [getAttackSimulationSimulationUserCoverage](../api/reportroot-getattacksimulationsimulationusercoverage.md) |
| 租户中每个用户的培训覆盖范围 | [attackSimulationTrainingUserCoverage](attacksimulationtrainingusercoverage.md) | [getAttackSimulationTrainingUserCoverage](../api/reportroot-getattacksimulationtrainingusercoverage.md) |

## <a name="next-steps"></a>后续步骤

报表资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式。要了解详细信息，请：

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

