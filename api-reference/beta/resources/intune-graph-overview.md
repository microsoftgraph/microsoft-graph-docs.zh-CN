---
title: 使用 Intune Graph API - Microsoft Graph API
description: 列出你可用于管理租户组织及其设备、应用、访问权限和资源的 Intune 终结点 (REST) 的 Microsoft Graph API。
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 883fce914176b2e08d49e4de414cc7c09776714a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941189"
---
# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) Intune 服务。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。  

就移动设备管理 (MDM) 应用场景而言，适用于 Intune 的 Microsoft Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>使用适用于 Intune 的 Microsoft Graph API

Intune 向 Microsoft Graph 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。使用 Microsoft Graph 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。     

以下示例说明如何能够确定是否在用户的设备上安装了应用程序： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>使用 Microsoft Graph 权限

Microsoft Graph 通过权限控制对资源的访问。 作为开发者，你必须指定访问 Intune 资源需要的权限。 通常是在 Azure Active Directory 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](https://docs.microsoft.com/zh-CN/graph/permissions-reference)。

## <a name="next-steps"></a>后续步骤

- 了解[如何使用 Azure AD](https://docs.microsoft.com/zh-CN/intune/intune-graph-apis) 访问适用于 Intune 的 Microsoft Graph API。  
- 浏览 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，这些示例演示如何在工作示例上下文中使用适用于 Intune 的 Microsoft Graph API。

