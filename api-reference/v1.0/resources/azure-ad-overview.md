---
title: 在 Microsoft Graph 中使用 Azure Active Directory 资源
description: '借助 Microsoft Graph，用户可以访问 Azure Active Directory (Azure AD) 资源以支持诸多应用场景，如管理管理员（目录）角色，邀请外部用户进入组织，并且，如果你是云解决方案提供商 (CSP)，则可以管理客户的数据。 Microsoft Graph 还提供了可供应用使用的方法；例如，用于发现用户的可传递组和角色成员身份的相关信息的方法。 '
ms.localizationpriority: high
author: dkershaw10
ms.prod: identity-and-access
doc_type: conceptualPageType
ms.openlocfilehash: da7518a16122573b6c8c1080085ed1ca22c67723
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019410"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Azure Active Directory 资源

借助 Microsoft Graph，用户可以访问 [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) 资源以支持诸多应用场景，如管理管理员（目录）角色，邀请外部用户进入组织，并且，如果你是[云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider)，则可以管理客户的数据。 Microsoft Graph 还提供了可供应用使用的方法；例如，用于发现用户的可传递组和角色成员身份的相关信息的方法。

> **注意**：一些 Azure AD 资源收录在 API 参考的其他部分中。有关详细信息，请参阅 [用户](users.md)和 [组](group.md)。


## <a name="authorization"></a>Authorization

若要对 Azure AD 资源调用 Microsoft Graph API，应用必须拥有适当的权限。许多已对 Azure AD 资源公开的 API 需要拥有 [_Directory_ 权限](/graph/permissions-reference#directory-permissions)之一。Directory 具有很多特权，始终需要征得管理员同意。

如果应用要代表用户（委派权限）执行操作，用户可能需要是相应的[管理员角色](/azure/active-directory/active-directory-assign-admin-roles)的成员，应用才能成功调用许多 Azure AD API。

有关委派权限和应用程序权限等权限的详细信息，请参阅[权限](/graph/permissions-reference)。

## <a name="common-use-cases"></a>常见用例

下表列出了一些 Azure AD 资源的常见用例。

| **用例**        | **REST 资源** | **另请参阅** |
|:---------------|:--------|:----------|
| **对象和方法** | | |
| `directoryObject` 是许多目录资源（如用户和组）继承自的基类。Microsoft Graph 公开了多个可用于发现用户、组和其他目录对象的相关信息的方法。例如，可以在组列表中检查可传递成员身份，也可以返回目录对象是其可传递成员的所有组和目录角色，亦可以从常规资源 ID 列表获取指定类型（如用户或组）的所有资源。 | [directoryObject](../resources/directoryobject.md) | 无 |
| **管理目录（管理员）角色** | | |
| 激活 Azure AD 租户中的目录角色，并管理目录角色中的用户成员身份。目录角色亦称为“管理员角色”。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | [在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles) |
| 跨租户应用预定义组设置或将其应用到单个资源实例。 组设置控制行为，如组显示名称的禁止使用的词语列表，是否允许来宾用户成为组所有者等。 | [groupSetting](../resources/groupsetting.md) <br/>[groupSettingTemplate](../resources/groupsettingtemplate.md)| [用于配置组设置的 Azure Active Directory cmdlet](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| **管理设备** | | |
| 管理组织中的注册设备。设备注册绑定到用户，包括笔记本电脑、台式机、平板电脑和移动电话等。设备通常是在云中使用 Device Registration Service 或 Microsoft Intune 进行创建。条件访问策略使用它们进行多重身份验证。 | [设备](../resources/device.md) | [Azure Active Directory 设备注册入门](/azure/active-directory/active-directory-device-registration-overview)。<br/><br/>[什么是 InTune？](/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[在 Intune 中注册设备以进行管理](/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **合作伙伴租户管理** | | |
| 获取与客户租户的合作关系的相关信息。<br/><br/>**注意：** 这仅适用于合作伙伴租户。合作伙伴租户是属于已加入 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 合作伙伴计划的 Microsoft 合作伙伴的 Azure AD 租户。 | [合同](../resources/contract.md) | [从云解决方案提供商应用程序中调用 Microsoft Graph](/graph/auth-cloudsolutionprovider) |
| 管理与租户关联的域。借助域操作，注册机构可以对 Microsoft 365 等服务自动执行域关联。 | [domain](../resources/domain.md) | [将自定义域名添加到 Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **租户管理** | | |
| 获取组织的相关信息，如商家地址、技术和通知联系人、订阅的服务计划及其关联域。 | [组织](../resources/organization.md) | 无 |
| 获取公司订阅的服务 SKU 的相关信息。 | [subscribedSku](../resources/subscribedsku.md) | 无 |
| 邀请外部（来宾）用户加入组织。 | [邀请](../resources/invitation.md) | [什么是 Azure AD B2B 协作？](/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b) |
| 管理组织的登录体验的品牌。 | [organizationalbranding](../resources/organizationalbrandingproperties.md) | [将品牌添加到组织的 Azure Active Directory 登录页面](/azure/active-directory/fundamentals/customize-branding)|
| **许可请求** | | |
| 管理尝试访问需要管理员授权的用户的请求许可请求工作流。  | [许可请求 API](../resources/consentrequests-root.md) |[配置管理员同意工作流](/azure/active-directory/manage-apps/configure-admin-consent-workflow) |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤
目录资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式。若要了解更多：

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。
