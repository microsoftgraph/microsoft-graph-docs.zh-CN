---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046317"
---
# <a name="working-with-intune-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Intune  

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。  

对于移动设备管理 (MDM) 场景，适用于 Intune 的 Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。 

## <a name="using-the-intune-graph-api"></a>使用 Intune Graph API

Intune 提供数据到 Microsoft Graph 相同的方式其他云服务一样，具有丰富的实体信息的关系，以及导航。使用 Microsoft Graph 来合并来自其他服务和 Intune IT 专业人员或最终用户构建丰富跨服务应用程序的信息。     

以下是如何能够确定是否在用户的设备上安装了应用程序的方法示例： 

1. 从 Azure Active Directory 获取注册到用户的设备列表： 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. 然后，查看租户的应用程序列表： 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. 从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a>使用图权限范围

Microsof 图控制使用权限作用域的资源的访问权限。 作为开发者，你必须指定访问 Intune 资源需要的权限范围。 通常情况下，可以在 Azure Active Directory 门户中指定需要的权限范围。 有关详细信息，请参阅 [Microsoft Graph 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)和 [Intune 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)。

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a>若要使用 Microsoft Graph 网站上的目录
  
可以浏览目录 （在网站的左窗格中） 以查找您想要查看的 Intune 图形 API 和资源文档的部分。

1. 单击 **/Beta 引用**以打开 beta 文档。
2. 向下滚动并单击**Intune**。
3. 继续单击下方**Intune**的小节的 API 的部件您 
