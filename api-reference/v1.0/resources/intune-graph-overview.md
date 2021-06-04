---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
author: dougeby
localization_priority: Priority
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: baad1c809bfd34dd60bab009b7b83c5fcb46dddf
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732400"
---
# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) Intune 服务。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户** 执行的相同 Intune 操作。  

就移动设备管理 (MDM) 应用场景而言，适用于 Intune 的 Microsoft Graph API 支持独立部署；不支持 Intune [混合部署](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。 

## <a name="using-the-microsoft-graph-api-for-intune"></a>使用适用于 Intune 的 Microsoft Graph API

Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。 使用 Microsoft Graph API 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。     

以下示例说明如何能够确定是否在用户的设备上安装了应用程序： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a>访问适用于 Intune 的 Microsoft Graph API

Intune 同时支持[委托的权限](/graph/auth-v2-user)和[应用程序权限](/graph/auth-v2-service)。 委托的权限和应用程序权限都支持读取和写入操作。 委托的权限和应用程序权限都支持单租户应用程序和多租户应用程序。 若要详细了解可通过 Microsoft Graph 获取的权限，请参阅 [ Microsoft Graph 权限参考](/graph/permissions-reference)。

## <a name="using-permissions"></a>使用权限

Microsoft Graph API 通过权限控制对资源的访问。 作为开发者，你必须指定访问 Intune 资源需要的权限。 通常是在 Azure Active Directory 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

- 了解[如何使用 Azure AD](/intune/intune-graph-apis) 访问适用于 Intune 的 Microsoft Graph API。  
- 浏览 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，这些示例演示如何在工作示例上下文中使用适用于 Intune 的 Microsoft Graph API。