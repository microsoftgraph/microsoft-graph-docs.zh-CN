# <a name="microsoft-graph-permissions-reference"></a>Microsoft Graph 权限引用 
Microsoft Graph 公开了控制应用程序对资源（如用户、组和邮件）的访问权限的粒度权限。作为开发人员，你可以决定应用程序请求哪些 Microsoft Graph 权限。当用户登录你的应用时，他们或处于某些情况下的管理员可以选择是否同意这些权限。如果用户同意，你的应用可以访问它所请求的资源和 API。对于没有已登录用户的应用，安装应用程序或注册时，管理员可以事先同意权限。 

## <a name="delegated-permissions-application-permissions-and-effective-permissions"></a>委派权限、应用程序权限和有效权限
Microsoft Graph 有两类权限：**委派权限**和**应用权限**。 

- **委派权限**由具有已登录用户的应用使用。对于这些应用，用户或管理员同意应用请求的权限，并向应用委派调用 Microsoft Graph 时代表已登录用户的权限。某些委派权限可以由非管理用户同意，但一些较高特权权限需要管理员同意。  

- **应用程序权限**由无需具有登录用户即可运行的应用使用；例如，作为后台服务或守护程序运行的应用程序。应用程序权限只能由管理员同意。 

_有效权限_是应用在向 Microsoft Graph 发出请求时具有的权限。调用 Microsoft Graph 时，了解授予应用的委派权限及应用程序权限与其有效权限之间的区别非常重要。

- 对于委派权限，应用的_有效权限_将至少是授予应用的委派权限（通过同意）和当前已登录用户的特权之间的特权交集。应用永远不会拥有比已登录用户更多的特权。在组织内，已登录用户的特权可以由策略或一个或多个管理员角色的成员资格确定。有关管理员角色的详细信息，请参阅[在 Azure Active Directory 中分配管理员角色](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles)。<br/><br/>例如，假设已授予应用 _User.ReadWrite.All_ 委派权限。此权限名义上授予应用读取和更新组织中每个用户配置文件的权限。如果已登录的用户是全局管理员，则应用将能够更新组织中每个用户的配置文件。但是，如果已登录的用户不具有管理员角色，则应用将只能更新已登录用户的配置文件。它将无法更新组织中其他用户的配置文件，因为该应用代表用户执行操作的权限中不包括这些权限。
  
- 对于应用程序权限，应用的_有效权限_将是权限默示的完整特权级别。例如，具有 _User.ReadWrite.All_ 应用程序权限的应用可以更新组织中每个用户的配置文件。 

### <a name="microsoft-graph-permission-names"></a>Microsoft Graph 权限名称
Microsoft Graph 权限名称遵循简单模式：_resource.operation.constraint_。例如，_User.Read_ 授予读取已登录用户的配置文件的权限，_User.ReadWrite_ 授予读取和修改已登录用户的配置文件的权限，而 _Mail.Send_ 则授予代表已登录用户发送邮件的权限。 

名称的 _constraint_ 元素决定了你的应用程序在目录中具有的潜在访问范围。Microsoft Graph 当前支持以下约束： 

* **All** 授予应用对目录中指定类型的所有资源执行操作的权限。例如，_User.Read.All_ 可能授予应用读取目录中所有用户的配置文件的特权。 
* **Shared** 授予该应用对其他用户与已登录用户共享的资源执行操作的权限。此约束主要用于 Outlook 资源，如邮件、日历和联系人。例如，_Mail.Read.Shared_ 授予在已登录用户的邮箱中以及组织中的其他用户与已登录用户共享的邮箱中读取邮件的权限。
* **AppFolder** 授予应用在 OneDrive 专用文件夹中读取和写入文件的权限。此约束仅在[文件权限](#files-permissions)上公开，并且仅适用于 Microsoft 帐户。
* 如果未指定**任何约束**，则应用程序仅限于对已登录用户拥有的资源执行操作。例如，_User.Read_ 仅授予读取已登录用户的配置文件的特权，_Mail.Read_ 仅授予读取已登录用户邮箱中的邮件的权限。

> **注意**：在委托场景中，授予应用的有效权限可能受到组织中已登录用户的特权的限制。
> 

### <a name="microsoft-accounts-and-work-or-school-accounts"></a>Microsoft 帐户和工作或学校帐户

并非所有权限都适用于 Microsoft 帐户和工作或学校帐户。你可以检查每个权限组的**备注**，以确定特定权限是否对 Microsoft 帐户和/或工作或学校帐户有效。 

### <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>组织中来宾用户的用户和组搜索限制

用户和组搜索功能允许应用通过对 `/users` 或 `/groups` 资源集（例如 `https://graph.microsoft.com/v1.0/users`）执行查询来搜索组织目录中的任何用户或组。管理员和用户都有此功能；但是，来宾用户用户没有。如果登录用户是来宾用户，应用可以读取特定用户或组的配置文件（例如，`https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`），具体视授予应用的权限而定；不过，不能对可能返回多个资源的 `/users` 或 `/groups` 资源集执行查询。借助授予的适当权限，应用可以读取通过导航属性中的链接获取的用户或组的配置文件；例如，`/users/{id}/directReports` 或 `/groups/{id}/members`。

---

## <a name="calendars-permissions"></a>日历权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    读取用户日历  | 允许应用读取用户日历中的事件。| 否 |
| _Calendars.Read.Shared_ |    读取用户日历和共享日历 | 允许应用读取用户可以访问的所有日历（包括委派日历和共享日历）中的事件。 | 否 |
| _Calendars.ReadWrite_ |    具有对用户日历的完整访问权限  | 允许应用创建、读取、更新和删除用户日历中的事件。 | 否 |
| _Calendars.ReadWrite.Shared_ |    读取和写入用户日历和共享日历 | 允许应用创建、读取、更新和删除用户有权访问的所有日历中的事件。这包括委派日历和共享日历。| 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    读取所有邮箱中的日历  | 允许应用在没有登录用户的情况下读取所有日历的事件。| 是 |
| _Calendars.ReadWrite_ |    读取和写入所有邮箱中的日历 | 允许应用在没有登录用户的情况下创建、读取、更新和删除所有日历的事件。| 是 |

### <a name="remarks"></a>注解

_Calendars.Read.Shared_ 和 _Calendars.ReadWrite.Shared_ 仅适用于工作或学校帐户。所有其他权限对于 Microsoft 帐户和工作或学校帐户均有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委托

* _Calendars.Read_：获取 2017 年 4 月 23 日至 2017 年 4 月 29 日用户日历上的事件 (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`)。
* _Calendars.Read.Shared_：查找所有与会者都均有空参加的会议时间 (`POST /users/{id|userPrincipalName}/findMeetingTimes`)。
* _Calendars.ReadWrite_：将事件添加到用户日历 (`POST /me/events`)。

#### <a name="application"></a>应用程序

* _Calendars.Read_：在由 bob@contoso.com 组织的会议室日历中查找事件 (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`)。
* _Calendars.Read_：列出 5 月份用户日历上的所有事件 (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_：将事件添加到用户的日历以获得批准的空闲时间 (`POST /users/{id | userPrincipalName}/events`)。
* _Calendars.Send_：发送邮件 (`POST /users/{id | userPrincipalName}/sendCalendars`)。


有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="contacts-permissions"></a>联系人权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    读取用户联系人  | 允许应用读取用户联系人。 | 否 |
| _Contacts.Read.Shared_ |    读取用户联系人和共享联系人 | 允许应用读取用户有权访问的联系人，包括用户个人联系人和共享联系人。 | 否 |
| _Contacts.ReadWrite_ |    具有对用户联系人的完整访问权限  | 允许应用创建、读取、更新和删除用户联系人。 | 否 |
| _Contacts.ReadWrite.Shared_ |    读取和写入用户联系人和共享联系人 | 允许应用创建、读取、更新和删除用户有权访问的联系人，包括用户个人联系人和共享联系人。| 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    读取所有邮箱中的联系人 | 允许应用在没有已登录用户的情况下读取所有邮箱中的所有联系人。 | 是 |
| _Contacts.ReadWrite_ |    读取和写入所有邮箱中的联系人  |允许应用在没有登录用户的情况下创建、读取、更新和删除所有邮箱中的全部联系人。| 是 |

### <a name="remarks"></a>注解
仅 _Contacts.Read_ 和 _Contacts.ReadWrite_ 委派权限对 Microsoft 帐户有效。 

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _Contacts.Read_：从已登录用户的顶级联系人文件夹之一读取联系人 (`GET /me/contactfolders/{Id}/contacts/{id}`)。
* _Contacts.ReadWrite_：更新已登录用户的一个联系人的联系人照片 (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。 
* _Contacts.ReadWrite_：将联系人添加到已登录用户的根文件夹 (`POST /me/contacts`)。

#### <a name="application"></a>应用程序

* _Contacts.Read_：从组织中任何用户的顶级联系人文件夹之一读取联系人 (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`)。 
* _Contacts.ReadWrite_：更新组织中任何用户的任何联系人的照片 (`PUT /user/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。 
* _Contacts.ReadWrite_：将联系人添加到组织中任何用户的根文件夹 (`POST /users/{id | userPrincipalName}/contacts`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="device-permissions"></a>设备权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.Read_ | 读取用户设备 | 允许应用代表已登录用户读取用户的设备列表。 | 否 |
| _Device.Command_ | 与用户设备通信 | 允许应用启动其他应用，或代表已登录用户在用户设备上与其他应用进行通信。 | 否 |


#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.ReadWrite.All_ | 读取和写入设备 | 允许应用在没有登录用户的情况下读取和写入所有设备属性。不允许创建设备、删除设备或更新设备备用安全标识符。 | 是 |

### <a name="remarks"></a>注解

_Device.Read_ 和 _Device.Command_ 委派权限仅对个人 Microsoft 帐户有效。

### <a name="example-usage"></a>用法示例
#### <a name="application"></a>应用程序

* _Device.ReadWrite.All_：读取组织中所有已注册的设备 (`GET /devices`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="intune-device-management-permissions"></a>Intune 设备管理权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _DeviceManagementApps.Read.All_ | 读取 Microsoft Intune 应用 | 允许应用读取由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 |
| _DeviceManagementApps.ReadWrite.All_ | 读取和写入 Microsoft Intune 应用 | 允许应用读取和写入由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 |
| _DeviceManagementConfiguration.Read.All_ | 读取 Microsoft Intune 设备配置和策略 | 允许应用读取 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 |
| _DeviceManagementConfiguration.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备配置和策略  | 允许应用读取和写入 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | 在 Microsoft Intune 设备上执行影响用户的远程操作 | 允许应用执行高影响级别远程操作，如在由 Microsoft Intune 管理的设备上擦除设备或重置密码。 | 是 |
| _DeviceManagementManagedDevices.Read.All_ | 读取 Microsoft Intune 设备 | 允许应用读取由 Microsoft Intune 管理的设备的属性。 | 是 |
| _DeviceManagementManagedDevices.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备 | 允许应用读取和写入由 Microsoft Intune 管理的设备的属性。不允许执行具有高影响级别的操作，例如针对设备所有者的远程擦除和密码重置。 | 是 |
| _DeviceManagementRBAC.Read.All_ | 读取 Microsoft Intune RBAC 设置 | 允许应用读取与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 |
| _DeviceManagementRBAC.ReadWrite.All_ | 读取和写入 Microsoft Intune RBAC 设置 | 允许应用读取和写入与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 |
| _DeviceManagementServiceConfig.Read.All_ | 读取 Microsoft Intune 配置 | 允许应用读取 Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 |
| _DeviceManagementServiceConfig.ReadWrite.All_ | 读取和写入 Microsoft Intune 配置 | 允许应用读取和写入 Microsoft Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="remarks"></a>注解
> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

这些权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例
#### <a name="application"></a>应用程序

* _DeviceManagementServiceConfiguration.Read.All_：检查 Intune 订阅的当前状态 (`GET /deviceManagement/subscriptionState`)
* _DeviceManagementServiceConfiguration.ReadWrite.All_：创建新的条款和条件 (`POST /deviceManagement/termsAndConditions`)
* _DeviceManagementConfiguration.Read.All_：查找设备配置状态 (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)
* _DeviceManagementConfiguration.ReadWrite.All_：将设备合规性策略分配给组 (`POST deviceCompliancePolicies/{id}/assign`)
* _DeviceManagementApps.Read.All_：查找发布到 Intune 的所有 Windows 应用商店应用 (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)
* _DeviceManagementApps.ReadWrite.All_：发布新应用程序 (`POST /deviceAppManagement/mobileApps`)
* _DeviceManagementRBAC.Read.All_：按名称查找角色分配 (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)
* _DeviceManagementRBAC.ReadWrite.All_：创建新的自定义角色 (`POST /deviceManagement/roleDefinitions`)
* _DeviceManagementManagedDevices.Read.All_：按名称查找托管的设备 (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)
* _DeviceManagementManagedDevices.ReadWrite.All_：删除托管设备 (`DELETE /managedDevices/{id}`)
* _DeviceManagementManagedDevices.PrivilegedOperations.All_：重置用户的托管设备密码 (`POST /managedDevices/{id}/resetPasscode`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="directory-permissions"></a>目录权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_           |     读取目录数据                     | 允许应用读取组织目录中的数据，如用户、组和应用。 | 是 |
| _Directory.ReadWrite.All_      |     读取和写入目录数据           | 允许应用读取和写入组织目录中的数据，如用户和组。它不允许应用删除用户或组，或重置用户密码。 | 是 |
| _Directory.AccessAsUser.All_   |     以登录用户身份访问目录  | 允许应用以登录用户身份访问目录中的信息。| 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | 读取目录数据 | 允许应用在没有登录用户的情况下读取组织目录中的数据（如用户、组和应用）。 | 是 |
| _Directory.ReadWrite.All_ | 读取和写入目录数据 | 允许应用在没有登录用户的情况下读取和写入组织目录中的数据（如用户和组）。不允许删除用户或组。 | 是 |

### <a name="remarks"></a>注解
Microsoft 帐户不支持目录权限。 

 Directory 权限提供访问目录资源（如组织中的 [User](../api-reference/v1.0/resources/user.md)、[Group](../api-reference/v1.0/resources/group.md) 和 [Device](../api-reference/v1.0/resources/device.md)）的最高级别特权。它们还以独占方式控制对其他目录资源的访问，如[组织联系人](../api-reference/beta/resources/orgcontact.md)、[架构扩展 API](../api-reference/beta/resources/schemaextension.md)、[Privileged Identity Management (PIM) API](../api-reference/beta/resources/privilegedidentitymanagement_root.md)，以及 v1.0 和 beta API 参考文档中的 **Azure Active Directory** 节点下列出的许多资源和 API。其中包括管理单元、目录角色、目录设置、策略等。 

_Directory.ReadWrite.All_ 权限可授予以下特权：

- 完全读取所有目录资源（包括声明属性和导航属性）
- 创建和更新用户
- 禁用和启用用户（而不是公司管理员）
- 设置用户可选安全 ID（而不是管理员）
- 创建和更新组
- 管理组成员
- 更新组所有者
- 管理许可证分配
- 在应用程序上定义架构扩展
- **注意**：无权重置用户密码
- **注意**：无权删除资源（包括用户或组）
- **注意**：特别排除创建或更新以上未列出的资源。这包括：application、oAauth2Permissiongrant、appRoleAssignment、device、servicePrincipal、organization、domains等。
 

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托
* _Directory.Read.All_：列出组织中的所有管理单元 (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_：将成员添加到目录角色 (`POST /directoryRoles/{id}/members/$ref`)

#### <a name="application"></a>应用程序
* _Directory.Read.All_：列出用户的所有成员资格，包括目录角色和管理单元 (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_：列出所有组成员，包括服务主体 (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_：向组中添加所有者 (`POST /groups/{id}/owners/$ref`)


有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="files-permissions"></a>文件权限

#### <a name="delegated-permissions"></a>委派权限

| 权限                  | 显示字符串                                         | 说明                                                                                                                                                                                             | 需经过管理员同意 |
| :-------------------------- | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :--------------------- |
| _Files.Read_                | 读取用户文件                                        | 允许应用读取登录用户的文件。                                                                                                                                                      | 否                     |
| _Files.Read.All_            | 读取用户可以访问的所有文件                    | 允许应用读取登录用户可以访问的所有文件。                                                                                                                                         | 否                     |
| _Files.ReadWrite_           | 具有对用户文件的完全访问权限                         | 允许应用读取、创建、更新和删除登录用户的文件。                                                                                                                          | 否                     |
| _Files.ReadWrite.All_       | 具备对用户可以访问的所有文件的完全访问权限          | 允许应用读取、创建、更新和删除登录用户可以访问的所有文件。                                                                                                             | 否                     |
| _Files.ReadWrite.AppFolder_ | 具有对应用程序文件夹的完全访问权限（预览） | （预览）允许应用读取、创建、更新和删除应用程序文件夹中的文件。                                                                                                         | 否                     |
| _Files.Read.Selected_       | 读取用户选择的文件                       | **Microsoft Graph 提供一定程度的支持（见备注）** <br/> （预览）允许应用读取用户选择的文件。在用户选择文件后，应用有几个小时的访问权限。            | 否                     |
| _Files.ReadWrite.Selected_  | 读取和写入用户选择的文件             | **Microsoft Graph 提供一定程度的支持（见备注）** <br/> （预览）允许应用读取和写入用户选择的文件。在用户选择文件后，应用有几个小时的访问权限。 | 否                     |

#### <a name="application-permissions"></a>应用程序权限

| 权限            | 显示字符串                               | 说明                                                                                                    | 需经过管理员同意 |
| :-------------------- | :------------------------------------------- | :------------------------------------------------------------------------------------------------------------- | :--------------------- |
| _Files.Read.All_      | 读取所有网站集中的文件           | 允许应用在没有登录用户的情况下读取所有网站集中的全部文件。                             | 是                    |
| _Files.ReadWrite.All_ | 读取和写入所有网站集中的文件 | 允许应用在没有登录用户的情况下读取、创建、更新和删除所有网站集中的全部文件。 | 是                    |

### <a name="remarks"></a>注解

Files.Read、Files.ReadWrite、Files.Read.All 和 Files.ReadWrite.All 委派权限在个人 Microsoft 帐户和工作或学校帐户上都有效。请注意，对于个人帐户而言，Files.Read 和 Files.ReadWrite 还授予其权限访问与登录用户共享的文件。 

Files.Read.Selected 和 Files.ReadWrite.Selected 委派权限仅在工作或学校帐户上有效，并仅在处理 [Office 365 文件处理程序 (v1.0)](https://msdn.microsoft.com/office/office365/howto/using-cross-suite-apps) 时才公开。它们不应该用来直接调用 Microsoft Graph API。 

Files.ReadWrite.AppFolder 委派权限仅适于个人帐户，并仅用于访问带有 OneDrive [获取特殊文件夹](../api-reference/v1.0/api/drive_get_specialfolder.md) Microsoft Graph API 的[应用程序根特殊文件夹](https://dev.onedrive.com/misc/appfolder.htm)。


### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _Files.Read_：读取存储在已登录用户的 OneDrive 中的文件 (`GET /me/drive/root/children`)
* _Files.Read.All_：列出与已登录用户共享的文件 (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_：写入已登录用户的 OneDrive 中的文件 (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_：写入与用户共享的文件 (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_：将文件写入 OneDrive 中的应用的文件夹中 (`PUT /me/drive/special/approot/children/file.txt/content`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="group-permissions"></a>组权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ |    读取所有组 | 允许应用代表登录用户列出组，并读取其属性以及所有组成员身份。此外，还允许应用读取登录用户可以访问的所有组的日历、 对话、 文件和其他组内容。 | 是 |
| _Group.ReadWrite.All_ |    读取和写入所有组| 允许应用代表登录用户创建组并读取所有组属性和成员身份。此外，还允许组所有者管理他们的组并允许组成员更新组内容。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | 读取所有组 | 允许应用在没有登录用户的情况下读取所有组的成员。请注意，并非所有组 API 都支持使用仅限应用权限进行访问。有关示例，请参阅[已知问题](../concepts/known_issues.md)。 | 是 |
| _Group.ReadWrite.All_ | 读取和写入所有组 | 允许应用创建组、读取和更新组成员以及删除组。应用可以在没有登录用户的情况下执行所有这些操作。请注意，并非所有组 API 都支持使用仅限应用权限进行访问。有关示例，请参阅[已知问题](../concepts/known_issues.md)。| 是 |


### <a name="remarks"></a>注解

Microsoft 个人帐户不支持组功能。 

对于 Office 365 组，组权限授予应用对组内容的访问权限；例如对话、文件、注释等。 

应用程序权限对受支持的 API 有一些限制。有关详细信息，请参阅[已知问题](../concepts/known_issues.md)。

在某些情况下，应用可能需要[目录权限](#directory-permissions)才能读取 `member` 和 `memberOf` 等组属性。例如，如果组将一个或多个 [servicePrincipals](../api-reference/beta/resources/serviceprincipal.md) 作为成员，则应用将需要有效权限才能通过授予的其中一个_目录\*_权限读取服务主体，否则 Microsoft Graph 将返回错误。（如果是委派权限，已登录用户还需要组织的足够的权限才能读取服务主体。）相同的指导适用于 `memberOf` 属性，该属性可以返回 [administrativeUnits](../api-reference/beta/resources/administrativeunit.md)。

组权限也用于控制对 [Microsoft Planner](../api-reference/beta/resources/planner_overview.md) 资源和 API 的访问权限。Microsoft Planner API 仅支持委派权限，不支持应用程序权限。不支持 Microsoft 个人帐户。


### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _Group.Read.All_：读取已登录用户所属的所有 Office 365 组 (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`)。
* _Group.Read.All_：读取类似对话的所有 Office 365 组内容 (`GET /groups/{id}/conversations`)。
* _Group.ReadWrite.All_：更新组属性，如照片 (`PUT /groups/{id}/photo/$value`)。
* _Group.ReadWrite.All_：更新组成员 (`POST /groups/{id}/members/$ref`)。注意：这还要求 _User.ReadBasic.All_ 读取作为成员添加的用户。

#### <a name="application"></a>应用程序

* _Group.Read.All_：查找名称以“Sales”开头的所有组 (`GET /groups?$filter=startswith(displayName,'Sales')`)。
* _Group.ReadWrite.All_：守护程序服务在 Office 365 组日历上创建新事件 (`POST /groups/{id}/events`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="identity-risk-event-permissions"></a>标识风险事件权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   读取标识风险事件信息  | 允许应用代表登录用户为组织中所有用户读取标识风险事件信息。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   读取标识风险事件信息 | 允许应用无需具有已登录用户即可为组织中所有用户读取标识风险事件信息。 | 是 |


### <a name="remarks"></a>注解

_IdentityRiskEvent.Read.All_ 仅适用于工作或学校帐户。对于通过委派权限读取标识风险信息的应用，登录用户必须是以下管理员角色之一的成员：全局管理员、安全管理员或安全读者。有关管理员角色的详细信息，请参阅[在 Azure Active Directory 中分配管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)

### <a name="example-usage"></a>用法示例
#### <a name="delegated-and-application"></a>委派和应用程序
以下用法对委派权限和应用程序权限均有效：

* 读取为租户中的所有用户所生成的全部风险事件 (`GET /beta/identityRiskEvents`)
* 读取由 Dorknet 僵尸网络所生成的恶意软件风险事件 (`GET /beta/malwareRiskEvents?$filter=malwareName eq 'Dorkbot'`)
* 阅读最新的 50 个风险事件 (`GET /beta/identityRiskEvents?$orderBy=riskEventDateTime desc&top=50`)
 
有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="mail-permissions"></a>邮件权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_ |    读取用户邮件 | 允许应用读取用户邮箱中的电子邮件。 | 否 |
| _Mail.ReadWrite_ |    对用户邮件的读写权限 | 允许应用创建、读取、更新和删除用户邮箱中的电子邮件。不包括发送电子邮件的权限。| 否 |
| _Mail.Read.Shared_ |    读取用户邮件和共享邮件 | 允许应用读取用户可以访问的邮件，包括用户个人邮件和共享邮件。 | 否 |
| _Mail.ReadWrite.Shared_ |    读取和写入用户邮件和共享邮件 | 允许应用创建、读取、更新和删除用户有权访问的邮件，包括用户个人邮件和共享邮件。不包括邮件发送权限。 | 否 |
| _Mail.Send_ |    以用户身份发送邮件 | 允许应用以组织用户身份发送邮件。 | 否 |
| _Mail.Send.Shared_ |    代表他人发送邮件 | 允许应用以登录用户身份发送邮件，包括代表他人发送邮件。 | 否 |
| _MailboxSettings.Read_ |  读取用户的邮箱设置 | 允许应用读取用户的邮箱设置。不包括邮件发送权限。 | 否 |
| _MailboxSettings.ReadWrite_ |  读取和写入用户邮箱设置 | 允许应用创建、读取、更新和删除用户邮箱设置。不包括邮件发送权限。 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_       |    读取所有邮箱中的邮件 | 允许应用在没有登录用户的情况下读取所有邮箱中的邮件。| 是 |
| _Mail.ReadWrite_ |    读取和写入所有邮箱中的邮件 | 允许应用在没有登录用户的情况下创建、读取、更新和删除所有邮箱中的邮件。不包括发送电子邮件的权限。 | 是 |
| _Mail.Send_ |    以任意用户身份发送邮件 | 允许应用在没有登录用户的情况下以任意用户身份发送邮件。 | 是 | 
| _MailboxSettings.Read_ |  读取用户的所有邮箱设置 | 允许应用在没有已登录用户的情况下读取用户邮箱设置。不包括邮件发送权限。 | 否 |
| _MailboxSettings.ReadWrite_ | 读取和写入所有用户邮箱设置  | 允许应用在没有登录用户的情况下创建、读取、更新和删除用户邮箱设置。不包括邮件发送权限。 | 是 |

### <a name="remarks"></a>注解

_Mail.Read.Shared_、_Mail.ReadWrite.Shared_ 和 _Mail.Send.Shared_ 仅适用于工作或学校帐户。所有其他权限对于 Microsoft 帐户和工作或学校帐户均有效。

通过 _Mail.Send_ 或 _Mail.Send.Shared_ 权限，应用可以发送邮件并将副本保存到用户的“已发送邮件”文件夹中，即使应用不使用相应的 _Mail.ReadWrite_ 或 _Mail.ReadWrite.Shared _ 权限也是如此。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委托

* _Mail.Read_：列出用户收件箱中的邮件，按 `receivedDateTime` 排序 (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`)。
* _Mail.Read.Shared_：在已与登录用户共享其收件箱的用户收件箱中查找带有附件的所有邮件 (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`)。
* _Mail.ReadWrite_：标记读取的邮件 (`PATCH /me/messages/{id}`)。
* _Mail.Send_：发送邮件 (`POST /me/sendmail`)。
* _MailboxSettings.ReadWrite_：更新用户的自动答复 (`PATCH /me/mailboxSettings`)。

#### <a name="application"></a>应用程序

* _Mail.Read_：从 bob@contoso.com 查找邮件 (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`)。
* _Mail.ReadWrite_：在名为 `Expense Reports` 的项目中创建一个新的文件夹 (`POST /users/{id | userPrincipalName}/mailfolders`)。
* _Mail.Send_：发送邮件 (`POST /users/{id | userPrincipalName}/sendmail`)。
* _MailboxSettings.Read_：获取用户邮箱的默认时区 (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="member-permissions"></a>成员权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Member.Read.Hidden_ | 读取隐藏成员资格 | 对于已登录用户具有访问权限的隐藏组和管理单元，允许应用代表已登录用户读取隐藏组和管理单元的成员资格。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Member.Read.Hidden_ | 读取所有隐藏成员 | 允许应用在没有登录用户的情况下读取隐藏的组和管理单元中的成员。 | 是 |

### <a name="remarks"></a>注释
_Member.Read.Hidden_ 仅对工作或学校帐户有效。

可以隐藏某些 Office 365 组中的成员资格。这意味着只有该组的成员可以查看其成员。此功能可用于帮助遵守要求组织对外部用户（例如，表示某个班级内注册的学生的 Office 365 组）隐藏组成员身份的规定。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委托

* _Member.Read.Hidden_：代表已登录用户读取隐藏了成员资格的管理单元的成员 (`GET /administrativeUnits/{id}/members`)。
* _Member.Read.Hidden_：代表已登录用户读取隐藏了成员资格的组的成员 (`GET /groups/{id}/members`)。

#### <a name="application"></a>应用程序

* _Member.Read.Hidden_：读取隐藏了成员资格的管理单元的成员 (`GET /administrativeUnits/{id}/members`)。
* _Member.Read.Hidden_：读取隐藏了成员资格的组的成员 (`GET /groups/{id}/members`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="notes-permissions"></a>注释权限
#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read_ |    读取用户 OneNote 笔记本 | 允许应用代表已登录用户读取 OneNote 笔记本和分区标题并创建新的页面、笔记本和分区。 | 否 |
| _Notes.Create_ |    创建用户 OneNote 笔记本 | 允许应用代表已登录用户读取 OneNote 笔记本和分区标题并创建新的页面、笔记本和分区。| 否 |
| _Notes.ReadWrite_ |    读取和写入用户 OneNote 笔记本 | 允许应用代表已登录用户读取、共享和修改 OneNote 笔记本。 | 否 |
| _Notes.Read.All_ |    读取用户可以访问的所有 OneNote 笔记本 | 允许应用读取登录用户在组织中有权访问的 OneNote 笔记本。 | 否 |
| _Notes.ReadWrite.All_ |    读取和写入用户可以访问的所有 OneNote 笔记本。 | 允许应用读取、共享和修改已登录用户在组织中有权访问的 OneNote 笔记本。| 否 |
| _Notes.ReadWrite.CreatedByApp_ |    有限的笔记本访问权限（不推荐使用） | **不推荐使用** <br/>请勿使用。此权限不授予任何特权。 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read.All_ |    读取所有 OneNote 笔记本 | 允许应用无需具有已登录用户即可读取组织中的所有 OneNote 笔记本。 | 是 |
| _Notes.ReadWrite.All_ |    读取和写入所有 OneNote 笔记本 | 允许应用无需具有已登录用户即可读取、共享和修改组织中的所有 OneNote 笔记本。| 是 |


### <a name="remarks"></a>注解
_Notes.Read.All_ 和 _Notes.ReadWrite.All_ 仅适用于工作或学校帐户。所有其他权限对于 Microsoft 帐户和工作或学校帐户均有效。

通过 _Notes.Create_ 权限，应用可以查看已登录用户的 OneNote 笔记本层次结构，并创建 OneNote 内容（笔记本、分区组、分区、页面等）。

_Notes.ReadWrite_ 和 _Notes.ReadWrite.All_ 还允许应用修改针对已登录用户可以访问的 OneNote 内容的权限。 

对于工作或学校帐户，_Notes.Read.All_ 和 _Notes.ReadWrite.All_ 允许该应用访问已登录用户有权限在组织内访问的其他用户的 OneNote 内容。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _Notes.Create_：为登录用户创建新笔记本 (`POST /me/onenote/notebooks`)。
* _Notes.Read_：读取已登录用户的笔记本 (`GET /me/onenote/notebooks`)。
* _Notes.Read.All_：获取已登录用户有权在组织内访问的所有 OneNote 笔记本 (`GET /me/onenote/notebooks?includesharednotebooks=true`)。
* _Notes.ReadWrite_：更新已登录用户的页面 (`PATCH /me/onenote/pages/{id}/$value`)。
* _Notes.ReadWrite.All_：在已登录用户有权在组织内访问的其他用户的笔记本中创建页面 (`POST /users/{id}/onenote/pages`)。

#### <a name="application"></a>应用程序

* _Notes.Read.All_：读取组中的所有用户笔记本 (`GET /groups/{id}/onenote/notebooks`)。
* _Notes.ReadWrite.All_：为组织中任何用户更新笔记本中的页面 (`PATCH /users/{id}/onenote/pages/{id}/$value`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="openid-permissions"></a>OpenID 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _电子邮件_ |    查看用户的电子邮件地址 | 允许应用读取用户的主电子邮件地址。 | 否 |
| _offline_access_ |    随时访问用户数据 | 允许应用读取和更新用户数据，即使用户当前没有在使用此应用，也不例外。| 否 |
| _openid_ |    让用户登录 | 允许用户以其工作或学校帐户登录应用，并允许应用查看用户的基本个人资料信息。| 否 |
| _个人资料_ |    查看用户的基本个人资料 | 允许应用查看用户的基本个人资料（名称、图片、用户名称）。| 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="remarks"></a>注解
可以使用这些权限指定要在 Azure AD 授权和令牌请求中返回的项目。Azure AD v1.0 和 v2.0 终结点以不同的方式支持它们。

使用 Azure AD (v1.0) 终结点时，仅使用 _openid_ 权限。在授权请求的 *scope* 参数中指定它，以在使用 OpenID Connect 协议让用户登录应用时返回 ID 令牌。有关详细信息，请参阅[使用 OpenID Connect 和 Azure Active Directory 来授权访问 Web 应用程序](https://docs.microsoft.com/azure/active-directory/develop/active-directory-protocols-openid-connect-code)。若要成功返回 ID 令牌，还必须确保在注册应用时已配置 _User.Read_ 权限。 

使用 Azure AD v2.0 终结点时，在 _scope_ 参数中指定 _offline\_access_ 权限，以在使用 OAuth 2.0 或 OpenID Connect 协议时显式请求获取刷新令牌。使用 OpenID Connect 时，指定 _openid_ 权限来请求获取 ID 令牌。还可指定 _email_ 权限和/或 _profile_ 权限，以在 ID 令牌中返回其他声明。使用 v2.0 终结点时，无需指定 _User.Read_ 来返回 ID 令牌。有关详细信息，请参阅 [OpenID Connect 作用域](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes)。

> **重要说明**：目前，Microsoft 身份验证库 (MSAL) 默认在授权和令牌请求中指定 _offline\_access_、_openid_、_profile_ 和 _email_。也就是说，在默认情况下，如果显式指定这些权限，Azure AD 可能会返回错误。
>  

---

## <a name="people-permissions"></a>People 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read_ |    读取用户的相关人员列表 | 允许应用读取登录用户相关人员的得分列表。该列表可包括当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。 | 否 |
| _People.Read.All_ | 读取所有用户的相关人员列表 | 允许应用读取登录用户或登录用户组织中的其他用户的相关人员得分列表。该列表可包括当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。此外，还允许应用搜索登录用户组织的整个目录。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read.All_ | 读取所有用户的相关人员列表 | 允许应用读取登录用户或登录用户组织中的其他用户的相关人员得分列表。该列表可包括当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。此外，还允许应用搜索登录用户组织的整个目录。 | 是 |

### <a name="remarks"></a>备注

People.Read.All 权限仅适用于工作和学校帐户。 

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托
* _People.Read_：读取相关人员列表（`GET /me/people`）
* _People.Read.All_：读取同一个组织中的其他用户的相关人员列表（`GET /users('{id})/people`）

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="reports-permissions"></a>报告权限

#### <a name="delegated-permissions"></a>委派权限

无。

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Reports.Read.All_ | 读取所有使用情况报告 | 允许应用在没有登录用户的情况下读取所有服务使用情况报告。提供使用情况报告的服务包括 Office 365 和 Azure Active Directory。 | 是 |

### <a name="remarks"></a>注解
这些报告权限仅对工作或学校帐户有效。 

### <a name="example-usage"></a>用法示例

#### <a name="application"></a>应用程序

* _Reports.Read.All_：读取 7 天的电子邮件应用的使用情况详细信息报告 (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`)
* _Reports.Read.All_：读取日期为“2017-01-01”的电子邮件的活动详细信息报告 (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`)
* _Reports.Read.All_：读取 Office 365 激活详细信息报告 (`GET /reports/Office365Activations(view='Detail')/content`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="sites-permissions"></a>站点权限

#### <a name="delegated-permissions"></a>委派权限

| 权限              | 显示字符串                                                   | 说明                                                                                                                   | 需经过管理员同意 |
| :---------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- | :--------------------- |
| _Sites.Read.All_        | 读取所有网站集中的项目                               | 允许应用代表登录用户读取文档，并列出所有网站集中的项目。                      | 否                     |
| _Sites.ReadWrite.All_   | 读取和写入所有网站集中的项目                     | 允许应用代表登录用户编辑或删除所有网站集中的文档和列表项。            | 否                     |
| _Sites.Manage.All_      | 创建、编辑和删除所有网站集中的项目和列表 | 允许应用代表登录用户管理和创建所有网站集中的列表、文档和列表项。 | 否                     |
| _Sites.FullControl.All_ | 具有对所有网站集的完全控制权限                        | 允许应用代表登录用户具有对所有网站集中的 SharePoint 网站的完全控制权限。              | 是                    |

#### <a name="application-permissions"></a>应用程序权限

| 权限              | 显示字符串                                                   | 说明                                                                                                                   | 需经过管理员同意 |
| :---------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- | :--------------------- |
| _Sites.Read.All_        | 读取所有网站集中的项目                               | 允许应用在没有登录用户的情况下读取所有网站集中的文档和列表项。                             | 是                    |
| _Sites.ReadWrite.All_   | 读取和写入所有网站集中的项目                     | 允许应用在没有登录用户的情况下创建、读取、更新和删除所有网站集中的文档和列表项。 | 是                    |
| _Sites.Manage.All_      | 具有对所有网站集的完全控制权限                        | 允许应用在没有登录用户的情况下管理和创建所有网站集中的列表、文档和列表项。        | 是                    |
| _Sites.FullControl.All_ | 创建、编辑和删除所有网站集中的项目和列表 | 允许应用在没有登录用户的情况下具有对所有网站集中的 SharePoint 网站的完全控制权限。                     | 是                    |


### <a name="remarks"></a>注解

站点权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委托

* _Sites.Read.All_：读取 SharePoint 根网站上的列表 (`GET /v1.0/sites/root/lists`)
* _Sites.ReadWrite.All_：创建 SharePoint 列表中的新列表项 (`POST /v1.0/sites/root/lists/123/items`)
* _Sites.Manage.All_：将新列表添加到 SharePoint 网站 (`POST /v1.0/sites/root/lists`)
* _Sites.FullControl.All_：完整访问 SharePoint 网站和列表。

---

## <a name="tasks-permissions"></a>任务权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Tasks.Read_ | 读取用户任务 | 允许应用读取用户任务。 | 否 |
| _Tasks.Read.Shared_ | 读取用户任务和共享任务 | 允许应用读取用户有权访问的任务，包括用户个人任务和共享任务。 | 否 |
| _Tasks.ReadWrite_ |    创建、读取、更新和删除用户任务和容器 | 允许应用创建、读取、更新和删除分配给已登录用户或与已登录用户共享的任务和容器（以及其中的任务）。| 否 |
| _Tasks.ReadWrite.Shared_ | 读取和写入用户任务和共享任务 | 允许应用创建、读取、更新和删除用户有权访问的任务，包括用户个人任务和共享任务。 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="remarks"></a>注解
_任务_权限用于控制对 Outlook 任务的访问权限。Microsoft Planner 任务的访问权限由[_组_权限](#group-permissions)控制。

目前仅工作或学校帐户支持_共享_权限。即使具有_共享_权限，如果未授予拥有共享内容的用户在文件夹内修改内容访问用户权限，读取和写入仍会失败。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _Tasks.Read_：获取用户邮箱中的所有任务 (`GET /me/outlook/tasks`)。
* _Tasks.Read.Shared_：访问组织中其他用户与你共享的文件夹中的任务 (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`)。
* _Tasks.ReadWrite_：将事件添加到用户的默认任务文件夹 (`POST /me/outook/tasks`)。
* _Tasks.Read_：获取用户邮箱中的所有未完成的任务 (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`)。
* _Tasks.ReadWrite_：更新用户邮箱中的任务 (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`)。
* _Tasks.ReadWrite.Shared_：代表其他用户完成一项任务 (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="user-permissions"></a>用户权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read_       |    登录并读取用户个人资料 | 允许用户登录应用，并允许应用读取登录用户的个人资料。它还允许应用读取登录用户的基本公司信息。| 否 |
| _User.ReadWrite_ |    对用户个人资料的读写权限 | 允许应用读取您的个人资料。此外，它还允许应用代表您更新您的个人资料。 | 否 |
| _User.ReadBasic.All_ |    读取所有用户的基本个人资料 | 允许应用代表登录用户读取组织中其他用户的一套基本个人资料属性。其中包括显示名称、名字和姓氏、电子邮件地址和照片。 | 否 |
| _User.Read.All_  |     读取所有用户的完整个人资料           | 允许应用代表登录用户读取组织中其他用户的整套个人资料属性、下属和经理。 | 是 |
| _User.ReadWrite.All_ |     读取和写入所有用户的完整个人资料 | 允许应用代表登录用户读取和写入组织中其他用户的整套个人资料属性、下属和经理。还允许应用代表已登录用户创建和删除用户以及重置用户密码。 | 是 |
| _User.Invite.All_  |     将来宾用户邀请到组织 | 允许应用代表已登录用户将来宾用户邀请到你的组织。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read.All_ |    读取所有用户的完整个人资料 | 允许应用在没有登录用户的情况下读取组织中其他用户的整套个人资料属性、组成员身份、下属和经理。| 是 |
| _User.ReadWrite.All_ |   读取和写入所有用户的完整个人资料 | 允许应用在没有登录用户的情况下读取和写入组织中其他用户的整套个人资料属性、组成员身份、下属和经理。还允许应用创建和删除非管理用户。不允许重置用户密码。 | 是 |
| _User.Invite.All_  |     将来宾用户邀请到组织 | 允许应用无需具有已登录用户即可将来宾用户邀请到你的组织。 | 是 |

### <a name="remarks"></a>注解

对于 Microsoft 帐户有效的唯一权限是 _User.Read_ 和 _User.ReadWrite_。所有权限对工作或学校帐户均有效。

通过 _User.Read_ 权限，应用还可以通过 [organization](../api-reference/v1.0/resources/organization.md) 资源读取工作或学校帐户的已登录用户的基本公司信息。以下属性可用：ID、displayName 和 verifiedDomains。

对于工作或学校帐户，完整个人资料包括 [User](../api-reference/v1.0/resources/user.md) 资源的所有声明属性。在读取时，默认情况下仅返回有限数量的属性。若要读取不在默认设置中的属性，请使用 `$select`。默认属性包括：

- displayName
- givenName
- jobTitle
- mail
- mobilePhone
- officeLocation
- preferredLanguage
- surname
- userPrincipalName

 _User.ReadWrite_ 和 _User.Readwrite.All_ 委派权限允许应用更新工作或学校帐户的以下配置文件属性：

- aboutMe
- birthday
- hireDate
- interests
- mobilePhone
- mySite
- pastProjects
- photo
- preferredName
- responsibilities
- schools
- skills

通过 _User.ReadWrite.All_ 应用程序权限，应用可更新工作或学校帐户的所有声明属性，但密码除外。

要读取或写入工作或学校帐户的直接下属 (`directReports`) 或经理 (`manager`)，应用必须具有 _User.Read.All_（只读）或 _User.ReadWrite.All_。

_User.ReadBasic.All_ 权限限制应用访问称为基本个人资料的有限属性集。这是因为完整的个人资料可能包含敏感的目录信息。基本个人资料仅包括以下属性： 

- displayName
- givenName
- mail
- photo
- surname
- userPrincipalName

若要读取用户的组成员资格 (`memberOf`)，则应用必须具有 [_Group.Read.All_](#group-permissions) 或 [_Group.ReadWrite.All_](#group-permissions)。但是，如果用户还具有 [directoryRole](../api-reference/v1.0/resources/directoryrole.md) 或 [administrativeUnit](../api-reference/beta/resources/administrativeunit.md) 中的成员资格，则应用还将需要有效权限来读取这些资源，否则 Microsoft Graph 将返回错误。这意味着应用还需要[目录权限](#directory-permissions)，而对于委派权限来说，已登录的用户还需要组织内的足够特权来访问目录角色和管理单元。 

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委托

* _User.Read_：读取已登录用户的完整个人资料 (`GET /me`)。
* _User.ReadWrite_：更新已登录用户的照片 (`PUT /me/photo/$value`)。
* _User.ReadBasic.All_：查找名称以“David”开头的所有用户 (`GET /users?$filter=startswith(displayName,'David')`)。
* _User.Read.All_：读取用户的经理 (`GET /user/{id | userPrincipalName}/manager`)。


#### <a name="application"></a>应用程序

* _User.Read.All_：通过 delta 查询读取所有用户和关系 (`GET /beta/users/delta?$select=displayName,givenName,surname`)。
* _User.ReadWrite.All_：更新组织中任何用户的照片 (`PUT /user/{id | userPrincipalName}/photo/$value`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="permission-scenarios"></a>权限方案

本节介绍一些面向组织中 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md) 资源的常见方案。这些表显示了应用执行方案要求的特定操作所需的权限。请注意，在某些情况下，应用执行特定操作的能力取决于权限是应用程序权限还是委派权限。如果是委派权限，应用的有效权限还将取决于组织内已登录用户的特权。有关详细信息，请参阅[委派权限、应用程序权限和有效权限](#delegated-permissions-application-permissions-and-effective-permissions)。

### <a name="access-scenarios-on-the-user-resource"></a>关于 User 资源的访问方案

| **涉及用户的应用任务**   |  **必需的权限** | **权限字符串** |
|:-------------------------------|:---------------------|:---------------|
| 应用想要读取其他用户的基本信息（仅限显示名称和图片），例如展示人员挑选经验   | _User.ReadBasic.All_  |  读取所有用户的基本个人资料 |
| 应用想要读取已登录用户的完整用户个人资料（请参见直接下属和经理等)     | _User.Read_ | 允许登录和读取用户个人资料|
| 应用想要读取所有用户的完整用户个人资料  | _User.Read.All_ |  读取所有用户的完整个人资料   |
| 应用要读取登录用户的文件、邮件和日历信息  | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | 允许登录和读取用户配置文件、读取用户文件、读取用户邮件、读取用户日历 |
| 应用想要读取登录用户（我）的文件，以及其他用户与登录用户（我）共享的文件。 | _User.Read_, _Files.Read_, _Sites.Read.All_ | 允许登录和读取用户个人资料、读取用户文件、读取所有网站集中的项目 |
| 应用想要读取和写入登录用户的完整用户个人资料   | _User.ReadWrite_ | 对用户个人资料的读写权限 |
| 应用想要读取和写入所有用户的完整用户个人资料    | _User.ReadWrite.All_ | 读取和写入所有用户的完整个人资料 |
| 应用要读取和写入登录用户的文件、邮件和日历信息    | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  对用户个人资料的读写权限、对用户个人资料的读写权限、对用户邮件的读写权限、具有访问用户日历的完整权限 |
   

### <a name="access-scenarios-on-the-group-resource"></a>关于组资源的访问方案
    
| **涉及组的应用任务**  |  **必需的权限** |  **权限字符串** |
|:-------------------------------|:---------------------|:---------------|
| 应用想要读取基本组信息（仅限显示名称和图片），例如展示组挑选经验  | _Group.Read.All_  | 读取所有组|
| 应用想要读取所有 Office 365 组中的全部内容（包括文件、对话）。它还需要显示组成员，同时能够更新组成员（若是所有者）。  |  _Group.Read.All_ | 读取所有网站集中的项、读取所有组|
| 应用想要读取和写入所有 Office 365 组中的全部内容（包括文件、对话）。它还需要显示组成员，同时能够更新组成员（若是所有者）。  |   _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  读取和写入所有组、编辑或删除所有网站集中的项 |
| 应用想要发现（找到）Office 365 组。它允许用户搜索特定组，然后从枚举列表中选择一个组，从而允许用户加入组。     | _Group.ReadWrite.All_ | 读取和写入所有组|
| 应用想要通过 AAD Graph 创建一个组 |   _Group.ReadWrite.All_ | 读取和写入所有组|
