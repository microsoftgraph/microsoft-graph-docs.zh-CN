# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Azure Active Directory 资源

借助 Microsoft Graph，可以访问 [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) 资源，并使用它们启用多个不同方案。其中包括管理管理员（目录）角色、邀请外部用户加入组织，以及管理客户数据（如果你是[云解决方案提供商 (CSP)](https://partner.microsoft.com/cloud-solution-provider) 的话）。Microsoft Graph 还提供了多个方法可供多种应用使用；例如，用于发现用户的可传递组和角色成员身份的相关信息的方法。 

> **注意**：一些 Azure AD 资源收录在 API 参考的其他部分中。有关详细信息，请参阅[用户](users.md)和[组](group.md)。


## <a name="authorization"></a>授权
 
若要对 Azure AD 资源调用 Microsoft Graph API，应用必须拥有适当的权限。许多已对 Azure AD 资源公开的 API 需要拥有 [_Directory_ 权限](../../../concepts/permissions_reference.md#directory-permissions)之一。_Directory_ 具有很多特权，始终需要征得管理员同意。 

权限分为两种：委派权限和应用程序权限。如果应用是要代表用户调用 API，则需要拥有委派权限。如果应用是要在用户未登录的情况下自行调用 API，则需要拥有应用程序权限。后端服务或守护程序通常需要用到后一种权限。有关委派权限和应用程序权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。 

最后，如果应用要代表用户执行操作，用户可能需要是相应的[管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)的成员，应用才能成功调用许多 Azure AD API。

## <a name="common-use-cases"></a>常见用例 

下表列出了 Azure AD 资源适用的一些常见方案。

| 用例        | REST 资源 | 另请参阅 |
|:---------------|:--------|:----------|
| **目录对象和方法** | | |
| `directoryObject` 是许多目录资源（如用户和组）继承自的基类。Microsoft Graph 公开了多个可用于发现用户、组和其他目录对象的相关信息的方法。例如，可以在组列表中检查可传递成员身份，也可以返回目录对象是其可传递成员的所有组和目录角色，亦可以从常规资源 ID 列表获取指定类型（如用户或组）的所有资源。 | [directoryObject](../resources/directoryobject.md) | 无 |
| **管理目录（管理员）角色** | | |
| 激活 Azure AD 租户中的目录角色，并管理目录角色中的用户成员身份。目录角色亦称为“管理员角色”。 | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | 有关目录（管理员）角色的详细信息，请参阅[在 Azure Active Directory 中分配管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)。 |
| **管理设备** | | |
| 管理组织中的注册设备。设备注册绑定到用户，包括笔记本电脑、台式机、平板电脑和移动电话等。设备通常是在云中使用 Device Registration Service 或 Microsoft Intune 进行创建。条件访问策略使用它们进行多重身份验证。 | [device](../resources/device.md) | 有关 Device Registration Service 的详细信息，请参阅 [Azure Active Directory 设备注册入门](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)。<br/><br/> 有关 Microsoft Intune 的详细信息，请参阅[什么是 InTune？](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)和[在 InTune 中注册设备以进行管理](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune)。 |
| **合作伙伴租户管理** | | |
| 获取与客户租户的合作关系的相关信息。 | [contract](../resources/contract.md) | 仅存在于合作伙伴租户中。合作伙伴租户是属于已加入 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 合作伙伴计划的 Microsoft 合作伙伴的 Azure AD 租户。 <br/><br/>若要详细了解如何以云解决方案提供商身份通过 Microsoft Graph 管理客户数据，请参阅[通过云解决方案提供商应用程序调用 Microsoft Graph](../../../concepts/auth_cloudsolutionprovider.md)。 |
| 管理与租户关联的域。借助域操作，注册机构可以对 Office 365 等服务自动执行域关联。 | [domain](../resources/domain.md) | 有关详细信息，请参阅[将自定义域名添加到 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal)。 |
| **租户管理** | | |
| 获取组织的相关信息，如商家地址、技术和通知联系人、订阅的服务计划及其关联域。 | [organization](../resources/organization.md) | 无 |
| 获取公司订阅的服务 SKU 的相关信息。 | [subscribedSku](../resources/subscribedsku.md) | 无 |
| 邀请外部（来宾）用户加入组织。 | [invitation](../resources/invitation.md) | 有关详细信息，请参阅[什么是 Azure AD B2B 协作？](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)。 |



## <a name="next-steps"></a>后续步骤
目录资源和 API 提供了使用 Microsoft Graph 与用户交互及管理用户体验的新方式： 

- 深入了解对你的方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。


