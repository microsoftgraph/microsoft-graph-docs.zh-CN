---
title: 自定义 Microsoft Graph 中的项目见解隐私
description: ''
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: a2f4c86c5c4de0d87034e2db708adde270e1b243
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427493"
---
# <a name="customizing-item-insights-privacy-in-microsoft-graph-preview"></a>自定义 Microsoft Graph 中的项目见解隐私（预览版）

项目见解隐私设置提供了在用户与 Microsoft 365 中其他项目（例如文档或站点）之间，对派生自 Microsoft Graph 见解的可见性进行配置的能力。 可通过预先存在的控件禁用 Delve 应用，但允许其他基于见解的体验，以继续提供协助。

## <a name="background"></a>背景
2014 年首次发布时，Office Graph 是 Delve 的后端服务。 它们为 Office Graph 见解和 Delve 用户界面共享了一组数据保护控件。 此后，作为每个 Microsoft 365 体验和 Microsoft Graph 的一部分，Office Graph 不断发展并变得更加独立和强大。 为了提供一致的 Microsoft Graph 架构，Microsoft引入了一个[itemInsights](/graph/api/resources/itemInsights?view=graph-rest-beta)实体，其继承了先前存在的 [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta)资源的所有属性，并保留了** officeGraphInsights**，以向后兼容。 **itemInsights** 的引入还使两个独立作品的隐私故事分离。  

虽然现有应用可以继续使用 **officeGraphInsights**，但这些应用应升级到 **itemInsights**，以获得在 Office Graph 和 Delve 中微调项目见解的灵活性。

## <a name="how-to-customize-item-insights"></a>如何自定义项目见解？
默认情况下，将为组织启用项目见解。 要为组织中的所有用户禁用项目见解，请将 **isEnabledInOrganization** 属性设置为 `false`。 若要禁用 Azure AD 组中用户_子集_的项目见解，将 **disabledForGrou ** 属性设置为该组的 ID；了解有关[创建群组并将用户添加为成员](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)的详细信息。 

这些设置为管理员提供了灵活性，使其可以使用 Azure AD 工具并仅对指定组的成员而不是整个组织禁用项目见解。 通过在某个应用程序、PowerShell 或具有适当权限的其它应用中[更新项目见解设置](/graph/api/iteminsightssettings-update?view=graph-rest-beta)，配置每个属性。

注意，读取或更新这些设置需要_全局管理员角色_。 

### <a name="available-configurations"></a>可用配置
通过相应[更新](/graph/api/iteminsightssettings-update?view=graph-rest-beta) **isEnabledInOrganization** 和 **disabledForGroup** 属性，配置组织中用户的项目见解设置。

| 如何启用项目见解 | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| 整个组织（默认） | `true` | 空 |
| 组织用户子集禁用 | `true` | 包含用户子集的 Azure AD 组 ID |
| 整个组织禁用 | `false` | 忽略 |

更新项目见解设置时，请记住以下几点：
- 项目见解隐私设置(**itemInsightsSettings** 资源)仅在 beta 终结点中可用。
- 从 Azure 门户获取 Azure AD 组 ID，并确保该组存在，因为更新操作不会检查组是否存在。 在 **disabledForGroup** 中指定不存在的组_不会_禁用组织中任何用户的见解。
- 更新设置最多可能需要 8 个小时才能应用到所有 Microsoft 365 体验中。
- 无论项目见解设置如何，Delve 都会继续采用 Delve 租户和用户级别的[隐私设置](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta)。


## <a name="behavior-changes-in-ui-and-apis"></a>UI 和 API 中的行为更改
某些[趋势](/graph/api/resources/insights-trending)或[已使用](/graph/api/resources/insights-used)的见解可能会受到影响，如下所述。 随着时间推移，这些见解的范围和类型将得到扩展。 

- 对于禁用项目见解的用户，个人资料卡不会显示其**使用过的**文档。 相同的限制适用于 Microsoft 必应搜索的配置文件结果，其中“**最近文件**”窗格为空。 此外，降低了首字母缩写词扩展搜索精度。

- 在 Delve 中，禁用项目见解的用户将其文档隐藏。 

- 禁用项目见解的任何用户的活动都将从组织范围的见解中删除。 通常，此类分析会为用户的同事提供从 Outlook 到 OneDrive 和 SharePoint 的多种体验的辅助见解。 无论设置如何，分析始终是匿名的，但是当用户禁用见解时，该用户的活动将无法提高其他人的工作效率。

- 对于已禁用项目见解的用户，在 Microsoft Graph API 中查询[趋势](/graph/api/resources/insights-trending)和[已使用](/graph/api/resources/insights-used)资源将返回 `HTTP 403 Forbidden`。


## <a name="transition-period"></a>过渡期
为了适应配置项目见解设置，到 2020年底，Microsoft 365 采用 Delve 设置和项目见解设置，并且如果两者有所不同，则将两者严格化。 这意味着，如果用户通过 Delve 控件或项目见解设置选择退出，则认为用户已退出项目见解。

在此过渡期后，Delve 设置仅控制 Delve 体验，并且项目见解设置仅影响 Microsoft Graph 项目见解。 确保根据组织的要求配置项目见解。


> [!NOTE]
> 过渡期间，由于技术原因，如果组织为所有用户禁用项目见解，则 SharePoint 起始页可能会提供过时的建议。 此问题将在未来的服务器端更改中得到解决。 
