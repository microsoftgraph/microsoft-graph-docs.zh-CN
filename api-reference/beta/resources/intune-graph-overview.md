---
title: 在 Microsoft Graph 中使用 Intune
description: 适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 Azure 门户执行的相同 Intune 操作。
author: dougeby
ms.localizationpriority: high
ms.prod: intune
ms.openlocfilehash: ade9b1d7579f94e84f8512d8ede342e6d57f2fcc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441151"
---
# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户** 执行的相同 Intune 操作。  

就移动设备管理 (MDM) 应用场景而言，适用于 Intune 的 Microsoft Graph API 支持独立部署；不支持 Intune [混合部署](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。

所有适用于 Intune 的 Microsoft Graph beta API 都由 Intune 团队进行测试和验证后再进行部署。 有关最新 API 更改，请参阅 [changelog](/graph/changelog)。

## <a name="using-the-microsoft-graph-api-for-intune"></a>使用适用于 Intune 的 Microsoft Graph API

Intune 向 Microsoft Graph 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。 使用 Microsoft Graph 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。     

以下示例说明如何能够确定是否在用户的设备上安装了应用程序： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>使用 Microsoft Graph 权限

Microsoft Graph 通过权限控制对资源的访问。 作为开发者，你必须指定访问 Intune 资源需要的权限。 通常是在 Azure Active Directory 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)。

## <a name="interaction-between-microsoft-graph-apis-for-windows-updates"></a>适用于 Windows 更新的 Microsoft Graph API 之间的交互

Microsoft Graph 包括两组可用于管理 Windows 更新的 API： 

- [Intune API](/graph/intune-concept-overview)
- [Windows 更新 API](/graph/windowsupdates-concept-overview)

可以使用任一 API 管理 Windows 更新；但这两个 API 彼此并不兼容。 每个 API 都可以覆盖另一 API 所做的配置，而不提供该操作的可见性。 同时使用两个 API 管理更新可能导致意外行为，包括在没有确定原因的情况下取消或修改更新部署的临时配置。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

- 了解[如何使用 Azure AD](/intune/intune-graph-apis) 访问适用于 Intune 的 Microsoft Graph API。
- 浏览 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，这些示例演示如何在工作示例上下文中使用适用于 Intune 的 Microsoft Graph API。
