---
title: 自定义 Microsoft Graph 中的人员见解隐私
description: 了解如何使用 Microsoft Graph API 在组织级别自定义人员见解。
author: anthona
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: 03bd6d41435eb7c6d6b8f5460e559a52ef48b5e8
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60781009"
---
# <a name="customizing-people-insights-privacy-in-microsoft-graph-preview"></a>自定义 Microsoft Graph 中的项目见解隐私

人员见解表示根据人员之间的公共关系， [与同一组织内的](people-example.md#including-a-person-as-relevant-or-working-with) 彼此相关或相互协作的人员的连接。 这些见解可以显示在Delve和个人资料卡片中，并且由[人员 API](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true) 返回。


## <a name="customizing-people-insights-for-an-organization"></a>为组织自定义人员见解

默认情况下，可以为组织显示或返回人员见解。 具有此全局管理员角色管理员可以使用 REST API 和相应权限为组织自定义此行为。 他们可以通过以下方式设置 [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) 资源的属性来自定义：

- 为组织中的所有用户禁用人员见解：将 **insightsSettings** 资源的 **isEnabledInOrganization** 属性设置为 `false`。 （默认情况下， **isEnabledInOrganization** 属性为 `true`。）

- 为用户的子集禁用人员见解：将这些用户分配到一个 Azure Active Directory (Azure AD) 组中，将 **disabledForGroup** 属性设置为该组的 ID。 详细了解如何[创建组并将用户添加为成员](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)。 

使用 [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) 操作来相应地设置 **isEnabledInOrganization** 和 **disabledForGroup** 属性。 

更新项目见解设置时，请记住以下几点： 
* 人员见解设置仅可用于 beta 版终结点。 
* 更新操作不会验证组是否存在。 确保从 Azure 门户获取 Azure AD 组的正确 ID，验证该组是否存在，并且目标用户已添加到组。 如果组不存在，不会对组织中的任何用户进行更改。 
* 更新 **insightsSettings** 可能需要长达 8 小时才能生效。 

## <a name="behavior-changes-in-the-microsoft-365-ui-and-people-api"></a>Microsoft 365 UI 和人员 API 中的行为更改 

禁用人员见解意味着不会为指定用户生成数据。 它不会影响结果的搜索和排名。

为人员见解自定义隐私时，可以观察到以下方面的行为变化：
* Microsoft 365 [个人资料卡片](https://support.microsoft.com/office/profile-cards-in-microsoft-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)
* Delve 中的用户个人资料
* [列出相关人员](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true)。

