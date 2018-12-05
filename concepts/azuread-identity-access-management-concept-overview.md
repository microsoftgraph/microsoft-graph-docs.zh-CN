---
title: Azure AD 标识和访问管理 API 概述
description: 'Azure Active Directory (Azure AD) 有助于集中化标识和访问管理 (IAM)，实现应用、设备、服务和基础结构之间的安全和高效访问。 组织可以使用 Azure AD 来管理标识，并控制本地、混合及云环境中的访问。  '
ms.openlocfilehash: f933e47f890f228865968d47040fdb1316607692
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156045"
---
# <a name="azure-ad-identity-and-access-management-api-overview"></a>Azure AD 标识和访问管理 API 概述

Azure Active Directory (Azure AD) 有助于集中化标识和访问管理 (IAM)，实现应用、设备、服务和基础结构之间的安全和高效访问。 组织可以使用 Azure AD 来管理标识，并控制本地、混合及云环境中的访问。  

可以使用 Microsoft Graph 中的 Azure AD REST API 在 Azure AD [资源](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0)和第三方服务之间创建独特的工作流。

## <a name="why-use-the-azure-ad-apis"></a>为什么使用 Azure AD API？

超过 1,500 万个组织使用 Azure AD，同时订阅 Microsoft 云服务，如 Office 365、Microsoft Azure、企业移动性套件或 Microsoft 365。  

企业开发者使用 Microsoft Graph 集成 Azure AD 标识管理和其他服务，以实现管理工作流的自动化，例如员工入职和离职、个人资料维护、许可证部署等。

对于许多企业开发者来说，Microsoft Graph 和 Azure AD 可帮助将现有应用程序“提升并转移到”云中，从而加速组织的数字化转型。 可以利用 Azure AD 功能向应用程序添加访问控制机制，包括验证用户组成员身份、目录角色或管理单位成员身份。

你可以将 Microsoft Graph 和 Azure AD 用作轻松快速地访问超过 1,500 万个组织的方式，其中包括 90% 已使用 Azure AD 服务的财富 500 强公司。 集成的应用程序具有无缝登录体验，可以使用现有组织数据创建个性化体验。  

你可以使用 Microsoft Graph 中的 Azure AD API 来查询用户配置文件、查找其他用户、管理组织关系、跟踪任务或创建包含现有组织数据的原始解决方案。 这些 API 提供了坚实基础，可将自定义业务应用程序无缝集成到组织现有的数字服务。

### <a name="access-users-and-groups"></a>访问用户和组

可以将 Microsoft Graph 中的 Azure AD API 用于：

- 查找和管理组织中用户的[用户配置文件](/graph/api/resources/user?view=graph-rest-1.0)信息（例如，姓名、照片、电子邮件地址、职务、办公地点等）。
- 为组织中的项目和团队创建[组](/graph/api/resources/groups-overview?view=graph-rest-1.0)。 从组中添加和删除成员，以控制对资源的访问权限。 （动态组可根据用户属性值自动更改成员身份。）
- 要控制访问权限，你可以在组列表中检查[可传递成员资格](/graph/api/user-checkmembergroups?view=graph-rest-1.0)，或从[常规资源 ID](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) 列表中获取指定类型的所有资源（如用户或组）。

### <a name="manage-directory-roles"></a>管理目录角色

你可以将用户分配给预定义的 Azure AD 管理[目录角色](/graph/api/resources/directoryrole?view=graph-rest-1.0)，该角色授予执行特定任务的权限。

### <a name="manage-devices"></a>管理设备

[管理组织中注册的设备](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction)。 设备注册绑定到用户，包括笔记本电脑、台式机、平板电脑和移动电话等。 设备通常是在云中使用 Device Registration Service 或 Microsoft Intune 进行创建。 条件访问策略使用它们进行多重身份验证。

### <a name="partner-tenant-management"></a>合作伙伴租户管理

转售和管理 Microsoft Online Services（如 Office 365、Microsoft Azure 和 CRM Online）的 Microsoft 合作伙伴可以查看他们目前管理的[组织租户](/graph/api/resources/contract?view=graph-rest-1.0)。

你还可以[管理与租户关联的域](/graph/api/resources/domain?view=graph-rest-1.0)。 借助域操作，Microsoft 合作伙伴可以对 Office 365 等服务自动执行域注册。

### <a name="tenant-management"></a>租户管理

用于租户管理的 Azure AD API 允许执行以下操作：

- 获取[组织](/graph/api/resources/organization?view=graph-rest-1.0)的相关信息，如公司办公地址、技术和通知联系人、活动服务预订及其关联域。
- 获取公司订阅的[服务 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0) 的相关信息。
- [邀请外部](/graph/api/resources/invitation?view=graph-rest-1.0)（来宾）用户加入组织。

### <a name="monitor-identity-risks-preview"></a>监视标识风险 （预览）

大多数安全漏洞都会导致攻击者窃取用户的身份，攻击者利用第三方漏洞、密码喷洒攻击和复杂的网络钓鱼攻击，从而使攻击变得非常有效。 这就意味着，你需要保护所有用户帐户免受这些攻击，并主动防止泄露的身份信息被滥用。

Azure AD 使用自适应机器学习算法和启发式方法来检测异常情况，指示可能会遭到入侵的帐户。 使用此数据，Azure AD 身份保护保护您的用户与基于风险的条件访问策略，并生成报告和其检测上的通知。

目前，Microsoft Graph 使 Azure AD Premium P2 到[检测到的标识保护查询风险事件](/graph/api/resources/identityprotection-root?view=graph-rest-beta)，包括风险事件的类型、 严重性、 日期、 时间、 位置、 受影响的用户等客户能够轻松访问。 然后，客户可以 SIEM 系统和安全应用程序中使用这些事件。

### <a name="activate-users-into-privileged-roles-preview"></a>激活用户成为特权角色（预览）

你可以通过按需激活管理权限来保护对资源的访问权限。 [Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) 是 Azure AD Premium P2 中提供的功能。

### <a name="manage-user-access-reviews-preview"></a>管理用户访问审阅 （预览）

您可以配置访问 reviews （英文） 的组成员身份和应用程序访问。 [Access 会检查](/graph/api/resources/accessreviews-root?view=graph-rest-beta)的功能在 Azure AD Premium P2。

## <a name="api-reference"></a>API 参考

正在寻找此服务的 API 参考？

- [Azure AD 身份和访问管理 API 中 Microsoft Graph v1.0](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0)
- [Azure AD 身份和访问管理 API 中 Microsoft Graph beta](/graph/api/resources/azure-ad-overview?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

- 了解到如何[使用 Azure AD REST API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0)。
- 使用 Azure AD 对 Microsoft Graph [进行身份验证](auth-overview.md)。
- 将 [Azure AD 登录](https://azure.microsoft.com/en-us/develop/identity/signin/)集成到应用或网站中。
- 有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。
- 浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
