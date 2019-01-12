---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 1db77aceaab82e869fc540d2b29cce17ddba100f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911950"
---
# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。  

为移动设备管理 (MDM) 方案，Intune Microsoft Graph API 支持独立部署;不支持 Intune[混合部署](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>使用 Intune Microsoft Graph API

Intune 提供数据到 Microsoft Graph 相同的方式其他云服务一样，具有丰富的实体信息的关系，以及导航。使用 Microsoft Graph 来合并来自其他服务和 Intune IT 专业人员或最终用户构建丰富跨服务应用程序的信息。     

下面的示例演示如何确定用户的设备上是否安装了应用程序： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>使用 Microsoft Graph 权限

Microsof 图控制通过权限的资源的访问权限。 作为开发人员，您必须指定需要访问 Intune 资源的权限。 通常情况下，您将在 Azure Active Directory 门户中指定的权限。 有关详细信息，请参阅[Microsoft Graph 权限参考](https://docs.microsoft.com/en-us/graph/permissions-reference)。

## <a name="next-steps"></a>后续步骤

- 了解[如何使用 Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis)以访问 Intune Microsoft Graph API。  
- 浏览这些[PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，其中显示如何使用示例上下文中使用 Intune Microsoft Graph API。

