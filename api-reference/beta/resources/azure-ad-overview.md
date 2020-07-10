---
title: 在 Microsoft Graph 中使用 Azure Active Directory 资源
description: Microsoft Graph Azure Active Directory (Azure AD) 提供 REST API，以帮助管理你的组织、资源和资产。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b2d6bff52e7defbf487b0cbe9016dd278591588b
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080868"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Azure Active Directory 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助 Microsoft Graph，用户可以访问 [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) 资源以支持诸多应用场景，如管理管理员（目录）角色，邀请外部用户进入组织，并且，如果你是[云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider)，则可以管理客户的数据。 Microsoft Graph 还提供了应用可使用的方法；例如，用于发现用户的可传递组和角色成员身份的相关信息的方法。

> **Note**: Some Azure AD resources are documented in other sections of the API reference. For more information, see [Users](users.md) and [Groups](group.md).


## <a name="authorization"></a>Authorization

To call the Microsoft Graph APIs on Azure AD resources, your app will need the appropriate permissions. Many of the APIs exposed on Azure AD resources require one of the [_Directory_ permissions](/graph/permissions-reference#directory-permissions). Directory permissions are highly privileged and always require administrator consent.

如果应用要代表用户（委派权限）执行操作，用户可能需要是相应的[管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)的成员，应用才能成功调用许多 Azure AD API。

有关委派权限和应用程序权限等权限的详细信息，请参阅[权限](/graph/permissions-reference)。

## <a name="common-use-cases"></a>常见用例

下表列出了一些 Azure AD 资源的常见用例。

| **用例**        | **REST 资源** | **另请参阅** |
|:-----------------|:--------|:----------|
| ** 对象和方法** | | |
| `directoryObject` is the base class that many directory resources, like users and groups, inherit from. Microsoft Graph exposes several methods that you can use to discover information about users, groups, and other directory objects. For example, you can check for transitive membership in a list of groups, return all the groups and directory roles that a directory object is a transitive member of, or get all the resources of a specified type (like user or group) from a list of generic resource IDs. | [directoryObject](../resources/directoryobject.md) | 不适用 |
| **管理目录（管理员）角色、管理单元、目录设置和策略** | | |
| Activate directory roles in an Azure AD tenant and manage user memberships in directory roles. Directory roles are also known as administrator roles. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[在 Azure Active Directory 中分配管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| 管理管理单元。 目录角色向其成员委派租户机构。 管理员可以创建和管理管理单元，以便向用户更精确地委培具有范围限定的管理机构。 | [administrativeUnit](../resources/administrativeunit.md) | [Azure AD 中的管理单元管理](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| 跨租户应用预定义目录设置或将其应用到单个资源实例。 目前，仅支持 Microsoft 365 组设置。 跨租户应用预定义组设置或将其应用到单个资源实例。组设置控制行为，如组显示名称的禁止使用的词语列表，是否允许来宾用户成为组所有者等。 | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [用于配置组设置的 Azure Active Directory cmdlet](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| 将 Azure AD 策略应用到应用程序、服务主体、组或整个组织。 支持声明映射、令牌颁发、令牌生存期、主页领域发现等策略。  | [可用策略](../resources/policy-overview.md) | 不适用 |
| **保护至 Azure AD 的特权访问** | | |
| 利用 Privileged Identity Management (PIM) 为管理员和 IT 专业人员管理和监控至目录和 Azure 资源的具有时间限定的特权访问。 | [Privileged Identity Management API](../resources/privilegedidentitymanagement-root.md) | [什么是 Azure AD Privileged Identity Management？](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| 监视身份风险事件，如用户从被恶意感染的设备或从不熟悉的位置登录。 | [Identity Protection 服务 API](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Azure Active Directory 风险事件](/azure/active-directory/active-directory-reporting-risk-events) |
| **管理设备** | | |
| Manage devices registered in the organization. Devices are registered to users and include items like laptops, desktops, tablets, and mobile phones. Devices are typically created in the cloud using the Device Registration Service or by Microsoft Intune. They're used by conditional access policies for multifactor authentication. | [设备](../resources/device.md) | [Azure Active Directory 设备注册入门](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[什么是 InTune？](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[在 Intune 中注册设备以进行管理](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **应用管理** | | |
| 管理开发人员租户中的应用配置。 | [应用](../resources/application.md) | [Azure Active Directory 中的应用程序和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| 管理租户中安装的应用。 | [servicePrinicpal](../resources/serviceprincipal.md) | [Azure Active Directory 中的应用程序和服务主体对象](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| 管理租户安装的应用中的用户和管理员许可的权限。 | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | 不适用 |
| 管理租户中安装的应用中的用户、组和服务主体角色成员身份。 | [appRoleAssignment](../resources/approleassignment.md) | 不适用 |
| **合作伙伴租户管理** | | |
| 获取与客户租户的合作关系的相关信息。 <br/><br/>**Note:** This applies to partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of the [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.| [合同](../resources/contract.md) | [从云解决方案提供商应用程序中调用 Microsoft Graph](/graph/auth-cloudsolutionprovider) |
| Manage domains associated with a tenant. Domain operations enable registrars to automate domain association for services such as Microsoft 365. | [domain](../resources/domain.md) | [将自定义域名添加到 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **租户管理** | | |
| 获取组织的相关信息，如商家地址、技术和通知联系人、订阅的服务计划及其关联域。 | [组织](../resources/organization.md) | 无 |
| 获取公司订阅的服务 SKU 的相关信息。 | [subscribedSku](../resources/subscribedsku.md) | 无 |
| 邀请外部（来宾）用户加入组织。 | [邀请](../resources/invitation.md) | [什么是 Azure AD B2B 协作？](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **访问审查** | | |
| 通过访问审查确保组成员关系和应用程序访问权限是正确的 | [访问审查 API](../resources/accessreviews-root.md) |[Azure AD 访问审查](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤
Directory resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph. To learn more:

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

