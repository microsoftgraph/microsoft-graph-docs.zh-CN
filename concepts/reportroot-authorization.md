---
title: 授权API读取Microsoft 365使用报告
description: 可通过 Microsoft Graph 报告 API 访问的报告数据是敏感数据，并受到权限和 Azure Active Directory (Azure AD) 角色的保护。
author: kszb
ms.localizationpriority: high
ms.prod: reports
ms.openlocfilehash: 1710f5c1be640f61c0ff02340e90b991d3d69f9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139021"
---
# <a name="authorization-for-apis-to-read-microsoft-365-usage-reports"></a>授权API读取Microsoft 365使用报告

可通过 Microsoft Graph 报告 API 访问的报告数据是敏感数据。 具体而言，Office 365 使用情况报告由权限和 Azure Active Directory (Azure AD) 角色双重保护。 本文中的信息适用于读取 Microsoft 365 使用报告的报告 API。

读取 Microsoft 365 使用报告的 API 支持两种类型的授权：

- **应用程序级别授权** - 允许应用在没有登录用户的情况下读取所有服务使用情况报告。 授权由授予给应用程序的权限决定。
- **用户委派的授权** - 允许应用代表已登录的用户读取所有服务使用情况报告。 除了向应用授予所需权限之外，用户必须是 Azure AD 受限管理员角色的成员。 这可以是下列角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、Teams 服务管理员、Teams 通信管理员、全局读取者、使用情况摘要报告读取者或报告读取者。 全局读取者角色和使用情况摘要报告读取者角色将只能访问租户级数据，而不能查看详细指标。

如果从 Graph 浏览器调用 API：

- Azure AD 租户管理员必须对 Graph 浏览器应用程序显式授予所请求的权限。
- 对于上面列出的用户委派的授权，该用户必须是 Azure AD 受限管理员角色的成员。

>**注意**：Graph 浏览器不支持应用程序级别授权。

如果从应用程序调用 API：

- Azure AD 租户管理员必须对你的应用程序显式授权。 应用程序级别授权和用户委派的授权都需要满足此要求。
- 如果使用的是用户委派的授权，已登录的用户必须是 Azure AD 受限管理员角色的成员。

## <a name="assign-azure-ad-roles-to-users"></a>向用户分配 Azure AD 角色

应用程序被授予权限后，每个可以访问该应用程序的人（即 Azure AD 租户的成员）都将获得所授予的权限。 为了进一步保护敏感的报告数据，租户管理员必须为应用程序的用户分配相应的 Azure AD 角色。 有关详细信息，请参阅 [Azure Active Directory 中的管理员角色权限](/azure/active-directory/active-directory-assign-admin-roles-azure-portal)和 [为具有 Azure Active Directory 的用户分配管理员和非管理员角色](/azure/active-directory/active-directory-users-assign-role-azure-portal)。

>**注意：** 必须是租户管理员才能执行此步骤。

向用户分配角色：

1. 登录到 [Azure 门户](https://portal.azure.com) (https://portal.azure.com)。
2. 单击左上角的图标以展开 Azure 门户菜单。 选择“**Azure Active Directory**” > “**用户**”。
3. 单击相应用户的姓名。
4. 选择“**分配的角色**”，然后选择“**添加分配**”。
5. 选择适当的角色，并单击“**添加**”。
