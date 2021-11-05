---
title: 自定义 Microsoft Graph 中的项目见解隐私
description: 组织级别上自定义项见解的概述
author: simonhult
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: 430c44adc75bf18d44d3e3bc6d3c0fc7dc724b45
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780931"
---
# <a name="customizing-item-insights-privacy-in-microsoft-graph-preview"></a>自定义 Microsoft Graph 中的项目见解隐私（预览版）

项目见解是 Microsoft 使用高级机器学习技术计算的关系。 当用户针对文档、SharePoint 网站和列表、Teams 聊天和频道进行协作时，Microsoft 会将这些活动聚合为信号。 Microsoft 从这些信号中获得见解，为组织的用户提供以用户为中心的内容建议。

项目见解可帮助用户快速查找重要文件，例如在 Office.com 和 Delve 中的 **建议** 体验中。 用户可以在 Outlook Mobile 中的 **发现** 区域发现他们有权访问但之前可能未看到过的可能有用内容。 通过个性化见解（例如 Microsoft 365 应用中 Bing 和 **最近使用内容** 的人员卡片中的 **最近使用过的文件**），用户可轻松发现其最近使用的文件。

这些项目见解仅反映用户有权访问的内容。 没有用户会获得他们无法访问的内容的建议。

> **注意** 本文不处理 Microsoft 365 中其他基于见解的体验，例如 Viva Insights、适用于 Outlook 的 Insights 加载项、WorkWith 功能、MyAnalytics 和 Insights 仪表板。


## <a name="item-insights-privacy"></a>项目见解隐私 

项目见解隐私设置提供了在用户与 Microsoft 365 中其他项目（例如文档或站点）之间，对派生自 Microsoft Graph 见解的可见性进行配置的能力。 可通过预先存在的控件禁用 Delve 应用，但允许其他基于见解的体验，以继续提供协助。

本文介绍如何在组织中自定义项见解隐私。 要为用户自定义项见解，请参阅 [userInsightsSettings](/graph/api/resources/userinsightssettings?view=graph-rest-beta&preserve-view=true) 资源。 这些以用户为中心的设置通过 [userSettings](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) 资源中名为 **itemInsights** 的导航属性公开。

## <a name="background"></a>背景
2014 年首次发布时，Office Graph 是 Delve 的后端服务。 它们为 Office Graph 见解和 Delve 用户界面共享了一组数据保护控件。 此后，作为每个 Microsoft 365 体验和 Microsoft Graph 的一部分，Office Graph 不断发展并变得更加独立和强大。 为了提供一致的 Microsoft Graph 架构，Microsoft引入了一个 [itemInsights](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true)实体，其继承了先前存在的 [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta&preserve-view=true)资源的所有属性，并保留了 **officeGraphInsights**，以向后兼容。 **itemInsights** 的引入还使两个独立作品的隐私故事分离。  

虽然现有应用可以继续使用 **officeGraphInsights**，但这些应用应升级到 **itemInsights**，以获得在 Office Graph 和 Delve 中微调项目见解的灵活性。

## <a name="how-to-customize-item-insights"></a>如何自定义项目见解？

项目见解设置为管理员提供了使用 Azure AD 工具的灵活性。 管理员可为整个组织禁用项目见解，也可以仅针对指定 Azure AD 组的成员禁用项目见解。 他们可以在 Microsoft 365 管理中心内配置项目简介，或者使用具有适当权限的 PowerShell SDK 或 Microsoft Graph REST API 进行配置。 请记住，该操作需 要 _全局管理员角色_。 

下一部分介绍管理中心的使用，然后是有关 PowerShell cmdlet 的部分。 如果正在使用 REST API，请跳过下一部分，并继续 [使用 REST API 配置项目见解](#configure-item-insights-using-rest-api)。 有关详细信息，请参阅 [读取](/graph/api/organizationsettings-list-iteminsights?view=graph-rest-beta&preserve-view=true) 或 [更新](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) REST 操作。

### <a name="how-to-configure-item-insights-settings-via-microsoft-admin-center"></a>如何通过 Microsoft 管理中心配置项目见解设置？
拥有 _全局管理员角色_ 的管理员可以通过切换来调整项见解隐私设置。 要执行这一操作，请在 Micrsofot 365 管理中心展开“**设置**”，选择“**搜索和智能**”，并在“**项目见解**”下选择“**更改设置**”。
![图像](https://user-images.githubusercontent.com/54312959/117024482-b39eca00-ad02-11eb-9a11-e6a01039822e.png)


### <a name="how-to-configure-item-insights-settings-via-powershell"></a>如何通过 PowerShell 配置项目见解设置？
确认以下附加先决条件。 然后，你可以使用 [Microsoft Graph PowerShell SDK](./powershell/installation.md) 为整个组织或特定组设置项目见解。

#### <a name="additional-prerequisites"></a>附加先决条件
* **PowerShell 模块** - 安装 [模块 0.9.1 或更高版本](https://www.powershellgallery.com/packages/Microsoft.Graph)。
* **.NET Framework** - 安装 [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework) 或更高版本。

#### <a name="command-examples"></a>命令示例
> [!NOTE]
> 由于项目见解命令仅在 beta 版中可用，调用命令之前请切换到 beta 版配置文件。
> ```powershell
>    Select-MgProfile beta
> ```
若要获取组织的项目见解配置，请使用 Microsoft Graph PowerShell 模块和以下命令，其中用 Azure Active Directory 租户 ID 替换 `$TenantId`: 可以从 Azure Active Directory 的概览页中检索此 ID。
```powershell
   Get-MgOrganizationSettingItemInsight -OrganizationId $TenantId
```

默认情况下，将为整个组织启用项目见解。 你可以使用 Microsoft Graph PowerShell 模块来更改该设置并为组织中的所有人禁用项目见解。 
> [!NOTE]
> 更新方法需要其他 `User.ReadWrite.All` 权限。 若要创建带特定所需范围的 Microsoft Graph 会话，请使用以下命令并同意请求的权限。
> ```powershell
>    Connect-MgGraph -Scopes "User.Read.All","User.ReadWrite.All"
> ```

使用以下命令，其中用 Azure Active Directory 租户 ID 替换 `$TenantId`，并指定 `-IsEnabledInOrganization` 为 `false`。
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -IsEnabledInOrganization:$false
```
或者，也可以更改默认设置并为特定 Azure AD 组禁用项目见解。 使用以下命令，其中用 Azure Active Directory 租户 ID 替换 `$TenantId`，用 Azure Active Directory 组 ID 替换 `$GroupID`。
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -DisabledForGroup $GroupId
```

### <a name="configure-item-insights-using-rest-api"></a>使用 REST API 配置项目见解
如前所述，默认情况下，将为整个组织启用项目见解隐私设置。 这些设置通过 [organizationSettings](/graph/api/resources/organizationsettings?view=graph-rest-beta&preserve-view=true) 中名为 **itemInsights** 的导航属性公开。 可采用以下两种方式之一来更改默认设置：

- 通过将 [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) 资源的 **isEnabledInOrganization** 属性设置为`false`，为组织中的所有用户禁用项目见解。 
- 为用户的 _子集_ 禁用项目见解：将这些用户分配到一个 Azure AD 组中，将 **disabledForGroup** 属性设置为该组的 ID。 详细了解如何[创建组并将用户添加为成员](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)。 

使用 [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) 操作来相应地设置 **isEnabledInOrganization** 和 **disabledForGroup** 属性。

| 如何启用项目见解 | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| 整个组织（默认） | `true` | 空 |
| 组织用户子集禁用 | `true` | 包含用户子集的 Azure AD 组 ID |
| 整个组织禁用 | `false` | 忽略 |

更新项目见解设置时，请记住以下几点：
- [insights 设置](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) 仅在 beta 终结点中可用。
- 从 Azure 门户获取 Azure AD 组 ID，并确保该组存在，因为更新操作不会检查组是否存在。 在 **disabledForGroup** 中指定不存在的组 _不会_ 禁用组织中任何用户的见解。
- 更新设置最多可能需要 24 个小时才能应用到所有 Microsoft 365 体验中。
- 无论项目见解设置如何，Delve 都会继续采用 Delve 租户和用户级别的[隐私设置](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta&preserve-view=true)。


## <a name="behavior-changes-in-ui-and-apis"></a>UI 和 API 中的行为更改
有关禁用项见解时受影响体验的完整列表，请参阅 [项见解概述](item-insights-overview.md#disabling-item-insights)。 

## <a name="transition-period"></a>过渡期
为了适应配置项目见解设置，到 2020年底，Microsoft 365 采用 Delve 设置和项目见解设置，并且如果两者有所不同，则将两者严格化。 这意味着，如果用户通过 Delve 控件或项目见解设置选择退出，则认为用户已退出项目见解。

在此过渡期后，Delve 设置仅控制 Delve 体验，并且项目见解设置仅影响 Microsoft Graph 项目见解。 确保根据组织的要求配置项目见解。


> [!NOTE]
> 在切换期间，出于技术原因，如果组织为所有用户禁用项目见解，则 SharePoint 起始页可能会提供过时的建议。在即将进行的服务器端更改中，此问题将得以解决。 

## <a name="see-also"></a>另请参阅
了解 Delve 以及如何使用 Delve 功能设置来控制在 **发现** 源中显示的文档： 
- [在 Office Delve 中连接和协作](https://support.microsoft.com/office/connect-and-collaborate-in-office-delve-46f92806-b52c-4187-b60e-b3bf8d25f73e)
- [我的文档在 Office Delve 中安全吗？](https://support.microsoft.com/office/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3)
- [面向管理员的 Delve](/sharepoint/delve-for-office-365-admins)
