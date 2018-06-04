# <a name="azure-ad-identity-and-access-management-api-overview"></a>Azure AD 标识和访问管理 API 概述

Azure Active Directory (Azure AD) 有助于集中化标识和访问管理 (IAM)，实现应用、设备、服务和基础结构之间的安全和高效访问。 组织可以使用 Azure AD 来管理标识，并控制本地、混合及云环境中的访问。  

可以使用 Microsoft Graph 中的 Azure AD REST API 在 Azure AD [资源](../api-reference/v1.0/resources/azure_ad_overview.md)和第三方服务之间创建独特的工作流。

## <a name="why-use-the-azure-ad-apis"></a>为什么使用 Azure AD API？

超过 1,500 万个组织使用 Azure AD，同时订阅 Microsoft 云服务，如 Office 365、Microsoft Azure、企业移动性套件或 Microsoft 365。  

企业开发者使用 Microsoft Graph 集成 Azure AD 标识管理和其他服务，以实现管理工作流的自动化，例如员工入职和离职、个人资料维护、许可证部署等。

对于许多企业开发者来说，Microsoft Graph 和 Azure AD 可帮助将现有应用程序“提升并转移到”云中，从而加速组织的数字化转型。 可以利用 Azure AD 功能向应用程序添加访问控制机制，包括验证用户组成员身份、目录角色或管理单位成员身份。

你可以将 Microsoft Graph 和 Azure AD 用作轻松快速地访问超过 1,500 万个组织的方式，其中包括 90% 已使用 Azure AD 服务的财富 500 强公司。 集成的应用程序具有无缝登录体验，可以使用现有组织数据创建个性化体验。  

你可以使用 Microsoft Graph 中的 Azure AD API 来查询用户配置文件、查找其他用户、管理组织关系、跟踪任务或创建包含现有组织数据的原始解决方案。 这些 API 提供了坚实基础，可将自定义业务应用程序无缝集成到组织现有的数字服务。

### <a name="access-users-and-groups"></a>访问用户和组

可以将 Microsoft Graph 中的 Azure AD API 用于：

- 查找和管理组织中用户的[用户配置文件](../api-reference/v1.0/resources/user.md)信息（例如，姓名、照片、电子邮件地址、职务、办公地点等）。
- 为组织中的项目和团队创建[组](../api-reference/v1.0/resources/groups-overview.md)。 从组中添加和删除成员，以控制对资源的访问权限。 （动态组可根据用户属性值自动更改成员身份。）
- 要控制访问权限，你可以在组列表中检查[可传递成员资格](../api-reference/v1.0/api/user_checkmembergroups.md)，或从[常规资源 ID](../api-reference/v1.0/api/directoryobject_getbyids.md) 列表中获取指定类型的所有资源（如用户或组）。

### <a name="manage-directory-roles"></a>管理目录角色

你可以将用户分配给预定义的 Azure AD 管理[目录角色](../api-reference/v1.0/resources/directoryrole.md)，该角色授予执行特定任务的权限。

### <a name="manage-devices"></a>管理设备

[管理组织中注册的设备](https://docs.microsoft.com/zh-CN/azure/active-directory/device-management-introduction.md)。 设备注册绑定到用户，包括笔记本电脑、台式机、平板电脑和移动电话等。 设备通常是在云中使用 Device Registration Service 或 Microsoft Intune 进行创建。 条件访问策略使用它们进行多重身份验证。

### <a name="partner-tenant-management"></a>合作伙伴租户管理

转售和管理 Microsoft Online Services（如 Office 365、Microsoft Azure 和 CRM Online）的 Microsoft 合作伙伴可以查看他们目前管理的[组织租户](../api-reference/v1.0/resources/contract.md)。

你还可以[管理与租户关联的域](../api-reference/v1.0/resources/domain.md)。 借助域操作，Microsoft 合作伙伴可以对 Office 365 等服务自动执行域注册。

### <a name="tenant-management"></a>租户管理

用于租户管理的 Azure AD API 允许执行以下操作：

- 获取[组织](../api-reference/v1.0/resources/organization.md)的相关信息，如公司办公地址、技术和通知联系人、活动服务预订及其关联域。
- 获取公司订阅的[服务 SKU](../api-reference/v1.0/resources/subscribedsku.md) 的相关信息。
- [邀请外部](../api-reference/v1.0/resources/invitation.md)（来宾）用户加入组织。

### <a name="monitor-identity-protection-risks-preview"></a>监视 Identity Protection 风险（预览版）

你可以检索由 Azure AD [Identity protection](../api-reference/beta/resources/identityprotection_root.md) 生成的风险事件，包括风险事件类型、严重性、日期、时间、位置、受影响的用户等。 Identity Protection 是 Azure AD Premium P2 中提供的功能。

### <a name="activate-users-into-privileged-roles-preview"></a>激活用户成为特权角色（预览）

你可以通过按需激活管理权限来保护对资源的访问权限。 [Privileged Identity Management](../api-reference/beta/resources/privilegedidentitymanagement_root.md) 是 Azure AD Premium P2 中提供的功能。


## <a name="next-steps"></a>后续步骤

- 了解到如何[使用 Azure AD REST API](../api-reference/v1.0/resources/azure_ad_overview.md)。
- 使用 Azure AD 对 Microsoft Graph [进行身份验证](auth_overview.md)。 
- 将 [Azure AD 登录](https://azure.microsoft.com/zh-CN/develop/identity/signin/)集成到应用或网站中。
- 有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。
- 浏览[示例](https://developer.microsoft.com/zh-CN/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
