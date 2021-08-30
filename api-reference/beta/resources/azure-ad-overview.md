---
title: 在 Microsoft Graph 中使用 Azure Active Directory 资源
description: Microsoft Graph Azure Active Directory (Azure AD) 提供 REST API，以帮助管理你的组织、资源和资产。
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: identity-and-access
author: dkershaw10
ms.openlocfilehash: f9556ca4f908533b2934ec381368b0845917819e
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696321"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Azure Active Directory 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助 Microsoft Graph，用户可以访问 [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) 资源以支持诸多应用场景，如管理管理员（目录）角色，邀请外部用户进入组织，并且，如果你是[云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider)，则可以管理客户的数据。 Microsoft Graph 还提供了应用可使用的方法；例如，用于发现用户的可传递组和角色成员身份的相关信息的方法。

> **注意**：一些 Azure AD 资源收录在 API 参考的其他部分中。有关详细信息，请参阅 [用户](users.md)和 [组](group.md)。


## <a name="authorization"></a>Authorization

若要对 Azure AD 资源调用 Microsoft Graph API，应用必须拥有适当的权限。许多已对 Azure AD 资源公开的 API 需要拥有 [_Directory_ 权限](/graph/permissions-reference#directory-permissions)之一。Directory 具有很多特权，始终需要征得管理员同意。

如果应用要代表用户（委派权限）执行操作，用户可能需要是相应的[管理员角色](/azure/active-directory/active-directory-assign-admin-roles)的成员，应用才能成功调用许多 Azure AD API。

有关委派权限和应用程序权限等权限的详细信息，请参阅[权限](/graph/permissions-reference)。

## <a name="common-use-cases"></a>常见用例

下表列出了一些 Azure AD 资源的常见用例。

| **用例**        | **REST 资源** | **另请参阅** |
|:-----------------|:--------|:----------|
| **对象和方法** | | |
| `directoryObject` 是许多目录资源（如用户和组）继承自的基类。Microsoft Graph 公开了多个可用于发现用户、组和其他目录对象的相关信息的方法。例如，可以在组列表中检查可传递成员身份，也可以返回目录对象是其可传递成员的所有组和目录角色，亦可以从常规资源 ID 列表获取指定类型（如用户或组）的所有资源。 | [directoryObject](../resources/directoryobject.md) | 不适用 |
| **管理目录（管理员）角色、管理单元、目录设置和策略** | | |
| 激活 Azure AD 租户中的目录角色，并管理目录角色中的用户成员身份。目录角色亦称为“管理员角色”。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)|
| 管理管理单元。 目录角色向其成员委派租户机构。 管理员可以创建和管理管理单元，以便向用户更精确地委培具有范围限定的管理机构。 | [administrativeUnit](../resources/administrativeunit.md) | [Azure AD 中的管理单元管理](/azure/active-directory/active-directory-administrative-units-management) |
| 跨租户应用预定义目录设置或将其应用到单个资源实例。 目前，仅支持 Microsoft 365 组设置。 跨租户应用预定义组设置或将其应用到单个资源实例。组设置控制行为，如组显示名称的禁止使用的词语列表，是否允许来宾用户成为组所有者等。 | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [用于配置组设置的 Azure Active Directory cmdlet](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| 将 Azure AD 策略应用到应用程序、服务主体、组或整个组织。 支持声明映射、令牌颁发、令牌生存期、主页领域发现等策略。  | [可用策略](../resources/policy-overview.md) | 不适用 |
| **保护至 Azure AD 的特权访问** | | |
| 利用 Privileged Identity Management (PIM) 为管理员和 IT 专业人员管理和监控至目录和 Azure 资源的具有时间限定的特权访问。 | [Privileged Identity Management API](../resources/privilegedidentitymanagement-root.md) | [什么是 Azure AD Privileged Identity Management？](/azure/active-directory/active-directory-privileged-identity-management-configure)|
| 监视身份风险事件，如用户从被恶意感染的设备或从不熟悉的位置登录。 | [Identity Protection 服务 API](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](/azure/active-directory/active-directory-identityprotection)<br/><br/>[Azure Active Directory 风险事件](/azure/active-directory/active-directory-reporting-risk-events) |
| **管理设备** | | |
| 管理组织中的注册设备。设备注册绑定到用户，包括笔记本电脑、台式机、平板电脑和移动电话等。设备通常是在云中使用 Device Registration Service 或 Microsoft Intune 进行创建。条件访问策略使用它们进行多重身份验证。 | [设备](../resources/device.md) | [Azure Active Directory 设备注册入门](/azure/active-directory/active-directory-device-registration-overview) |
| **应用管理** | | |
| 管理开发人员租户中的应用配置。 | [应用](../resources/application.md) | [Azure Active Directory 中的应用程序和服务主体对象](/azure/active-directory/develop/active-directory-application-objects) |
| 管理租户中安装的应用。 | [servicePrinicpal](../resources/serviceprincipal.md) | [Azure Active Directory 中的应用程序和服务主体对象](/azure/active-directory/develop/active-directory-application-objects) |
| 管理租户安装的应用中的用户和管理员许可的权限。 | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | 不适用 |
| 管理租户中安装的应用中的用户、组和服务主体角色成员身份。 | [appRoleAssignment](../resources/approleassignment.md) | 不适用 |
| **合作伙伴租户管理** | | |
| 获取与客户租户的合作关系的相关信息。 <br/><br/>**注意：** 这仅适用于合作伙伴租户。合作伙伴租户是属于已加入 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 合作伙伴计划的 Microsoft 合作伙伴的 Azure AD 租户。| [合同](../resources/contract.md) | [从云解决方案提供商应用程序中调用 Microsoft Graph](/graph/auth-cloudsolutionprovider) |
| 管理与租户关联的域。借助域操作，注册机构可以对 Microsoft 365 等服务自动执行域关联。 | [domain](../resources/domain.md) | [将自定义域名添加到 Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **租户管理** | | |
| 获取组织的相关信息，如商家地址、技术和通知联系人、订阅的服务计划及其关联域。 | [组织](../resources/organization.md) | 无 |
| 获取公司订阅的服务 SKU 的相关信息。 | [subscribedSku](../resources/subscribedsku.md) | 无 |
| 邀请外部（来宾）用户加入组织。 | [邀请](../resources/invitation.md) | [什么是 Azure AD B2B 协作？](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| 管理组织的登录体验的品牌。 | [organizationalbranding](../resources/organizationalbrandingproperties.md) | [将品牌添加到组织的 Azure Active Directory 登录页面](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)|
| **访问审查** | | |
| 通过访问审查确保组成员身份和应用程序访问权限是正确的。 | [访问审查 API](../resources/accessreviews-root.md) |[Azure AD 访问审查](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
| **许可请求** | | |
| 管理尝试访问需要管理员授权的用户的请求许可请求工作流。  | [许可请求 API](../resources/consentrequests-root.md) |[配置管理员同意工作流](/azure/active-directory/manage-apps/configure-admin-consent-workflow) |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤
目录资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式。若要了解更多：

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/partners)。
