---
title: 'Microsoft Graph 权限引用 '
description: Microsoft Graph 公开了控制应用程序对资源（如用户、组和邮件）的访问权限的粒度权限。 作为开发人员，你可以决定应用请求哪些 Microsoft Graph 权限。
author: jackson-woods
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e82902116d9e6abde93dffb9b8c090e8b26a782a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588531"
---
# <a name="microsoft-graph-permissions-reference"></a>Microsoft Graph 权限引用

若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 本主题列出了与每个主要 Microsoft Graph API 集关联的权限。 它还提供有关如何使用权限的指导。

[!INCLUDE [auth-use-least-privileged](../includes/auth-use-least-privileged.md)]

若要详细了解权限的工作原理，请参阅[身份验证和授权基础知识](auth/auth-concepts.md#microsoft-graph-permissions)，并观看以下视频。

> [!VIDEO https://www.youtube-nocookie.com/embed/yXYzgWWVdSM]

## <a name="microsoft-graph-permission-names"></a>Microsoft Graph 权限名称

Microsoft Graph 权限名称遵循简单模式：_resource.operation.constraint_。例如，_User.Read_ 授予读取已登录用户的配置文件的权限，_User.ReadWrite_ 授予读取和修改已登录用户的配置文件的权限，而 _Mail.Send_ 则授予代表已登录用户发送邮件的权限。

名称的 _constraint_ 元素决定了你的应用程序在目录中具有的潜在访问范围。Microsoft Graph 当前支持以下约束：

* **All** 授予应用对目录中指定类型的所有资源执行操作的权限。例如，_User.Read.All_ 可能授予应用读取目录中所有用户的配置文件的特权。
* **Shared** 授予该应用对其他用户与已登录用户共享的资源执行操作的权限。此约束主要用于 Outlook 资源，如邮件、日历和联系人。例如，_Mail.Read.Shared_ 授予在已登录用户的邮箱中以及组织中的其他用户与已登录用户共享的邮箱中读取邮件的权限。
* **AppFolder** 授予应用在 OneDrive 专用文件夹中读取和写入文件的权限。此约束仅在 [文件权限](#files-permissions)上公开，并且仅适用于 Microsoft 帐户。
* 如果未指定 **任何约束**，则应用程序仅限于对已登录用户拥有的资源执行操作。例如，_User.Read_ 仅授予读取已登录用户的配置文件的特权，_Mail.Read_ 仅授予读取已登录用户邮箱中的邮件的权限。

> [!NOTE]
> 在委派方案中，应用的访问权限也受已登录用户的权限限制。 这些权限由用户分配的角色及其与要访问的数据的关系决定。
> 例如，如果登录用户没有查看文件的适当权限，则客户端应用也无法读取该文件，即使向应用授予了 `File.Read.All` 委派权限。

## <a name="microsoft-accounts-and-work-or-school-accounts"></a>Microsoft 帐户和工作或学校帐户

并非所有权限都适用于 Microsoft 帐户和工作或学校帐户。 你可以检查每个权限组的 **支持的 Microsoft 帐户** 列，以确定特定权限是否对 Microsoft 帐户和/或工作或学校帐户有效。

## <a name="limits-on-requested-permissions-per-app"></a>每个应用请求的权限限制

Azure AD 限制客户端应用可以请求和同意的权限数。 这些限制取决于 `signInAudience` 应用的值，如应用清单中所示。 

| signInAudience                     | 允许的用户                                            | 应用可以请求的最大权限   | 应用可以请求的最大 Microsoft Graph 权限   | 单个请求中可同意的最大权限         |
| ---------------------------------- | -------------------------------------------------------- | ----------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------------------- |
| AzureADMyOrg                       | 注册应用的组织中的用户  | 400                                       | 400                                                       | 大约 155 个委派权限和大约 300 个应用程序权限 |
| AzureADMultleOrgs                | 来自任何 Azure AD 组织的用户                     | 400                                       | 400                                                       | 大约 155 个委派权限和大约 300 个应用程序权限 |
| PersonalMicrosoftAccount           | 消费者用户（如 Outlook.com 或 Live.com 帐户）  | 30                                        | 30                                                        | 30                                                                    |
| AzureADandPersonalMicrosoftAccount | 消费者用户和来自任何 Azure AD 组织的用户  | 30                                        | 30                                                        | 30                                                                    |

## <a name="permissions-availability-status"></a>权限可用性状态

[Azure 门户](https://portal.azure.com/)中的 Microsoft Graph 权限通常可用，并且处于 GA 状态，可供所有应用程序使用，除了少数处于预览或个人预览状态的集。 预览中的权限对公众可用；它们可能会更改，并且可能无法升级到 GA 状态。 个人预览状态中的权限不可用，并且永远不会对公众可用。 不要在生产应用中使用预览或个人预览状态中的权限。

## <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>组织中来宾用户的用户和组搜索限制

用户和组搜索功能允许应用对 `/users` 或 `/groups` 资源集(例如 `https://graph.microsoft.com/v1.0/users`)执行查询，以搜索组织目录中的任何用户或组。管理员和用户都具有此功能；但来宾用户没有。

如果登录用户是来宾用户，应用程序可以读取特定用户或组的配置文件（例如，`https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`），具体视应用程序获得的授权而定；不过，不能对可能返回多个资源的 `/users` 或 `/groups` 资源集执行查询。

借助授予的适当权限，应用程序可以读取用户或组的配置文件，具体是通过导航属性中的链接获取；例如，`/users/{id}/directReports` 或 `/groups/{id}/members`。

## <a name="limited-information-returned-for-inaccessible-member-objects"></a>为不可访问的成员对象返回有限的信息

容器对象（例如组）支持各种类型的成员（例如用户和设备）。 当应用程序查询容器对象的成员身份，但无读取特定类型的权限时，将返回该类型的成员，但信息有限。  应用程序将收到 200 响应和一个对象集合。  对于应用程序有权读取的对象类型，返回完整信息。  对于应用程序没有读取权限的对象类型，仅返回对象类型和 ID。

这适用于 [directoryObject](/graph/api/resources/directoryobject)类型的所有关系（而不仅仅是成员链接）。示例包括 `/groups/{id}/members`、`/users/{id}/memberOf` 或 `me/ownedObjects`。

例如，假设一个应用程序具有 Microsoft Graph 的 [User.Read.All](#user-permissions) 和 [Group.Read.All](#group-permissions) 权限。  当前已创建一个组，且该组包含用户、组和设备。  应用程序调用[列出组成员](/graph/api/group-list-members)。  应用程序可以访问组中的用户和组对象，而不能访问设备对象。  在响应中，将返回用户和组对象的所有选定属性。 但是对于设备对象，仅返回有限的信息。  返回内容包括设备的数据类型和对象 ID，但所有其他属性的值均为 *null*。 没有权限的应用将不能使用 ID 获取实际对象。

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members?$select=id,displayName,description,createdDateTime,deletedDateTime,homepage,loginUrl HTTP/1.1
```

以下是 JSON 响应：

```json
{
"@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects(id,displayName,description,createdDateTime,deletedDateTime,homepage,loginUrl)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.user",
            "id":"69d035a3-29c9-469f-809d-d21a4ae69e65",
            "displayName":"Jane Dane",
            "createdDateTime":"2019-09-18T09:06:51Z",
            "deletedDateTime":null
        },
        {
            "@odata.type":"#microsoft.graph.group",
            "id":"c43a7cc9-2d95-44b6-bf6a-6392e41949b4",
            "displayName":"Group 1",
            "description":null,
            "createdDateTime":"2019-10-24T01:34:35Z",
            "deletedDateTime":null
        },
        {
            "@odata.type":"#microsoft.graph.device",
            "id": "d282309e-f91d-43b6-badb-9e68aa4b4fc8",
            "accountEnabled":null,
            "deviceId":null,
            "displayName":null,
            "operatingSystem":null,
            "operatingSystemVersion":null
        }
    ]
}
```

## <a name="access-reviews-permissions"></a>访问评审权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AccessReview.Read.All_ |   读取所有访问评审  | 允许应用代表已登录的用户读取访问评审。 | 是 | 否 |
| _AccessReview.ReadWrite.All_ |   管理所有访问评审  | 允许应用代表已登录的用户读取和写入访问评审。 | 是 | 否 |
| _AccessReview.ReadWrite.Membership_ |   管理组和应用成员身份的访问评审 | 允许应用代表已登录的用户读取和写入组和应用的访问评审。 | 是 | 否 |



#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AccessReview.Read.All_ |   读取所有访问评审 | 允许应用在没有登录的用户的情况下读取访问评审。 | 是 |
| _AccessReview.ReadWrite.All_ |   管理所有访问评审 | 允许应用在没有登录用户的情况下对组织中的访问审查、审阅者、决策和设置执行读取、更新和删除等操作。 | 是 |
| _AccessReview.ReadWrite.Membership_ | 管理组和应用成员身份的访问评审 | 允许应用在没有已登录用户的情况下管理组和应用的访问评审。 | 是 |


### <a name="remarks"></a>备注

_AccessReview.Read.All_、_AccessReview.ReadWrite.All_、_AccessReview.ReadWrite.Membership_ 仅对于工作或学校帐户有效。

对于通过委派权限读取组或应用的访问评审的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员、安全管理员、安全读取者或用户管理员。 对于通过委派权限读取组或应用的访问评审的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员或用户管理员。

对于通过委派权限读取 Azure AD 角色的访问评审的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员、安全管理员、安全读取者或特权角色管理员。 对于通过委派权限写入 Azure AD 角色的访问评审的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员或特权角色管理员。

若要详细了解管理员角色，请参阅[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

---

## <a name="administrative-units-permissions"></a>管理单元权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AdministrativeUnit.Read.All_ |   读取管理单元  | 允许应用代表已登录的用户读取管理单元和管理单元成员身份。 | 是 | 否 |
| _AdministrativeUnit.ReadWrite.All_ |   读取和写入管理单元  | 允许应用代表已登录的用户创建、读取、更新和删除管理单元并管理管理单元成员身份。 | 是 | 否 |


#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AdministrativeUnit.Read.All_ |   读取所有管理单元 | 允许应用在没有登录用户的情况下读取管理单元和管理单元成员身份。 | 是 |
| _AdministrativeUnit.ReadWrite.All_ |   读取和写入所有管理单元 | 允许应用在没有登录用户的情况下创建、读取、更新和删除管理单元并管理管理单元成员身份。 | 是 |

### <a name="remarks"></a>说明
使用 _AdministrativeUnit.Read.All_ 权限，应用程序可以读取包括成员在内的管理单元信息。

使用 _AdministrativeUnit.ReadWrite.All_ 权限，应用程序可以创建、读取、更新和删除包括成员在内的管理单元信息。

_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_ 仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

> [!NOTE]
> 管理单元 API 的 `v1.0`终结点`/v1.0/directory/administrativeUnits`。

- _AdministrativeUnit.Read.All_：读取管理单元 (`GET /beta/administrativeUnits`)
- _AdministrativeUnit.Read.All_：读取管理单元成员列表 (`GET /beta/administrativeUnits/<id>/members`)
- _AdministrativeUnit.ReadWrite.All_：创建管理单元 (`POST /beta/administrativeUnits`)
- _AdministrativeUnit.ReadWrite.All_：更新管理单元 (`PATCH /beta/administrativeUnits/<id>`)
- _AdministrativeUnit.ReadWrite.All_：将成员添加到管理单元 (`POST /beta/administrativeUnits/<id>/members`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="analytics-resource-permissions"></a>分析资源权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Analytics.Read_ |   读取用户活动统计信息。 | 允许应用读取已登录用户的活动统计消息，例如该用户在电子邮件、会议或聊天会话中花费的时间。 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>Delegated

* _Analytics.Read_：[列出用户的相关设置](/graph/api/useranalytics-get-settings?view=graph-rest-beta&preserve-view=true) (`GET /beta/me/analytics/settings`)

#### <a name="application"></a>应用程序

无。

---

## <a name="appcatalog-resource-permissions"></a>AppCatalog 资源权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 需要 Microsoft 帐户 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------| :----------|
| _AppCatalog.Read.All_ | 读取所有应用目录 | 允许应用读取应用目录中的应用。| 否 | 否 |
| _AppCatalog.ReadWrite.All_ | 读取和写入所有应用目录  | 允许应用在应用目录中创建、读取、更新和删除应用。 | 是 | 否 |
|_AppCatalog.Submit_|提交应用以供管理员审查|允许用户提交应用供管理员审查，以便发布在组织的应用目录中，并允许用户取消尚未发布的过去提交。</br> &#119821;&#119822;&#119827;&#119812;：非管理员用户通过添加 `requiresReview=true` 查询参数来提交应用以供审核。|是|否|

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _AppCatalog.Read.All_ | 读取所有应用目录 | 允许应用在没有登录用户的情况下读取应用目录中的应用。 | 是 |
| _AppCatalog.ReadWrite.All_ | 读取和写入所有应用目录 | 允许应用在没有登录用户的情况下在应用目录中创建、读取、更新和删除应用。 | 是 |

### <a name="remarks"></a>注解

当前的唯一目录是 [Microsoft Teams](teams-concept-overview.md) 中的应用程序列表。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派
* _AppCatalog.ReadWrite.All_：[：列出目录中的所有应用程序](/graph/api/appcatalogs-list-teamsapps) (`GET /beta/appCatalogs/teamsApps`)
* _AppCatalog.ReadWrite.All_：[发布一个应用](/graph/api/teamsapp-publish?view=graph-rest-beta&preserve-view=true) (`POST /beta/appCatalogs/teamsApps`)
* _AppCatalog.ReadWrite.All_：[更新某个已发布的应用](/graph/api/teamsapp-update?view=graph-rest-beta&preserve-view=true) (`PATCH /beta/appCatalogs/teamsApps/{id}`)
* _AppCatalog.ReadWrite.All_：[删除某个已发布的应用](/graph/api/teamsapp-delete?view=graph-rest-beta&preserve-view=true) (`DELETE /beta/appCatalogs/teamsApps/{id}`)

#### <a name="application"></a>应用程序

无。

---

## <a name="application-resource-permissions"></a>应用程序资源权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Application.Read.All_ | 读取应用程序 | 允许此应用代表已登录的用户读取应用程序和服务主体。 | 是 |
| _Application.ReadWrite.All_ | 读取和写入所有应用 |  允许此应用代表已登录的用户创建、读取、更新和删除应用程序和服务主体。 | 是 |
| _AppRoleAssignment.ReadWrite.All_ | 管理应用权限授予和应用角色分配 | 允许应用代表已登录用户管理任何 API（包括 Microsoft Graph）的应用程序权限授予和任何应用的应用程序分配。 | 是 |
| _DelegatedPermissionGrant.ReadWrite.All_ | 管理委派权限授予 | 允许应用代表已登录用户管理任何 API（包括 Microsoft Graph）委托的权限授予。 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Application.Read.All_ | 读取应用程序 | 允许此应用在没有登录用户的情况下读取应用程序和服务主体。 | 是 |
| _Application.ReadWrite.All_ | 读取和写入所有应用 | 允许调用应用在没有登录用户的情况下创建和管理（读取、更新、更新应用程序密码和删除）应用程序和服务主体。  不允许管理对用户或组的同意授权或应用程序分配。 | 是 |
| _Application.ReadWrite.OwnedBy_ | 管理此应用创建或拥有的应用 | 允许调用应用在没有登录用户的情况下创建其他应用程序和服务主体，以及完全管理这些应用程序和服务主体（读取、更新、更新应用程序密码和删除）。  它无法更新任何不是其所有者的应用程序。 不允许管理对用户或组的同意授权或应用程序分配。 | 是 |
| _AppRoleAssignment.ReadWrite.All_ | 管理应用权限授予和应用角色分配 | 允许应用在没有登录用户的情况下管理任何 API（包括 Microsoft Graph）的应用程序权限授予和任何应用的应用程序分配。 | 是 |
| _DelegatedPermissionGrant.ReadWrite.All_ | 管理所有委托的权限授予 | 允许应用在没有已登录用户的情况下，授予或吊销任何 API（包括 Microsoft Graph）委托的权限。 | 是 |

### <a name="remarks"></a>说明

> [!CAUTION]
> 允许授予授权的权限（如 _AppRoleAssignment.ReadWrite.All_）允许应用程序向自身、其他应用程序或任何用户授予其他权限。 同样，允许管理凭据的权限（如 _Application.ReadWrite.All_）允许应用程序充当其他实体，并使用已授予的权限。 授予此类权限时要谨慎。

_Application.ReadWrite.OwnedBy_ 权限允许与 _Application.ReadWrite.All_ 相同的操作，只不过前者只允许对调用应用充当所有者的应用程序和服务主体执行这些操作。所有权由目标 [应用](/graph/api/application-list-owners?view=graph-rest-beta&preserve-view=true)或 [服务主体](/graph/api/serviceprincipal-list-owners?view=graph-rest-beta&preserve-view=true)资源上的`owners`导航属性指示。
> 注意：使用 _Application.Read Write.Owned by_ 权限调用 `GET /applications` 以列出应用程序将失败，并显示 403。  请改为使用 `GET servicePrincipals/{id}/ownedObjects` 列出调用应用程序充当所有者的应用程序。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Application.Read.All_：列出所有应用程序 (`GET /v1.0/applications`)
* _Application.ReadWrite.All_：更新服务主体 (`PATCH /v1.0/servicePrincipals/{id}`)

#### <a name="application"></a>应用程序

* _Application.Read.All_：列出所有应用程序 (`GET /v1.0/applications`)
* _Application.ReadWrite.All_：删除服务主体 (`DELETE /v1.0/servicePrincipals/{id}`)
* _Application.ReadWrite.OwnedBy_：创建应用程序 (`POST /v1.0/applications`)
* _Application.ReadWrite.OwnedBy_：列出调用应用程序拥有的所有应用程序 (`GET /v1.0/servicePrincipals/{id}/ownedObjects`)
* _Application.ReadWrite.OwnedBy_：向拥有的应用程序添加另一个所有者 (`POST /v1.0/applications/{id}/owners/$ref`)。
    > 注意：这可能需要其他权限。

---

## <a name="audit-log-permissions"></a>审核日志权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _AuditLog.Read.All_ | 读取审核日志数据 | 允许应用代表已登录用户读取和查询你的审核日志活动。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_AuditLog.Read.All_ |读取所有审核日志数据 |允许应用在没有登录用户的情况下读取和查询你的审核日志活动。 |是 |

---

## <a name="bitlocker-recovery-key-permissions"></a>BitLocker 恢复密钥权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _BitlockerKey.ReadBasic.All_ | 读取基本 BitLocker 密钥信息 | 允许应用读取租户中所有设备的 BitLocker 密钥属性。不返回恢复密钥。 | 是 | 否 |
| _BitlockerKey.Read.All_ | 读取 BitLocker 密钥 | 允许应用读取租户中所有设备的 BitLocker 密钥。将返回恢复密钥。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _BitlockerKey.ReadBasic.All_：列出租户中所有设备的 BitLocker 恢复密钥，而不返回 'key' 属性 (`GET /bitlocker/recoveryKeys`)。
* _BitlockerKey.Read.All_：通过恢复密钥 (`GET /bitlocker/recoveryKeys/{bitlockerRecoveryKeyId}?$select=key`) 获取 BitLocker 恢复密钥

---

## <a name="bookings-permissions"></a>预订权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Bookings.Read.All_ |  允许应用代表登录用户读取预订约会、业务、客户、服务和员工。 | 适用于只读应用程序。典型的目标用户是预定业务的客户。 | 否 | 否 |
| _BookingsAppointment.ReadWrite.All_ | 允许应用代表登录用户读取和写入预订约会和客户，此外，还允许读取业务、服务和员工。 | 适用于需要操作约会和客户的安排日程的应用程序。 无法更改有关预订业务的基本信息及其服务和员工成员。 典型目标用户是某预订业务的客户。| 否 | 否 |
| _Bookings.ReadWrite.All_ | 允许应用代表登录用户读取和编写预订约会、业务、客户、服务和员工。 不允许创建、删除或发布预订业务。 | 适用于操纵现有业务、其服务和员工成员的管理应用程序。 无法创建、删除或更改预订业务的发布状态。 典型目标用户是组织的支持人员。| 否 | 否 |
| _Bookings.Manage.All_ | 允许应用代表登录用户读取、编写和管理预订约会、业务、客户、服务和员工。  | 允许应用具有完全访问权限。 <br>适用于完全管理体验。 典型目标用户是组织的管理员。| 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Bookings.Read.All_：获取为租户创建的预订业务集合的 ID 和名称 (`GET /bookingBusinesses`)。
* _BookingsAppointment.ReadWrite.All_：为预订业务中的服务创建约会 (`POST /bookingBusinesses/{id}/appointments`)。
* _Bookings.ReadWrite.All_：为指定的预订业务创建新服务 (`POST /bookingBusinesses/{id}/services`)。
* _Bookings.Manage.All_：使此业务的日程安排页对外部客户可用 (`POST /bookingBusinesses/{id}/publish`)。

## <a name="calendars-permissions"></a>日历权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Calendars.Read_ |读取用户日历 |允许应用读取用户日历中的事件。 |否 | 是 |
| _Calendars.Read.Shared_ |读取用户日历和共享日历 |允许应用读取用户可以访问的所有日历（包括委派日历和共享日历）中的事件。 |否 | 否 |
| _Calendars.ReadWrite_ |具有对用户日历的完整访问权限 |允许应用创建、读取、更新和删除用户日历中的事件。 |否 | 是 |
| _Calendars.ReadWrite.Shared_ |读取和写入用户日历和共享日历 |允许应用创建、读取、更新和删除用户有权访问的所有日历中的事件。这包括委派日历和共享日历。|否 | 否 |

<br/>

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Calendars.Read_ |读取所有邮箱中的日历 |允许应用在没有登录用户的情况下读取所有日历的事件。 |是 |
|_Calendars.ReadWrite_ |读取和写入所有邮箱中的日历 |允许应用在没有登录用户的情况下创建、读取、更新和删除所有日历的事件。 |是 |

> **重要说明** 管理员可以配置 [应用程序访问策略](auth-limit-mailbox-access.md)，以限制应用程序访问 _特定_ 邮箱，而不是组织中的所有邮箱，即使该应用程序已被授予 Calendars.Read 或Calendars.ReadWrite 的应用程序权限。
<br/>

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Calendars.Read_：获取从 2017 年 4 月 23 日到 2017 年 4 月 29 日用户日历中的事件 (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`)。
* _Calendars.Read.Shared_：查找所有与会者都均有空参加的会议时间 (`POST /users/{id|userPrincipalName}/findMeetingTimes`)。
* _Calendars.ReadWrite_：将事件添加到用户日历 (`POST /me/events`)。

#### <a name="application"></a>应用程序

* _Calendars.Read_：在 bob@contoso.com 组织整理的会议室日历中查找事件 (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`)。
* _Calendars.Read_：列出 5 月份用户日历上的所有事件 (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_：将获准休假事件添加到用户日历 (`POST /users/{id | userPrincipalName}/events`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

## <a name="calls-permissions"></a>通话权限

#### <a name="delegated-permissions"></a>委派权限

无。

<br/>

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Calls.Initiate.All_|从应用发起一对一拨出通话（预览版）|允许应用在没有登录用户的情况下，向单个用户发起播出通话并将通话转接到组织目录中的用户。|是|
|_Calls.InitiateGroupCall.All_|从应用发起组拨出通话（预览版）|允许应用在没有登录用户的情况下，向多个用户发起播出通话并向组织中的会议添加参与者。|是|
|_Calls.JoinGroupCall.All_|作为应用加入组通话和会议（预览版）|允许应用在没有登录用户的情况下，加入组织中的组通话和计划会议。 应用将加入到租户的会议中并获得目录用户特权。|是|
|_Calls.JoinGroupCallasGuest.All_|作为来宾加入组通话和会议（预览版）|允许应用在没有登录用户的情况下，以匿名方式加入组织中的组通话和计划会议。 应用将作为来宾加入租户的会议。|是|
|_Calls.AccessMedia.All_\*|作为应用访问通话中的媒体数据流（预览版）|允许应用在没有登录用户的情况下，直接访问通话中的媒体数据流。|是|

> \***重要说明：** 不得使用云通信 API 进行记录，否则保留来自应用程序访问的通话或会议的媒体内容，或派生自该媒体内容的数据。 请确保你遵守有关通信的数据保护和机密性方面的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

<br/>

### <a name="example-usage"></a>用法示例

#### <a name="application"></a>应用程序

* _Calls.Initiate.All_：从应用程序向组织中的某个用户发起对等通话 (`POST /beta/communications/calls`)。
* _Calls.InitiateGroupCall.All_：从应用程序向组织中的一组用户发起组通话 (`POST /beta/communications/calls`)。
* _Calls.JoinGroupCall.All_：从应用程序加入组通话或联机会议 (`POST /beta/communications/calls`)。
* _Calls.JoinGroupCallasGuest.All_：从应用程序加入组通话或联机会议，但应用程序在会议中仅具有来宾特权 (`POST /beta/communications/calls`)。
* _Calls.AccessMedia.All_：创建或加入某个通话，且应用将能够直接访问该通话中的参与者媒体数据流 (`POST /beta/communications/calls`)。

> **注意：** 有关请求示例，请参阅 [创建通话](/graph/api/application-post-calls?view=graph-rest-beta&preserve-view=true)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

## <a name="call-records-permissions"></a>通话记录权限

#### <a name="delegated-permissions"></a>委派权限

无。

<br/>

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_CallRecords.Read.All_|读取所有通话记录|允许应用在没有用户登录的情况下读取所有通话和联机会议的通话记录。|是|
|_CallRecord-PstnCalls.Read.All_|读取 PSTN 并直接路由呼叫日志数据|在没有已登录用户的情况下，允许应用读取所有 PSTN 和直接路由通话日志数据。|是|

### <a name="remarks"></a>备注

_CallRecords.Read.All_ 权限为组织内每次通话和联机会议（包括与外部电话号码的通话）授权 [callRecords](/graph/api/resources/callrecords-callrecord) 的特权访问。 这包括与参与呼叫的人员有关的潜在敏感详细信息，以及与这些通话和会议相关的、可用于网络疑难解答的技术信息（IP地址、设备详细信息和其他网络信息）。

_CallRecord-PstnCalls.Read.All_ 权限授予应用程序访问 [PSTN（通话套餐）](/graph/api/callrecords-callrecord-getpstncalls)和 [直接路由](/graph/api/callrecords-callrecord-getdirectroutingcalls)呼叫日志的权限。 这包括与用户相关的潜在敏感信息以及与外部电话号码的通话。

> **重要说明：** 应谨慎为应用程序授予这些权限。 通话记录可提供业务运营的见解，因此可能成为恶意参与者的目标。 仅为你信任的应用程序授予这些权限，以满足你的数据保护要求。

> **重要说明：** 请确保你遵守有关通信的数据保护和机密性方面的法律和法规。 有关详细信息，请参阅[使用条款](/legal/microsoft-apis/terms-of-use)并咨询法律顾问。

<br/>

### <a name="example-usage"></a>用法示例

#### <a name="application"></a>应用程序

* _CallRecords.Read.All_：检索通话记录 (`GET /v1.0/communications/callRecords/{id}`)。
* _CallRecords.Read.All_：订阅新的通话记录 (`POST /v1.0/subscriptions`)。
* _CallRecords.Read.All_：检索指定时间范围 (`GET /v1.0/communications/callRecords/microsoft.graph.callRecords.getDirectRoutingCalls(fromDateTime={start date and time),toDateTime={end date and time))`) 内的直接路由通话记录。
* _CallRecord-PstnCalls.Read.All_：检索指定时间范围 (`GET /v1.0/communications/callRecords/microsoft.graph.callRecords.getPstnCalls(fromDateTime={start date and time),toDateTime={end date and time))`) 内的 PSTN 通话记录

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

## <a name="channel-permissions"></a>频道权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Channel.ReadBasic.All_ | 读取频道名称和说明。 | 代表已登录用户读取频道名称和频道说明。    | 否 | 否 |
| _Channel.Create_ | 创建频道。 | 代表已登录用户在任何团队中创建频道。   | 是 | 否 |
| _Channel.Delete.All_ | 删除频道。 | 代表已登录用户删除任何团队中的频道。   | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Channel.ReadBasic.All_ | 读取所有频道的名称和说明。 | 在没有登录用户的情况下读取所有频道名称和说明。  | 是 | 否 |
| _Channel.Create_ | 创建频道。 | 在没有登录用户的情况下在任何团队中创建频道。  | 是 | 否 |
| _Channel.Delete.All_ | 删除频道。 | 在没有登录用户的情况下删除任何团队中的频道。  | 是 | 否 |
|_团队合作。迁移。所有_|管理迁移到 Microsoft Teams|创建和管理用于迁移到 Microsoft Teams 的资源|是|是|

## <a name="channel-member-permissions"></a>频道成员权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMember.Read.All_  |读取频道的成员。 |代表已登录的用户读取频道的成员。 |是 | 否 |
|_ChannelMember.ReadWrite.All_ | 从频道中添加和删除成员。| 代表已登录用户从频道中添加和删除成员。 还允许更改成员的角色，例如从所有者到非所有者。| 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMember.Read.All_ |读取所有频道的成员。 |在没有用户登录的情况下读取所有频道的成员。 |是 | 否 |
|_ChannelMember.ReadWrite.All_ |从所有频道中添加和删除成员。|在没有用户登录的情况下从所有频道中添加和删除成员。 还允许更改成员的角色，例如从所有者到非所有者。| 是 | 否 |

## <a name="channel-message-permissions"></a>频道消息权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMessage.Edit_ （个人预览版）|编辑用户的频道消息 |允许应用代表已登录的用户在 Microsoft Teams 中编辑频道消息。 |是 | 否 |
|_ChannelMessage.Read.All_ |读取用户频道消息  |允许应用代表已登录的用户在 Microsoft Teams 中读取频道消息。 |是 | 否 |
|_ChannelMessage.Send_ |发送频道消息 |允许应用代表已登录的用户在 Microsoft Teams 中发送频道消息。 |否| 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ChannelMessage.Read.All_ |读取所有频道消息  |允许应用在没有登录的用户的情况下读取 Microsoft Teams 中的频道消息。 |是 | 否 |
|_ChannelMessage.UpdatePolicyViolation.All_ |标记违反策略的频道消息 |允许应用更新 Microsoft Teams 频道消息，方法是通过修补数据丢失保护 (DLP) 策略违反属性集来处理 DLP 处理的输出。 | 是 | 否 |

> **注意：** 另请参阅 [Group.Read.All](#group-permissions)。

## <a name="channel-settings-permissions"></a>频道设置权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChannelSettings.Read.All_ | 读取频道的名称、说明和设置。 | 代表已登录用户读取所有频道名称、频道说明和频道设置。| 是 | 否 |
| _ChannelSettings.ReadWrite.All_ | 读取和写入频道的名称、说明和设置。 | 代表已登录用户读取和写入所有频道的名称、说明和设置。| 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChannelSettings.Read.All_ | 读取所有频道的名称、说明和设置。 | 在没有登录用户的情况下读取所有频道名称、频道说明和频道设置。| 是 | 否 |
| _ChannelSettings.ReadWrite.All_ | 读取和写入所有频道的名称、说明和设置。 | 在没有登录用户的情况下读取和写入所有频道的名称、说明和设置。| 是 | 否 |

## <a name="chat-permissions"></a>聊天权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Chat.Read_ |读取聊天消息  |允许应用代表你读取 Microsoft Teams 中的一对一或群组聊天消息。 |否 | 否 |
|_Chat.ReadBasic_ |读取用户聊天线程的名称和成员  |允许应用代表已登录用户读取一对一以及群组聊天线程的成员和说明。 |否 | 否 |
|_Chat.ReadWrite_ |读取聊天消息并发送新消息  |允许应用代表你在 Microsoft Teams 中读取并发送一对一或群组聊天消息。 |否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Chat.Read.All_ |读取所有聊天消息  |允许应用在没有登录的用户的情况下读取 Microsoft Teams 中的一对一或群组聊天消息。 |是 | 否 |
|_Chat.ReadBasic.All_ |读取用户聊天线程的名称和成员  |读取所有聊天线程的名称和成员。 |是 | 否 |
|_Chat.UpdatePolicyViolation.All_ |标记违反策略的聊天消息 |允许应用更新 Microsoft Teams 一对一聊天或群组聊天消息，方法是通过修补数据丢失保护 (DLP) 策略违反属性集来处理 DLP 处理的输出。 | 是 | 否 |

> **注意：** 对于频道中的消息，请参阅 [ChannelMessage 权限](#channel-message-permissions)。

## <a name="chat-resource-specific-consent-permissions"></a>聊天资源特定的同意权限

#### <a name="application-permissions"></a>应用程序权限

| 权限                     | 显示字符串                                                | 说明  | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:-------------------------------|:--------------------------------------------------------------|:-------------|:-----------------------|:----------------------------|
| _ChatSettings.Read.Chat_         | 读取此聊天的设置。                                    | 允许应用在没有登录用户的情况下读取此聊天的设置。 |否 | 否 |
| _ChatSettings.ReadWrite.Chat_    | 读取和写入此聊天的设置。                          | 允许应用在没有登录用户的情况下读取和写入此聊天的设置。 |否 | 否 |
| _ChatMessage.Read.Chat_          | 读取此聊天的消息。                                    | 允许应用在没有登录用户的情况下读取此聊天的消息。 |否 | 否 |
| _ChatMember.Read.Chat_           | 读取此聊天的成员。                                     | 允许应用在没有登录用户的情况下读取此聊天的成员。 |否 | 否 |
| _Chat.Manage.Chat_               | 管理此聊天。                                             | 允许应用在没有登录用户的情况下管理聊天、聊天成员并授予对聊天数据的访问权限。  |否 | 否 |
| _TeamsTab.Read.Chat_             | 读取此聊天的选项卡。                                        | 允许应用在没有登录用户的情况下读取此聊天的选项卡。 |否 | 否 |
| _TeamsTab.Create.Chat_           | 在此聊天中创建选项卡。                                     | 允许应用在没有登录用户的情况下在此聊天中创建选项卡。 |否 | 否 |
| _TeamsTab.Delete.Chat_           | 删除此聊天的选项卡。                                      | 允许应用在没有登录用户的情况下删除此聊天的选项卡。 |否 | 否 |
| _TeamsTab.ReadWrite.Chat_        | 管理此聊天的选项卡。                                      | 允许应用在没有登录用户的情况下管理此聊天的选项卡。 |否 | 否 |
| _TeamsAppInstallation.Read.Chat_ | 读取此聊天中安装了哪些应用。                   | 允许应用在没有登录用户的情况下读取此聊天中安装的 Teams 应用以及授予每个应用的权限。  |否 | 否 |
| _OnlineMeeting.ReadBasic.Chat_   | 读取与此聊天关联的会议的基本属性。 | 允许应用在没有登录用户的情况下读取与此聊天关联的会议的基本属性（例如名称、日程安排、组织者和加入链接）。 |否 | 否 |
| _Calls.AccessMedia.Chat_         | 访问与此聊天或会议关联的通话中的媒体流。                                    | 允许应用在没有登录用户的情况下访问与此聊天或会议关联的通话中的媒体流。 |否 | 否 |
| _Calls.JoinGroupCalls.Chat_         | 加入与此聊天或会议关联的通话。                                    | 允许应用在没有登录用户的情况下加入与此聊天或会议关联的通话。 |否 | 否 |
| _TeamsActivity.Send.Chat_        | 向此聊天中的用户发送活动源通知。       | 允许此应用在没有登录用户的情况下，在此聊天中用户的团队合作活动源中创建新通知。 | 否 | 否 |

>[!NOTE]
> 目前，这些权限仅在 beta 版本的 Microsoft Graph 中受支持。

## <a name="chatmessage-permissions"></a>ChatMessage 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ChatMessage.Send_ | 发送用户聊天消息 | 允许应用代表已登录用户在 Microsoft Teams 中发送一对一以及群组聊天消息。 | 否 | 否 |

---

## <a name="cloud-pc-permissions"></a>云电脑权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | 读取云端电脑 | 允许应用代表已登录的用户读取云电脑对象（例如配置策略）。 | 否 | 否 |
|_CloudPC.ReadWrite.All_ | 读取和写入云端电脑 | 允许应用代表用户创建、读取、更新和删除云电脑对象，例如Azure 网络连接、预配策略和设备映像。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_CloudPC.Read.All_ | 读取云端电脑 | 无需登录用户，允许该应用读取 Cloud PC 对象，如设置策略。 | 否 | 否 |
|_CloudPC.ReadWrite.All_ | 读取和写入云端电脑 | 无需登录用户，允许该应用创建、读取、更新和删除 Cloud PC 对象，如 Azure 网络连接、设置策略和设备图像。 | 是 | 否 |

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _CloudPC.Read.All_：查看所有云电脑（`GET /deviceManagement/virtualEndpoint/cloudPCs`）的属性。
* _CloudPC.ReadWrite.All_：编辑云电脑设置策略（`PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}`）。

#### <a name="application"></a>应用程序

* _CloudPC.Read.All_：查看所有云电脑（`GET /deviceManagement/virtualEndpoint/cloudPCs`）的属性。
* _CloudPC.ReadWrite.All_：编辑云电脑设置策略（`PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}`）。

---

## <a name="consent-requests-permissions"></a>许可请求权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_ConsentRequest.Read.All_ |读取许可请求 |允许应用代表已登录用户读取许可请求和审批。 |是 | 否 |
|_ConsentRequest.ReadWrite.All_ |读取和写入许可请求 |允许应用代表已登录用户读取应用许可请求和审批，以及拒绝或批准这些请求。 |是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_ConsentRequest.Read.All_ |读取许可请求 |允许应用在未登录用户的情况下读取应用许可请求和审批。 |是 |
|_ConsentRequest.ReadWrite.All_ |读取和写入许可请求 |允许应用在没有登录用户的情况下读取应用许可请求和审批，以及拒绝或批准这些请求。 |是 |

## <a name="contacts-permissions"></a>联系人权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Contacts.Read_ |读取用户联系人  |允许应用读取用户联系人。 |否 | 是 |
|_Contacts.Read.Shared_ |读取用户联系人和共享联系人 |允许应用读取用户有权访问的联系人，包括用户个人联系人和共享联系人。 |否 |否|
|_Contacts.ReadWrite_ |具有对用户联系人的完整访问权限 |允许应用创建、读取、更新和删除用户联系人。 |否 |是|
|_Contacts.ReadWrite.Shared_ |读取和写入用户联系人和共享联系人 |允许应用创建、读取、更新和删除用户有权访问的联系人，包括用户个人联系人和共享联系人。 |否 |否|

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Contacts.Read_ |读取所有邮箱中的联系人 |允许应用在没有已登录用户的情况下读取所有邮箱中的所有联系人。 |是 |
|_Contacts.ReadWrite_ |读取和写入所有邮箱中的联系人 |允许应用在没有登录用户的情况下创建、读取、更新和删除所有邮箱中的全部联系人。 |是 |

> **重要说明** 管理员可以配置 [应用程序访问策略](auth-limit-mailbox-access.md)，以限制应用程序访问 _特定_ 邮箱，而不是组织中的所有邮箱，即使该应用程序已被授予 Contacts.Read 或 Contacts.ReadWrite 的应用程序权限。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委派

* _Contacts.Read_：从登录用户的一个顶层联系人文件夹读取联系人 (`GET /me/contactfolders/{Id}/contacts/{id}`)。
* _Contacts.ReadWrite_：更新登录用户的一个联系人的联系人照片 (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。
* _Contacts.ReadWrite_：将联系人添加到登录用户的根文件夹 (`POST /me/contacts`)。

#### <a name="application"></a>应用程序

* _Contacts.Read_：从组织中任意用户的一个顶层联系人文件夹读取联系人 (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`)。
* _Contacts.ReadWrite_：更新组织中任意用户的所有联系人的照片 (`PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。
* _Contacts.ReadWrite_：将联系人添加到组织中任意用户的根文件夹 (`POST /users/{id | userPrincipalName}/contacts`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="custom-security-attributes-permissions"></a>自定义安全属性权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _CustomSecAttributeAssignment.Read.All_ | 读取自定义安全属性分配 | 允许应用代表已登录用户读取租户中所有主体的自定义安全属性分配。 | 是 | 否 |
| _CustomSecAttributeAssignment.ReadWrite.All_ | 读取和写入自定义安全属性分配 | 允许应用代表已登录的用户读取和写入租户中所有主体的自定义安全属性分配。 | 是 | 否 |
| _CustomSecAttributeDefinition.Read.All_ | 读取自定义安全属性定义 | 允许应用代表已登录用户读取租户的自定义安全属性定义。 | 是 | 否 |
| _CustomSecAttributeDefinition.ReadWrite.All_ | 读取和写入自定义安全属性定义 | 允许应用代表已登录用户读取和写入租户的自定义安全属性定义。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _CustomSecAttributeAssignment.Read.All_ | 读取自定义安全属性分配 | 允许应用在没有登录用户的情况下读取租户中所有主体的自定义安全属性分配。 | 是 |
| _CustomSecAttributeAssignment.ReadWrite.All_ | 读取和写入自定义安全属性分配 | 允许应用代表已登录的用户读取和写入租户中所有主体的自定义安全属性分配。 | 是 |
| _CustomSecAttributeDefinition.Read.All_ | 读取自定义安全属性定义 | 允许应用在没有登录用户的情况下读取租户的自定义安全属性定义。 | 是 |
| _CustomSecAttributeDefinition.ReadWrite.All_ | 读取和写入自定义安全属性定义 | 允许应用在没有登录用户的情况下读取和写入租户的自定义安全属性定义。 | 是 |

---

## <a name="delegated-admin-relationship-permissions"></a>委派管理员关系权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _DelegatedAdminRelationship.Read.All_ | 读取委派管理员与客户的关系 | 允许应用代表已登录用户读取委派管理员与客户的关系的详细信息，例如访问详细信息（包括角色）和持续时间以及面向安全组的特定角色分配。 | 是 | 否 |
| _DelegatedAdminRelationship.ReadWrite.All_ | 管理委派管理员与客户的关系 | 允许应用代表你管理（创建-更新-终止）委派管理员与客户的关系，以及针对活动的委派管理员关系面向安全组的角色分配。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _DelegatedAdminRelationship.Read.All_ | 读取委派管理员与客户的关系 | 允许应用在无已登录用户的情况下，读取委派管理员与客户的关系的详细信息，例如访问详细信息（包括角色）和持续时间以及面向安全组的特定角色分配。 | 是 | 否 |
| _DelegatedAdminRelationship.ReadWrite.All_ | 管理委派管理员与客户的关系 | 允许应用在无已登录用户的情况下，管理（创建-更新-终止）委派管理员与客户的关系，以及针对活动的委派管理员关系面向安全组的角色分配。 | 是 | 否 |

---

## <a name="device-permissions"></a>设备权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Device.Read_ |读取用户设备 |允许应用代表已登录用户读取用户的设备列表。 |否 | 是 |
|_Device.Read.All_ |读取所有设备 |允许应用代表已登录用户读取组织设备的配置信息。|是 | 是 |
|_Device.Command_ |与用户设备通信 |允许应用启动其他应用，或代表已登录用户在用户设备上与其他应用进行通信。 |否 | 是 |


#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_Device.Read.All_ |读取所有设备 |允许应用在没有登录用户的情况下读取组织设备的配置信息。 |是 |
|_Device.ReadWrite.All_ |读取和写入设备 |支持应用程序读取和写入所有设备属性，而无需有登录用户。不得创建设备、删除设备或更新设备备用安全标识符。 |是 |

> [!NOTE]
> 2020 年 12 月 3 日之前，当应用程序权限 *Device.Read.All* 被授予时，[设备管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#deprecated-roles)目录角色也被分配给了应用程序的服务主体。 撤销关联的应用程序权限后，不会自动删除此目录角色分配。 为确保删除应用程序对设备的读写权限，客户还必须删除授予该应用程序的所有相关目录角色。
> 
> 禁用此行为的服务更新于 2020 年 12 月 3 日开始推出。 部署到所有客户，2021 年 1 月 11 日完成。 授予应用程序权限后，系统不再自动分配目录角色。

### <a name="example-usage"></a>用法示例

#### <a name="application"></a>应用程序

* _Device.ReadWrite.All_：读取组织中的所有已注册设备 (`GET /devices`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="directory-permissions"></a>目录权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Directory.Read.All_ |读取目录数据 | 允许应用程序读取组织目录中的数据，如用户、组和应用程序。 **注意**：如果应用程序已在自己组织的租户中注册，用户可能会同意应用程序要求必须有此权限。| 是 | 否 |
| _Directory.ReadWrite.All_ |读取和写入目录数据 | 允许应用读取和写入组织目录中的数据，如用户和组。它不允许应用删除用户或组，或重置用户密码。 | 是 | 否 |
| _Directory.AccessAsUser.All_ |以登录用户身份访问目录  | 允许应用以登录用户身份访问目录中的信息。 | 是 | 否 |

<br/>

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | 读取目录数据 | 允许应用在没有登录用户的情况下读取组织目录中的数据（如用户、组和应用）。 | 是 |
| _Directory.ReadWrite.All_ | 读取和写入目录数据 | 允许应用在没有登录用户的情况下读取和写入组织目录中的数据（如用户和组）。不允许删除用户或组。 | 是 |

### <a name="remarks"></a>注解

Directory 权限提供访问目录资源（如组织中的 [user](/graph/api/resources/user)、[group](/graph/api/resources/group) 和 [device](/graph/api/resources/device)）的最高级特权。

其还专门控制对其他目录资源的访问权限，例如: [组织联系人](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)、[架构扩展 API](/graph/api/resources/schemaextension?view=graph-rest-beta&preserve-view=true)、[Privileged Identity Management (PIM) API](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) 以及 v1.0 和 beta 版 API 参考文档中 **Azure Active Directory** 节点下列出的多个资源和 API。其中包含管理单元、目录角色、目录设置以及策略等。

> [!NOTE]
> 2020 年 12 月 3 日之前，当向应用程序授予权限 *Directory.Read.All* 时， [目录阅读器](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#directory-readers-permissions) 目录角色也分配给了应用程序的服务主体。 当 *Directory.ReadWrite.* 授予所有项目时， [作者](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#directory-writers-permissions) 分配了目录角色。 撤销关联的应用程序权限时，不会自动删除这些目录角色。 要删除应用程序对目录的读写权限，客户还必须删除授予该应用程序的所有目录角色。
> 
> 禁用此行为的服务更新于 2020 年 12 月 3 日开始推出。 部署到所有客户，2021 年 1 月 11 日完成。 授予应用程序权限后，系统不再自动分配目录角色。

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
- 管理目录设置
- 管理管理员许可工作流配置（但不要求管理员许可或授权授予管理员许可的用户）

> **注意**：
> - 无权重置用户密码。
> - 如需更新其他用户的 **businessPhones**、**mobilePhone** 或 **otherMails** 属性，仅允许针对非管理员或分配了以下角色之一的用户执行该操作：目录读取者、来宾邀请者、消息中心读取者和报告读取者。 有关详细信息，请参阅 [Azure AD 可用角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)中的支持人员（密码）管理员。  这适用于获得了 User.ReadWrite.All 或 Directory.ReadWrite.All 委派或应用程序权限的应用。
> - 无权删除资源（包括用户或组）。
> - 具体排除上面未列出的资源的创建或更新。 这包括：应用程序，oAauth2Permissiongrant，appRoleAssignment，设备，servicePrincipal，组织，域等。


### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派
* _Directory.Read.All_：列出组织中的所有管理单元 (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_：将成员添加到目录角色 (`POST /directoryRoles/{id}/members/$ref`)

#### <a name="application"></a>应用程序
* _Directory.Read.All_：列出用户的所有成员资格，包括目录角色和管理单元 (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_：列出所有组成员，包括服务主体 (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_：向组添加所有者 (`POST /groups/{id}/owners/$ref`)


有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="domain-permissions"></a>域权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_Domain.Read.All_ |读取域|允许应用代表已登录用户读取所有域属性。 |是 | 否 |
|_Domain.ReadWrite.All_ | 读取和写入域 |允许应用代表已登录用户读取和写入所有域属性。 还允许应用添加、验证和删除域。 |是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Domain.Read.All_ | 读取域 | 允许应用在没有登录用户的情况下读取所有域属性。 | 是 |
| _Domain.ReadWrite.All_ | 读取和写入域 | 允许应用在没有登录的用户的情况下读取和写入域。 | 是 |

---

## <a name="ediscovery-permissions"></a>电子数据展示权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_eDiscovery.Read.All_ |阅读用户电子数据展示案例数据 |允许应用代表已登录的用户读取电子数据展示对象，例如事例、保管人、审阅集和其他相关对象。 |是 | 否 |
|_eDiscovery.ReadWrite.All_ | 读取和编写电子数据展示案例数据 |允许应用代表已登录用户读取和写入电子数据展示对象，例如事例、保管人、审阅集和其他相关对象。 |是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _电子数据展示.读取.所有_：获取用户可用的事例列表（`GET /compliance/ediscovery/cases`）
* _电子数据展示.ReadWrite.所有_：在审阅集（审阅）`POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries`设置查询

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="education-permissions"></a>教育版权限

#### <a name="delegated-permissions"></a>委派权限

| 权限                      | 显示字符串                                                   | 说明                                                                                                                                                                                                                                                                      | 需经过管理员同意 | 支持的 Microsoft 帐户 |
| :------------------------------ | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------- | :-------------------------- |
| _EduAdministration.Read_        | 读取教育应用设置                                      | 允许应用代表用户读取教育应用设置。                                                                                                                                                                                                             | 是                    | 否                          |
| _EduAdministration.ReadWrite_   | 管理教育应用设置                                    | 允许应用代表用户管理教育应用设置。                                                                                                                                                                                                           | 是                    | 否                          |
| _EduAssignments.ReadBasic_      | 读取不含成绩的用户课堂作业                     | 允许应用代表用户读取不含成绩的作业                                                                                                                                                                                                          | 是                    | 否                          |
| _EduAssignments.ReadWriteBasic_ | 对不含成绩的用户课堂作业执行读取和写入操作           | 允许应用代表用户对不含成绩的作业执行读取和写入操作                                                                                                                                                                                                | 是                    | 否                          |
| _EduAssignments.Read_           | 读取用户的课堂作业及其成绩视图           | 允许应用代表用户读取作业及其成绩                                                                                                                                                                                                        | 是                    | 否                          |
| _EduAssignments.ReadWrite_      | 对用户的课堂作业及其成绩视图执行读取和写入操作 | 允许应用代表用户对作业及其成绩执行读取和写入操作                                                                                                                                                                                              | 是                    | 否                          |
| _EduRoster.ReadBasic_           | 读取用户的名单视图的有限子集               | 允许应用从组织名单中的学校和班级结构中读取属性的有限子集，以及有关要代表用户读取的用户的有限属性子集。包括姓名、状态、教育角色、电子邮件地址和照片。 | 是                    | 否                          |
| _EduRoster.Read_                | 读取用户名单的视图                                   | 允许应用读取组织名单中的学校和班级结构以及代表用户读取的有关用户的教育专属信息。                                                                                                         | 是                    |
| _EduRoster.ReadWrite_           | 读取并写入用户名单的视图                         | 允许应用读取和写入组织名单中的学校和班级结构以及代表用户读取和写入的有关用户的教育专属信息。                                                                                   | 是                    |

#### <a name="application-permissions"></a>应用程序权限

| 权限                          | 显示字符串                                      | 说明                                                                                                                                                                   | 需经过管理员同意 |
| :---------------------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------- |
| _EduAdministration.Read.All_        | 读取教育应用设置                         | 代表用户读取所有 Microsoft 教育应用的状态和设置                                                                                             | 是                    |
| _EduAdministration.ReadWrite.All_   | 管理教育应用设置                       | 代表用户管理所有 Microsoft 教育应用的状态和设置                                                                                           | 是                    |
| _EduAssignments.ReadBasic.All_      | 读取不含成绩的课堂作业               | 允许应用为所有用户读取不含成绩的作业                                                                                                               | 是                    |
| _EduAssignments.ReadWriteBasic.All_ | 对不含成绩的课堂作业执行读取和写入操作     | 允许应用为所有用户对不含成绩的的作业执行读取和写入操作                                                                                                     | 是                    |
| _EduAssignments.Read.All_           | 读取含成绩的课堂作业                  | 允许应用为所有用户读取作业及其成绩                                                                                                             | 是                    |
| _EduAssignments.ReadWrite.All_      | 对含成绩的课堂作业执行读取和写入操作        | 允许应用为所有用户对作业及其成绩执行读取和写入操作                                                                                                   | 是                    |
| _EduRoster.ReadBasic.All_           | 读取组织名单的有限子集。 | 允许应用读取组织名单中的学校和班级结构数据以及所有用户的教育专属信息的有限子集。          | 是                    |
| _EduRoster.Read.All_                | 读取组织名单。                     | 允许应用读取组织名单中的学校和班级结构数据以及所有用户的教育专属信息。                       | 是                    |
| _EduRoster.ReadWrite.All_           | 对组织名单执行读取和写入操作。           | 允许应用对组织名单中的学校和班级结构数据以及所有用户的教育专属信息执行读取和写入操作。 | 是                    |

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _EduAssignments.Read_：获取登录学生的作业信息 (`GET /education/classes/{id}/assignments/{id}`)
* _EduAssignments.ReadWriteBasic_：提交登录学生的作业 (`GET /education/classes/{id}/assignments/{id}submit`)
* _EduRoster.ReadBasic_：登录用户听讲或教授的课程 (`GET /education/classes/{id}/members`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="entitlement-management-permissions"></a>权利管理权限

#### <a name="delegated-permissions"></a>委派权限

|权限|显示字符串|说明|需经过管理员同意|
|:----------|:--------------|:-----------|:-------|
|_EntitlementManagement.ReadWrite.All_|读取和写入权利管理资源|允许应用代表已登录用户请求读取和管理访问包和相关权利管理资源的访问权限。|是|
|_EntitlementManagement.Read.All_|读取权利管理资源|允许应用代表已登录的用户请求读取访问包及相关权利管理资源的访问权限。|是|

#### <a name="application-permissions"></a>应用程序权限

|权限|显示字符串|说明|需经过管理员同意|
|:----------|:--------------|:-----------|:-------|
|_EntitlementManagement.ReadWrite.All_|读取和写入权利管理资源|允许应用读取和管理访问包和相关的权利管理资源。|是|
|_EntitlementManagement.Read.All_|读取权利管理资源|允许应用读取访问包和相关的权利管理资源。|是|

## <a name="files-permissions"></a>文件权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Files.Read_ | 读取用户文件 | 允许应用读取登录用户的文件。 | 否 | 是 |
| _Files.Read.All_ | 读取用户可以访问的所有文件 | 允许应用读取登录用户可以访问的所有文件。 | 否 | 是 |
| _Files.ReadWrite_  | 具有对用户文件的完全访问权限 | 允许应用读取、创建、更新和删除登录用户的文件。 | 否| 是 |
| _Files.ReadWrite.All_ | 具备对用户可以访问的所有文件的完全访问权限 | 允许应用读取、创建、更新和删除登录用户可以访问的所有文件。 | 否 | 是 |
| _Files.ReadWrite.AppFolder_ | 具有对应用程序文件夹的完全访问权限（预览） | （预览）允许应用读取、创建、更新和删除应用程序文件夹中的文件。 | 否 | 是 |
| _Files.Read.Selected_  | 读取用户选择的文件 | **Microsoft Graph 提供一定程度的支持（见“注解”）** <br/> （预览）允许应用读取用户选择的文件。在用户选择文件后，应用有几个小时的访问权限。  | 否 | 否 |
| _Files.ReadWrite.Selected_ | 读取和写入用户选择的文件 | **Microsoft Graph 提供一定程度的支持（见“注解”）** <br/> （预览）允许应用读取和写入用户选择的文件。在用户选择文件后，应用有几个小时的访问权限。 | 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 |
| :--------- | :------------- | :---------- | :--------------------- |
| _Files.Read.All_ | 读取所有网站集中的文件 | 允许应用在没有登录用户的情况下读取所有网站集中的全部文件。  | 是 |
| _Files.ReadWrite.All_ | 读取和写入所有网站集中的文件 | 允许应用在没有登录用户的情况下读取、创建、更新和删除所有网站集中的全部文件。 | 是 |

### <a name="remarks"></a>注解

> **注意**：对于个人帐户，Files.Read 和 Files.ReadWrite 还会授予与登录用户共享的文件的访问权限。

Files.Read.Selected 和 Files.ReadWrite.Selected 委派权限仅在工作或学校帐户上有效，并仅在处理 [Office 365 文件处理程序 (v1.0)](/previous-versions/office/office-365-api/) 时才公开。它们不应该用来直接调用 Microsoft Graph API。

Files.ReadWrite.AppFolder 委派权限仅适于个人帐户，并仅用于访问带有 OneDrive [获取特殊文件夹](/graph/api/drive-get-specialfolder) Microsoft Graph API 的[应用程序根特殊文件夹](https://dev.onedrive.com/misc/appfolder.htm)。


### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Files.Read_：读取登录用户的 OneDrive 中存储的文件 (`GET /me/drive/root/children`)
* _Files.Read.All_：列出与登录用户共享的文件 (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_：在登录用户的 OneDrive 中写入文件 (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_：写入与用户共享的文件 (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_：在 OneDrive 中将文件写入应用程序的文件夹 (`PUT /me/drive/special/approot/children/file.txt/content`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---
## <a name="financials-permissions"></a>财务权限
#### <a name="delegated-permissions"></a>委派权限

|权限|显示字符串|说明|需经过管理员同意|
|:----------|:--------------|:-----------|:-------|
|_Financials.ReadWrite.All_|读取和写入财务数据|允许应用代表登录用户读取和写入财务数据|否|

## <a name="group-permissions"></a>组权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Group.Read.All_ |    读取所有组 | 允许应用代表登录用户列出组，并读取其属性以及所有组成员身份。此外，还允许应用读取登录用户可以访问的所有组的日历、 对话、 文件和其他组内容。 | 是 | 否 |
| _Group.ReadWrite.All_ |    读取和写入所有组| 允许应用代表登录用户创建组并读取所有组属性和成员身份。  此外，还允许应用读取和写入登录用户可以访问的所有组的日历、对话、文件和其他组内容。 此外，还允许组所有者管理他们的组并允许组成员更新组内容。 | 是 | 否 |
| _GroupMember.Read.All_ |    读取组成员身份 | 允许应用列出组、读取基本组属性以及读取登录的用户有权访问的所有组的成员身份。 | 是 | 否 |
| _GroupMember.ReadWrite.All_ |    读取和写入组成员身份 | 允许应用列出组、读取基本属性、读取和更新登录的用户有权访问的组的成员身份。 无法更新组属性和所有者，并且无法删除组。 | 是 | 否 |
| _UnifiedGroupMember.Read.AsGuest_ |    以来宾用户身份读取统一 (Microsoft 365) 组成员身份 | 允许应用读取登录来宾所属组的基本统一组属性、成员身份和组所有者。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | 读取所有组 | 允许应用在没有登录用户的情况下读取所有组的成员身份。此外，还允许应用读取所有组的日历、对话、文件和其他组内容。<br/><br/>**注意：** 并非所有组 API 都支持使用仅限应用权限进行访问。 有关示例，请参阅[已知问题](known-issues.md)。 | 是 |
| _Group.ReadWrite.All_ | 读取和写入所有组 | 允许应用创建组、读取和更新组成员以及删除组。 此外，还允许应用读取和写入所有组的日历、对话、文件和其他组内容。 应用可以在没有登录用户的情况下执行所有这些操作。<br/><br/>**注意：** 并非所有组 API 都支持使用仅限应用权限进行访问。 有关示例，请参阅[已知问题](known-issues.md)。| 是 |
| _Group.Selected_ |    访问选定的组 | **注意：此权限在 Azure 门户中公开，适用于不可用作常规用途的功能。请不要使用此权限，因为它可能会发生更改。** | 是 |
| _GroupMember.Read.All_ |    读取组成员身份 | 允许应用在没有已登录用户的情况下读取所有组的成员身份和基本组属性。 | 是 |
| _GroupMember.ReadWrite.All_ |    读取和写入组成员身份 | 允许应用在没有已登录用户的情况下列出组、读取基本属性、读取和更新组的成员资格。 无法更新组属性和所有者，并且无法删除组。 | 是 |
| _Group.Create_ |    创建组 | 允许呼叫应用在没有已登录用户的情况下创建组。 不允许读取、更新或删除任何组。 | 是 |

### <a name="remarks"></a>注解

Microsoft 个人帐户不支持组功能。

Microsoft 365 组的组权限授予应用访问组内容的访问权限；例如，对话、文件、注释等。

应用程序权限对受支持的 API 有一些限制。有关详细信息，请参阅[已知问题](known-issues.md)。

在某些情况下，应用可能需要 [目录权限](#directory-permissions)才能读取 `member` 和 `memberOf` 等组属性。例如，如果组将一个或多个 [servicePrincipals](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) 作为成员，则应用将需要有效权限才能通过授予的其中一个 _目录\*_ 权限读取服务主体，否则 Microsoft Graph 将返回错误。（如果是委派权限，已登录用户还需要组织的足够的权限才能读取服务主体。）相同的指导适用于 `memberOf` 属性，该属性可以返回 [administrativeUnits](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true)。

要设置 Microsoft 365 组的 **preferredDataLocation** 属性，应用需要 Directory.ReadWrite.All 权限。 多地理位置环境中的用户创建 Microsoft 365 组时，该组的 **preferredDataLocation** 值将自动设置为该用户所使用的值。 有关组的首选数据位置的详细信息，请参阅[使用特定 PDL 创建 Microsoft 365 组](/office365/enterprise/multi-geo-add-group-with-pdl)。

组权限用于控制对 [Microsoft Teams](/graph/api/resources/teams-api-overview) 资源和 API 的访问权限。不支持 Microsoft 个人帐户。

组权限也用于控制对 [Microsoft Planner](/graph/api/resources/planner-overview) 资源和 API 的访问权限。Microsoft Planner API 仅支持委派权限，不支持应用程序权限。不支持 Microsoft 个人帐户。


### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>Delegated

* _Group.Read.All_：读取登录用户所属的全部 Microsoft 365 组 (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`)。
* _Group.Read.All_：读取诸如对话之类的所有 Microsoft 365 组内容 (`GET /groups/{id}/conversations`)。
* _Group.ReadWrite.All_：更新组属性，如照片 (`PUT /groups/{id}/photo/$value`)。
* _GroupMember.ReadWrite.All_：更新组成员 (`POST /groups/{id}/members/$ref`)。
> **注意：** 这还要求 _User.ReadBasic.All_ 读取要作为成员添加的用户。

#### <a name="application"></a>应用程序

* _Group.Read.All_：查找名称以“Sales”开头的所有组 (`GET /groups?$filter=startswith(displayName,'Sales')`)。
* _Group.ReadWrite.All_：守护程序服务在 Microsoft 365 组日历上新建事件 (`POST /groups/{id}/events`)。
* _Group.Create_：创建新组 (`POST /groups`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---


## <a name="identity-provider-permissions"></a>标识提供程序权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityProvider.Read.All_ |   读取标识提供程序信息  | 支持应用程序代表登录用户读取在 Azure AD 或 Azure AD B2C 租户中配置的标识提供程序。 | 是 | 否 |
| _IdentityProvider.ReadWrite.All_ |   读取和写入标识提供程序信息  |  支持应用程序代表登录用户读取或写入在 Azure AD 或 Azure AD B2C 租户中配置的标识提供程序。 | 是 | 否 |

### <a name="remarks"></a>注解

_IdentityProvider.Read.All_ 和 _IdentityProvider.ReadWrite.All_ 仅对工作或学校帐户有效。对于使用委派权限读取或写入标识提供程序的应用，已登录用户必须分配为全局管理员角色。有关管理员角色的详细信息，请参阅 [在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

### <a name="example-usage"></a>示例用法

#### <a name="delegated"></a>委派
以下用法对两种委派权限均有效：

* _IdentityProvider.Read.All_：读取在租户中配置的所有标识提供程序 (`GET /beta/identityProviders`)
* _IdentityProvider.Read.All_：读取现有标识提供程序 (`GET /beta/identityProviders/{id}`)
* _IdentityProvider.ReadWrite.All_：创建标识提供程序 (`POST /beta/identityProviders`)
* _IdentityProvider.ReadWrite.All_：更新现有标识提供程序 (`PATCH /beta/identityProviders/{id}`)
* _IdentityProvider.ReadWrite.All_：删除现有标识提供程序 (`DELETE /beta/identityProviders/{id}`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="identity-protection-risk-permissions"></a>标识保护风险权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityRiskEvent.Read.All_ |   读取标识风险事件信息  | 允许应用代表登录用户为组织中所有用户读取标识风险事件信息。 | 是 | 否 |
| _IdentityRiskyUser.Read.All_ |   读取标识用户风险信息  | 允许应用代表登录用户读取组织中所有用户的标识用户风险信息。 | 是 | 否 |
| _IdentityRiskyUser.ReadWrite.All_ |   读取和更新标识用户风险信息  | 允许应用代表登录用户读取和更新组织中所有用户的标识用户风险信息。 | 是 | 否 |
| _IdentityRiskyServicePrincipal.Read.All_ |   读取所有风险服务主体信息  | 允许应用代表已登录用户读取组织的所有风险服务主体信息。 | 是 | 否 |
| _IdentityRiskyServicePrincipal.ReadWrite.All_ |   读取和写入所有风险服务主体信息  | 允许应用代表已登录用户读取和更新组织中所有服务主体的风险服务主体信息。更新操作包括消除有风险的服务主体。| 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   读取标识风险事件信息 | 允许应用无需具有已登录用户即可为组织中所有用户读取标识风险事件信息。 | 是 |
| _IdentityRiskyUser.Read.All_ |   读取标识用户风险信息 | 允许应用在没有登录用户的情况下读取组织中所有用户的标识用户风险信息。 | 是 |
| _IdentityRiskyUser.ReadWrite.All_ |   读取和更新标识用户风险信息 | 允许应用在没有登录用户的情况下读取和更新组织中所有用户的标识用户风险信息。 | 是 |
| _IdentityRiskyServicePrincipal.Read.All_ |   读取所有风险服务主体信息  | 允许应用在没有登录用户的情况下读取组织的所有有风险的服务主体信息。 | 是 |
| _IdentityRiskyServicePrincipal.ReadWrite.All_ |   读取和写入所有风险服务主体信息  | 允许应用在没有登录用户的情况下读取和更新组织的风险服务主体。| 是 |

所有标识风险权限仅对工作或学校帐户有效。对于具有读取标识风险信息的委派权限的应用，登录用户必须是以下 [Azure AD管理员角色之一的成员](/azure/active-directory/roles/permissions-reference)：全局管理员、安全管理员或安全读取者。

### <a name="example-usage"></a>用法示例

以下用法对委派权限和应用程序权限均有效：

#### <a name="read-risk-events"></a>读取风险事件

* 读取为租户中的所有用户所生成的全部风险事件 (`GET /identityProtection/riskDetections`)
* 阅读最新的 50 个风险事件 (`GET /identityProtection/riskDetections?$orderBy=detectedDateTime desc&top=50`)

#### <a name="read-risky-users"></a>读取有风险的用户

* 读取租户中的所有风险用户和属性 (`GET /identityProtection/riskyUsers`)
* 读取所有聚合风险级别为中等的风险用户 (`GET /identityProtection/riskyUsers?$filter=riskLevel eq 'medium'`)
* 阅读特定用户的风险信息 (`GET /identityProtection/riskyUsers?$filter=id eq 'userId'`)

#### <a name="read-risky-service-principals"></a>读取有风险的服务主体

* 读取租户中的所有有风险的服务主体和属性（`GET /identityProtection/riskyServicePrincipals`）
* 读取聚合风险级别为中等 （`GET /identityProtection/riskyServicePrincipals?$filter=riskLevel eq 'medium'`） 的所有风险服务主体
* 阅读特定服务主体的风险信息（`GET /identityProtection/riskyServicePrincipals?$filter=id eq '{riskyServicePrincipalsId}'`）

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="identity-user-flow-permissions"></a>标识用户流权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityUserFlow.Read.All_ |   读取租户中的所有标识用户流  | 允许应用读取组织的用户流。 | 是 | 否 |
| _IdentityUserFlow.ReadWrite.All_ |   读取和写入租户中的所有标识用户流。    | 允许应用程序读取或写入组织的用户流。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _IdentityUserFlow.Read.All_ |   读取租户中的所有标识用户流  | 允许应用读取组织的用户流。 | 是 | 否 |
| _IdentityUserFlow.ReadWrite.All_ |   读取和写入租户中的所有标识用户流。    | 允许应用程序读取或写入组织的用户流。 | 是 | 否 |

### <a name="remarks"></a>说明

_IdentityUserFlow.Read.All_ 和 _IdentityUserFlow.ReadWrite.ALL_ 仅适用于工作或学校帐户。

对于具有读取用户流的委托权限的应用程序，登录用户必须是以下管理员角色之一的成员：全局管理员、外部身份用户流管理员或全局读者。 对于具有委托权限的应用程序来说，若要编写用户流，登录的用户必须是以下管理员角色之一的成员：全局管理员或外部身份用户流管理员。

若要详细了解管理员角色，请参阅[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

### <a name="example-usage"></a>用法示例

#### <a name="delegated-and-application"></a>委派和应用程序

以下用法对委派权限和应用程序权限均有效：

* _IdentityUserFlow.Read.All_：读取 Azure AD B2C 租户中的所有用户流 (`GET beta/identity/b2cUserFlows`) 
* _IdentityUserFlow.Read.All_：读取 Azure Active Directory (Azure AD) 租户中的所有用户流 (`GET beta/identity/b2xUserFlows`) 
* _IdentityUserFlow.Read.All_：读取 Azure AD B2C 用户流中的所有用户属性分配（`GET beta/identity/b2cUserFlows/{id}/userAttributeAssignments`） 
* _IdentityUserFlow.ReadWrite.All_：在 Azure AD B2C 租户中创建新用户流 (`POST beta/identity/b2cUserFlows`)
* _IdentityUserFlow.ReadWrite.All_：在 Azure Active Directory (Azure AD) 租户中创建新用户流 (`POST beta/identity/b2xUserflows`)
* _IdentitytUserFlow.ReadWrite.All_：将标识提供者添加到 Azure AD B2C 用户流 (`PATCH beta/identity/b2cUserFlows/{id}/identityProviders/$ref`)
* _IdentityUserFlow.ReadWrite.All_：从 Azure AD B2C 用户流中删除标识提供者 (`DELETE beta/identity/b2cUserFlows/{id}/identityProviders/{id}`)
* _IdentityUserFlow.ReadWrite.All_：在 Azure AD B2C 用户流中创建用户属性分配（`POST beta/identity/b2cUserFlows/{id}/userAttributeAssignments`）

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="information-protection-policy-permissions"></a>信息保护策略权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _InformationProtectionPolicy.Read_ |   读取用户敏感度标签和标签策略 | 允许应用代表已登录用户读取信息保护敏感度标签，以及标签策略设置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _InformationProtectionPolicy.Read.All_ |   读取组织的所有已发布标签和标签策略 | 无需已登录用户，允许应用读取整个组织或特定用户发布的敏感度标签和标签策略设置。 | 是 |

---


## <a name="intune-device-management-permissions"></a>Intune 设备管理权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_DeviceManagementApps.Read.All_ | 读取 Microsoft Intune 应用 | 允许应用读取由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 | 否 |
|_DeviceManagementApps.ReadWrite.All_ | 读取和写入 Microsoft Intune 应用 | 允许应用读取和写入由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 | 否 |
|_DeviceManagementConfiguration.Read.All_ | 读取 Microsoft Intune 设备配置和策略 | 允许应用读取 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 | 否 |
|_DeviceManagementConfiguration.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备配置和策略  | 允许应用读取和写入 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 | 否 |
|_DeviceManagementManagedDevices.PrivilegedOperations.All_ | 在 Microsoft Intune 设备上执行影响用户的远程操作 | 允许应用执行高影响级别远程操作，如在由 Microsoft Intune 管理的设备上擦除设备或重置密码。 | 是 | 否 |
|_DeviceManagementManagedDevices.Read.All_ | 读取 Microsoft Intune 设备 | 允许应用读取由 Microsoft Intune 管理的设备的属性。 | 是 | 否 |
|_DeviceManagementManagedDevices.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备 | 允许应用读取和写入由 Microsoft Intune 管理的设备的属性。不允许执行具有高影响级别的操作，例如针对设备所有者的远程擦除和密码重置。 | 是 | 否 |
|_DeviceManagementRBAC.Read.All_ | 读取 Microsoft Intune RBAC 设置 | 允许应用读取与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 | 否 |
|_DeviceManagementRBAC.ReadWrite.All_ | 读取和写入 Microsoft Intune RBAC 设置 | 允许应用读取和写入与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 | 否 |
|_DeviceManagementServiceConfig.Read.All_ | 读取 Microsoft Intune 配置 | 允许应用读取 Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 | 否 |
|_DeviceManagementServiceConfig.ReadWrite.All_ | 读取和写入 Microsoft Intune 配置 | 允许应用读取和写入 Microsoft Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_DeviceManagementApps.Read.All_ | 读取 Microsoft Intune 应用 | 允许应用读取由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 | 否 |
|_DeviceManagementApps.ReadWrite.All_ | 读取和写入 Microsoft Intune 应用 | 允许应用读取和写入由 Microsoft Intune 管理的应用、应用配置和应用保护策略的属性、组分配情况和状态。 | 是 | 否 |
|_DeviceManagementConfiguration.Read.All_ | 读取 Microsoft Intune 设备配置和策略 | 允许应用读取 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 | 否 |
|_DeviceManagementConfiguration.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备配置和策略  | 允许应用读取和写入 Microsoft Intune 管理的设备配置的属性和设备符合性策略以及它们对组的分配情况。 | 是 | 否 |
|_DeviceManagementManagedDevices.PrivilegedOperations.All_ | 在 Microsoft Intune 设备上执行影响用户的远程操作 | 允许应用执行高影响级别远程操作，如在由 Microsoft Intune 管理的设备上擦除设备或重置密码。 | 是 | 否 |
|_DeviceManagementManagedDevices.Read.All_ | 读取 Microsoft Intune 设备 | 允许应用读取由 Microsoft Intune 管理的设备的属性。 | 是 | 否 |
|_DeviceManagementManagedDevices.ReadWrite.All_ | 读取和写入 Microsoft Intune 设备 | 允许应用读取和写入由 Microsoft Intune 管理的设备的属性。不允许执行具有高影响级别的操作，例如针对设备所有者的远程擦除和密码重置。 | 是 | 否 |
|_DeviceManagementRBAC.Read.All_ | 读取 Microsoft Intune RBAC 设置 | 允许应用读取与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 | 否 |
|_DeviceManagementRBAC.ReadWrite.All_ | 读取和写入 Microsoft Intune RBAC 设置 | 允许应用读取和写入与基于 Microsoft Intune 角色的访问控制 (RBAC) 设置相关的属性。 | 是 | 否 |
|_DeviceManagementServiceConfig.Read.All_ | 读取 Microsoft Intune 配置 | 允许应用读取 Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 | 否 |
|_DeviceManagementServiceConfig.ReadWrite.All_ | 读取和写入 Microsoft Intune 配置 | 允许应用读取和写入 Microsoft Intune 服务属性，其中包括设备注册和第三方服务连接配置。 | 是 | 否 |

### <a name="remarks"></a>注解

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

这些权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _DeviceManagementServiceConfiguration.Read.All_：检查 Intune 订阅的当前状态 (`GET /deviceManagement/subscriptionState`)。
* _DeviceManagementServiceConfiguration.ReadWrite.All_：新建条款和条件 (`POST /deviceManagement/termsAndConditions`)。
* _DeviceManagementConfiguration.Read.All_：查找设备配置状态 (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)。
* _DeviceManagementConfiguration.ReadWrite.All_：向组分配设备符合性策略 (`POST deviceCompliancePolicies/{id}/assign`)。
* _DeviceManagementApps.Read.All_：查找发布到 Intune 的所有 Windows 应用商店应用 (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)。
* _DeviceManagementApps.ReadWrite.All_：发布新应用程序 (`POST /deviceAppManagement/mobileApps`)。
* _DeviceManagementRBAC.Read.All_：按名称查找角色分配 (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)。
* _DeviceManagementRBAC.ReadWrite.All_：新建自定义角色 (`POST /deviceManagement/roleDefinitions`)。
* _DeviceManagementManagedDevices.Read.All_：按名称查找受管理设备 (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)。
* _DeviceManagementManagedDevices.ReadWrite.All_：删除受管理设备 (`DELETE /managedDevices/{id}`)。
* _DeviceManagementManagedDevices.PrivilegedOperations.All_：重置用户的受管理设备上的密码 (`POST /managedDevices/{id}/resetPasscode`)。

#### <a name="application"></a>应用程序

* _DeviceManagementServiceConfiguration.Read.All_：检查 Intune 订阅的当前状态 (`GET /deviceManagement/subscriptionState`)。
* _DeviceManagementServiceConfiguration.ReadWrite.All_：新建条款和条件 (`POST /deviceManagement/termsAndConditions`)。
* _DeviceManagementConfiguration.Read.All_：查找设备配置状态 (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)。
* _DeviceManagementConfiguration.ReadWrite.All_：向组分配设备符合性策略 (`POST deviceCompliancePolicies/{id}/assign`)。
* _DeviceManagementApps.Read.All_：查找发布到 Intune 的所有 Windows 应用商店应用 (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)。
* _DeviceManagementApps.ReadWrite.All_：发布新应用程序 (`POST /deviceAppManagement/mobileApps`)。
* _DeviceManagementRBAC.Read.All_：按名称查找角色分配 (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)。
* _DeviceManagementRBAC.ReadWrite.All_：新建自定义角色 (`POST /deviceManagement/roleDefinitions`)。
* _DeviceManagementManagedDevices.Read.All_：按名称查找受管理设备 (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)。
* _DeviceManagementManagedDevices.ReadWrite.All_：删除受管理设备 (`DELETE /managedDevices/{id}`)。
* _DeviceManagementManagedDevices.PrivilegedOperations.All_：重置用户的受管理设备上的密码 (`POST /managedDevices/{id}/resetPasscode`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="mail-permissions"></a>邮件权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Mail.Read_ |    读取用户邮件 | 允许应用读取用户邮箱中的电子邮件。 | 否 | 是
| _Mail.ReadBasic_ |    读取用户基本邮件 | 允许应用读取已登录用户邮箱中的电子邮件， **正文** 除外， **bodyPreview**、 **uniqueBody**、 **附件**、 **扩展** 以及任何扩展属性。不包括搜索邮件的权限。 | 否 | 否
| _Mail.ReadWrite_ |    对用户邮件的读写权限 | 允许应用创建、读取、更新和删除用户邮箱中的电子邮件。不包括发送电子邮件的权限。| 否 | 是
| _Mail.Read.Shared_ |    读取用户邮件和共享邮件 | 允许应用读取用户可以访问的邮件，包括用户个人邮件和共享邮件。 | 否 | 否
| _Mail.ReadWrite.Shared_ |    读取和写入用户邮件和共享邮件 | 允许应用创建、读取、更新和删除用户有权访问的邮件，包括用户个人邮件和共享邮件。不包括邮件发送权限。 | 否 | 否
| _Mail.Send_ |    以用户身份发送邮件 | 允许应用以组织用户身份发送邮件。 | 否 | 是
| _Mail.Send.Shared_ |    代表他人发送邮件 | 允许应用以登录用户身份发送邮件，包括代表他人发送邮件。 | 否 | 否
| _MailboxSettings.Read_ |  读取用户的邮箱设置 | 允许应用读取用户的邮箱设置。不包括邮件发送权限。 | 否 | 是
| _MailboxSettings.ReadWrite_ |  读取和写入用户邮箱设置 | 允许应用创建、读取、更新和删除用户邮箱设置。 不包含直接发送邮件的权限，但允许应用创建能够转发或重定向邮件的规则。 | 否 | 是
| _IMAP.AccessAsUser.All_ | 通过IMAP对用户邮件进行读写访问 | 允许应用读取、更新、创建和删除用户邮箱中的电子邮件。不包括发送电子邮件的权限。 | 否 | 是
| _POP.AccessAsUser.All_ | 通过POP对用户邮件读写访问 | 允许应用读取、更新、创建和删除用户邮箱中的电子邮件。不包括发送电子邮件的权限。 | 否 | 是
| _SMTP.Send_ | 使用SMTP AUTH以用户身份发送邮件 | 允许应用以组织用户身份发送邮件。 | 否 | 是

#### <a name="application-permissions"></a>应用程序权限

| 权限                  | 显示字符串                           | 说明                                                                                                                                                                        | 需经过管理员同意 |
|:----------------------------|:-----------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|
| _Mail.Read_                 | 读取所有邮箱中的邮件               | 允许应用在没有登录用户的情况下读取所有邮箱中的邮件。                                                                                                             | 是                    |
| _Mail.ReadBasic.All_        | 读取所有用户基本邮件                | 允许此应用读取除 Body、BodyPreview、UniqueBody、Attachments、ExtendedProperties 和扩展以外的所有用户邮箱。不包括搜索邮件的权限。 | 是                    |
| _Mail.ReadWrite_            | 读取和写入所有邮箱中的邮件     | 允许应用在没有登录用户的情况下创建、读取、更新和删除所有邮箱中的邮件。不包括发送电子邮件的权限。                                       | 是                    |
| _Mail.Send_                 | 以任意用户身份发送邮件                    | 允许应用在没有登录用户的情况下以任意用户身份发送邮件。                                                                                                                  | 是                    |
| _MailboxSettings.Read_      | 读取用户的所有邮箱设置           | 允许应用在没有已登录用户的情况下读取用户邮箱设置。不包括邮件发送权限。                                                                 | 否                     |
| _MailboxSettings.ReadWrite_ | 读取和写入所有用户邮箱设置 | 允许应用在没有登录用户的情况下创建、读取、更新和删除用户邮箱设置。不包括邮件发送权限。                                     | 是                    |

> **重要说明** 管理员可以配置 [应用程序访问策略](auth-limit-mailbox-access.md)，以限制应用程序访问 _特定_ 邮箱，而不是组织中的所有邮箱，即使该应用程序已被授予 Mail.Read、Mail.ReadWrite、Mail.Send、MailboxSettings.Read 或 MailboxSettings.ReadWrite 的应用程序权限。


### <a name="remarks"></a>说明

_Mail.Read.Shared_、_Mail.ReadWrite.Shared_ 和 _Mail.Send.Shared_ 仅适用于工作或学校帐户。所有其他权限对于 Microsoft 帐户和工作或学校帐户均有效。

通过 _Mail.Send_ 或 _Mail.Send.Shared_ 权限，应用可以发送邮件并将副本保存到用户的“已发送邮件”文件夹中，即使应用不使用相应的 _Mail.ReadWrite_ 或 _Mail.ReadWrite.Shared_ 权限也是如此。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Mail.Read_：列出用户收件箱中的邮件，按 `receivedDateTime` 排序 (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`)。
* _Mail.Read.Shared_：在已与登录用户共享其收件箱的用户收件箱中查找带有附件的所有邮件 (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`)。
* _Mail.ReadWrite_：将邮件标记为已读 (`PATCH /me/messages/{id}`)。
* _Mail.Send_：发送邮件 (`POST /me/sendmail`)。
* _MailboxSettings.ReadWrite_：更新用户的自动答复 (`PATCH /me/mailboxSettings`)。

#### <a name="application"></a>应用程序

* _Mail.Read_：从 bob@contoso.com 查找邮件 (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`)。
* _Mail.ReadWrite_：在名为“`Expense Reports`”的收件箱中新建文件夹 (`POST /users/{id | userPrincipalName}/mailfolders`)。
* _Mail.Send_：发送邮件 (`POST /users/{id | userPrincipalName}/sendmail`)。
* _MailboxSettings.Read_：获取用户邮箱的默认时区 (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="managed-tenant-permissions"></a>托管租户权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ManagedTenants.Read.All_ | 读取所有托管租户特定信息 | 允许应用代表登录用户读取所有托管租户信息。 | 是 | 否 |
| _ManagedTenants.ReadWrite.All_ | 读取和写入所有托管租户特定信息 | 允许应用代表登录用户读取和写入所有托管租户信息。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

---

## <a name="member-permissions"></a>成员权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Member.Read.Hidden_ | 读取隐藏成员资格 | 对于已登录用户具有访问权限的隐藏组和管理单元，允许应用代表已登录用户读取隐藏组和管理单元的成员资格。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Member.Read.Hidden_ | 读取所有隐藏成员 | 允许应用在没有登录用户的情况下读取隐藏的组和管理单元中的成员。 | 是 |

### <a name="remarks"></a>注释
_Member.Read.Hidden_ 仅对工作或学校帐户有效。

可以隐藏某些 Microsoft 365 组中的成员资格。这意味着只有该组的成员可以查看其成员。此功能可用于帮助遵守要求组织对外部用户（例如，表示某个班级内注册的学生的 Microsoft 365 组）隐藏组成员身份的规定。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Member.Read.Hidden_：代表登录用户读取隐藏了成员资格的管理单元成员 (`GET /administrativeUnits/{id}/members`)。
* _Member.Read.Hidden_：代表登录用户读取隐藏了成员资格的组成员 (`GET /groups/{id}/members`)。

#### <a name="application"></a>应用程序

* _Member.Read.Hidden_：读取隐藏了成员资格的管理单元成员 (`GET /administrativeUnits/{id}/members`)。
* _Member.Read.Hidden_：读取隐藏了成员资格的组成员 (`GET /groups/{id}/members`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="notes-permissions"></a>注释权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Notes.Read_ |    读取用户 OneNote 笔记本 | 允许应用代表已登录用户读取 OneNote 笔记本和分区标题并创建新的页面、笔记本和分区。 | 否 | 是
| _Notes.Create_ |    创建用户 OneNote 笔记本 | 允许应用代表已登录用户读取 OneNote 笔记本和分区标题并创建新的页面、笔记本和分区。| 否 | 是
| _Notes.ReadWrite_ |    读取和写入用户 OneNote 笔记本 | 允许应用代表已登录用户读取、共享和修改 OneNote 笔记本。 | 否 | 是
| _Notes.Read.All_ |    读取用户可以访问的所有 OneNote 笔记本 | 允许应用读取登录用户在组织中有权访问的 OneNote 笔记本。 | 否 | 否
| _Notes.ReadWrite.All_ |    读取和写入用户可以访问的所有 OneNote 笔记本。 | 允许应用读取、共享和修改已登录用户在组织中有权访问的 OneNote 笔记本。| 否 | 否
| _Notes.ReadWrite.CreatedByApp_ |    有限的笔记本访问权限（不推荐使用） | **不推荐使用** <br/>请勿使用。此权限不授予任何特权。 | 否 | 否

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Notes.Read.All_ |    读取所有 OneNote 笔记本 | 允许应用无需具有已登录用户即可读取组织中的所有 OneNote 笔记本。 | 是 |
| _Notes.ReadWrite.All_ |    读取和写入所有 OneNote 笔记本 | 允许应用无需具有已登录用户即可读取、共享和修改组织中的所有 OneNote 笔记本。| 是 |


### <a name="remarks"></a>注解
_Notes.Read.All_ 和 _Notes.ReadWrite.All_ 仅适用于工作或学校帐户。所有其他权限对于 Microsoft 帐户和工作或学校帐户均有效。

通过 _Notes.Create_ 权限，应用可以查看已登录用户的 OneNote 笔记本层次结构，并创建 OneNote 内容（笔记本、分区组、分区、页面等）。

_Notes.ReadWrite_ 和 _Notes.ReadWrite.All_ 还允许应用修改针对已登录用户可以访问的 OneNote 内容的权限。

对于工作或学校帐户，_Notes.Read.All_ 和 _Notes.ReadWrite.All_ 允许该应用访问已登录用户有权限在组织内访问的其他用户的 OneNote 内容。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委派

* _Notes.Create_：为登录用户新建笔记本 (`POST /me/onenote/notebooks`)。
* _Notes.Read_：读取登录用户的笔记本 (`GET /me/onenote/notebooks`)。
* _Notes.Read.All_：获取登录用户有权在组织内访问的所有笔记本 (`GET /me/onenote/notebooks?includesharednotebooks=true`)。
* _Notes.ReadWrite_：更新登录用户的页面 (`PATCH /me/onenote/pages/{id}/$value`)。
* _Notes.ReadWrite.All_：在登录用户有权在组织内访问的其他用户笔记本中创建页面 (`POST /users/{id}/onenote/pages`)。

#### <a name="application"></a>应用程序

* _Notes.Read.All_：读取组中的所有用户笔记本 (`GET /groups/{id}/onenote/notebooks`)。
* _Notes.ReadWrite.All_：更新组织中任意用户的笔记本中的页面 (`PATCH /users/{id}/onenote/pages/{id}/$value`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="notifications-permissions"></a>通知权限
#### <a name="delegated-permissions"></a>委派权限
|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notifications.ReadWrite.CreatedByApp_ | 提供和管理此应用的通知。 | 允许应用代表登录用户提供其通知。 此外，还允许应用读取、更新和删除此应用的用户通知项目。 |否 |
### <a name="remarks"></a>注解
*Notifications.ReadWrite.CreatedByApp* 对 Microsoft 帐户和工作或学校帐户都有效。与此权限关联的 *CreatedByApp* 约束表明，服务将基于调用应用的标识(Microsoft 帐户应用 ID 或为跨平台应用程序标识配置的一组应用 ID)对结果应用隐式筛选。
### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委派
* _Notifications.ReadWrite.CreatedByApp_: 发布以用户为中心的通知，该通知之后可能会传递给在不同终结点上运行的用户的多个应用程序客户端。(POST /me/notifications/)。

---

## <a name="online-meetings-permissions"></a>联机会议权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
|_OnlineMeetings.Read_|读取联机会议。|允许应用代表已登录的用户读取联机会议的详细信息。|否|否|
|_OnlineMeetings.ReadWrite_|读取和创建联机会议。|允许应用代表已登录的用户创建和读取联机会议。 |否|否|
|_OnlineMeetingArtifact.Read.All_|读取联机会议项目。|允许应用代表已登录用户读取联机会议项目。 |否|否|

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
|_OnlineMeetings.Read.All_|从应用阅读联机会议详细信息 |允许应用在没有已登录用户的情况下读取组织中的联机会议详细信息。|是|
|_OnlineMeetings.ReadWrite.All_|从应用阅读联机会议详细信息|允许应用在没有已登录用户的情况下创建和读取联机会议。|是|
|_OnlineMeetingArtifact.Read.All_|从应用读取联机会议项目 |允许应用在没有已登录用户的情况下读取组织中的联机会议项目。|是|

> **重要** 管理员可以配置 [应用程序访问策略](cloud-communication-online-meeting-application-access-policy.md)以允许应用代表用户访问联机会议。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _OnlineMeetings.Read_：检索 [联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)的属性和关系 (`GET /beta/communications/onlinemeetings/{default id}`)。
* _OnlineMeetings.ReadWrite_：创建 [联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) (`POST /beta/communications/onlinemeetings`)。

#### <a name="application"></a>应用程序

* _OnlineMeetings.Read.All_
  * 检索[联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)的属性和关系 (`GET /beta/communications/onlinemeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'`)。
  * 代表用户检索[联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`GET /beta/users/{userId}/onlineMeetings/{id})
* _OnlineMeetings.ReadWrite.All_
  * 代表用户创建[联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`POST /beta/users/{userId}/onlineMeetings/)
  * 代表用户更新[联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`PATCH /beta/users/{userId}/onlineMeetings/{id})
  * 代表用户删除[联机会议](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) (`DELETE /beta/users/{userId}/onlineMeetings/{id})
  
> **注意**：创建 [联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true)时会代表用户创建一个会议，但不会在该用户的日历上显示该会议。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="on-premises-publishing-profiles-permissions"></a>本地发布配置文件权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| OnPremisesPublishingProfiles.ReadWrite.All |    访问本地发布配置文件| 允许应用通过代表已登录用户创建、查看、更新和删除本地发布的资源、本地代理和代理组来管理混合标识服务配置。 | 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| OnPremisesPublishingProfiles.ReadWrite.All |    访问本地发布配置文件| 允许应用通过代表已登录用户创建、查看、更新和删除本地发布的资源、本地代理和代理组来管理混合标识服务配置。 | 否 | 否 |

---

## <a name="openid-connect-oidc-permissions"></a>OpenID Connect （OIDC） 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _email_ |    查看用户的电子邮件地址 | 允许应用读取用户的主电子邮件地址。 | 否 | 否 |
| _offline_access_ |    随时访问用户数据 | 允许应用读取和更新用户数据，即使用户当前没有在使用此应用，也不例外。| 否 | 否 |
| _openid_ |    让用户登录 | 允许用户以其工作或学校帐户登录应用，并允许应用查看用户的基本个人资料信息。| 否 | 否 |
| _个人资料_ |    查看用户的基本个人资料 | 允许应用查看用户的基本个人资料（名称、图片、用户名称）。| 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="remarks"></a>注解
可以使用这些权限指定要在 Azure AD 授权和令牌请求中返回的项目。Azure AD v1.0 和 v2.0 终结点以不同的方式支持它们。

使用 Azure AD (v1.0) 终结点时，仅使用 _openid_ 权限。在授权请求的 *scope* 参数中指定它，以在使用 OpenID Connect 协议让用户登录应用时返回 ID 令牌。有关详细信息，请参阅 [使用 OpenID Connect 和 Azure Active Directory 来授权访问 Web 应用程序](/azure/active-directory/develop/active-directory-protocols-openid-connect-code)。若要成功返回 ID 令牌，还必须确保在注册应用时已配置 _User.Read_ 权限。

使用 Azure AD v2.0 终结点时，在 _scope_ 参数中指定 _offline\_access_ 权限，以在使用 OAuth 2.0 或 OpenID Connect 协议时显式请求获取刷新令牌。使用 OpenID Connect 时，指定 _openid_ 权限来请求获取 ID 令牌。还可指定 _email_ 权限和/或 _profile_ 权限，以在 ID 令牌中返回其他声明。使用 v2.0 终结点时，无需指定 _User.Read_ 来返回 ID 令牌。有关详细信息，请参阅 [OpenID Connect 作用域](/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes)。

> **重要说明**：目前，Microsoft 身份验证库 (MSAL) 默认在授权和令牌请求中指定 _offline\_access_、_openid_、_profile_ 和 _email_。也就是说，在默认情况下，如果显式指定这些权限，Azure AD 可能会返回错误。

---

## <a name="organization-permissions"></a>组织权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Organization.Read.All_ |读取组织信息 | 允许应用代表已登录用户读取组织和相关资源。 相关资源包括订阅的 SKU 和租户品牌信息等内容。|是 | 否 |
| _Organization.ReadWrite.All_ |读取和写入组织信息 | 允许应用代表已登录用户读取和写入组织和相关资源。 相关资源包括订阅的 SKU 和租户品牌信息等内容。 |是 | 否 |

<br/>

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Organization.Read.All_ |读取组织信息 | 允许应用在没有已登录用户的情况下读取组织和相关资源。 相关资源包括订阅的 SKU 和租户品牌信息等内容。 | 是 |
| _Organization.ReadWrite.All_ |读取和写入组织信息 | 允许应用在没有已登录用户的情况下读取和写入组织和相关资源。 相关资源包括订阅的 SKU 和租户品牌信息等内容。 |是 |


### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>Delegated

* _Organization.Read.All_：获取组织信息 (`GET /organization`)。
* _Organization.Read.All_：获取组织订阅的 SKU (`GET /subscribedSkus`)。

#### <a name="application"></a>应用程序

* _Organization.ReadWrite.All_：更新组织信息（例如 **technicalNotificationMails**）(`PATCH /organization/{id}`)。

---

## <a name="organizational-contact-permissions"></a>组织联系人权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _OrgContact.Read.All_ | 读取组织联系人|允许应用代表已登录用户读取所有组织联系人。 这些联系人由组织管理，不同于用户的个人联系人。|是 | 否 |

<br/>

#### <a name="application-permissions"></a>应用程序权限

|权限    |显示字符串   |说明 |需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _OrgContact.Read.All_ |读取组织联系人 | 允许应用在没有已登录用户的情况下读取所有组织联系人。  这些联系人由组织管理，不同于用户的个人联系人。 | 是 |

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>Delegated

* _OrgContact.Read.All_：获取所有组织联系人 (`GET /contacts`)。

---

## <a name="people-permissions"></a>People 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _People.Read_ |    读取用户的相关人员列表 | 允许应用读取登录用户相关人员的得分列表。该列表可包括当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。 | 否 | 是 |
| _People.Read.All_ | 读取所有用户的相关人员列表 | 允许应用读取登录用户或登录用户组织中的其他用户的相关人员得分列表。该列表可包括当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。此外，还允许应用搜索登录用户组织的整个目录。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read.All_ | 读取所有用户的相关人员列表 | 允许应用读取登录用户或登录用户组织中的其他用户的相关人员得分列表。 <br/><br/>该列表可以包括本地联系人、社交网络或组织目录的联系人以及来自最近通信（如电子邮件和 Skype）的人员。还允许应用搜索登录用户组织的整个目录。 | 是 |

### <a name="remarks"></a>备注

People.Read.All 权限仅适用于工作和学校帐户。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派
* _People.Read_：读取相关人员列表 (`GET /me/people`)
* _People.Read.All_：读取同一组织中与其他用户相关的人员列表 (`GET /users('{id})/people`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="privileged-access-permissions"></a>特权访问权限

#### <a name="delegated-permissions"></a>委派权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:---------- |:-------------- |:----------- |:---------------------- |:----------------- |
| _PrivilegedAccess.ReadWrite.AzureAD_ |为目录读取和写入 Privileged Identity Management 数据  | 允许应用读取和写入 Azure AD 的 Privileged Identity Management API。 | 是 | 否 |
| _PrivilegedAccess.ReadWrite.AzureADGroup_ |为特权范文组读取和写入 Privileged Identity Management 数据 | 允许应用读取和写入组的 Privileged Identity Management API 的权限。 | 是 | 否 |
| _PrivilegedAccess.ReadWrite.AzureResources_ |为 Azure 资源读取和写入 Privileged Identity Management 数据 | 允许应用读取和写入 Azure 资源的 Privileged Identity Management API。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 |
|:---------- |:-------------- |:----------- |:---------------------- |
| _PrivilegedAccess.Read.AzureAD_ |为目录读取 Privileged Identity Management 数据  | 允许应用读取 Azure AD 的 Privileged Identity Management API 的权限。 | 是 |
| _PrivilegedAccess.Read.AzureADGroup_ |读取特权访问组的 Privileged Identity Management 数据 | 允许应用读取组的 Privileged Identity Management API 的权限。 | 是 |
| _PrivilegedAccess.Read.AzureResources_ |读取 Azure 资源的 Privileged Identity Management 数据 | 允许应用读取 Azure AD 资源的 Privileged Identity Management API 的权限。 | 是 |

---

## <a name="places-permissions"></a>位置权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Place.Read.All_ |   读取所有公司位置 | 允许应用读取在 Exchange Online 中为租户设置的公司位置（会议室和房间列表）。 |是 | 否 |
| _Place.ReadWrite.All_ |   读取并写入所有公司位置 | 允许应用读取和写入在 Exchange Online 中为租户设置的公司位置（会议室和房间列表）。 |是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Place.Read.All_ |   读取所有公司位置 | 允许应用读取日历事件和其他应用程序的公司位置（会议室和房间列表）。| 是 |

---

## <a name="policy-permissions"></a>策略权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Policy.Read.All_ | 阅读你组织的策略 | 允许应用代表已登录用户阅读你组织的策略。 | 是 | 否 |
| _Policy.Read.PermissionGrant_ | 读取许可和权限授予策略 | 允许此应用代表已登录的用户读取与适用于应用程序的许可和权限授予相关的策略。 | 是 | 否 |
| _Policy.ReadWrite.AccessReview_ |   读取和写入组织的访问评审策略  | 允许应用代表已登录用户读取和写入你组织的访问评审策略。 | 是 | 否 |
| _Policy.ReadWrite.ApplicationConfiguration_ | 读取和写入组织的应用程序配置策略 | 允许应用代表已登录用户读取和写入组织的配置策略。 | 是 | 否 |
| _Policy.ReadWrite.AuthenticationFlows_ | 读取和写入你组织的身份验证流策略 | 允许应用代表已登录用户读取和写入身份验证流策略。 | 是 | 否 |
| _Policy.ReadWrite.AuthenticationMethod_        | 读取和写入身份验证方法策略       | 允许应用代表已登录用户读取和写入身份验证方法策略。 还必须为登录用户分配全局管理员角色。 | 是 | 否 |
| _Policy.ReadWrite.Authorization_ | 读取和写入组织的授权策略 | 允许应用代表已登录用户读取和写入你组织的授权策略。  例如，授权策略可以控制现有用户角色默认拥有的某些权限。 | 是 | 否 |
| _Policy.ReadWrite.ConditionalAccess_ | 读取和写入你组织的条件访问策略 | 允许应用代表已登录用户读取和写入你组织的条件访问策略。 | 是 | 否 |
| _Policy.ReadWrite.ConsentRequest_ | 读取和写入组织的同意请求策略 | 允许应用代表已登录用户读取和写入你组织的许可请求策略。 | 是 | 否 |
| _Policy.ReadWrite.CrossTenantAccess_ | 读取和写入组织的跨租户访问策略 | 允许应用代表已登录用户读取和写入组织的跨租户访问策略。 | 是 | 否 |
| _Policy.ReadWrite.FeatureRollout_ | 读取和写入你组织的功能推出策略 | 允许应用代表已登录用户读取和写入你组织的功能推出策略。 包括分配用户和组来推出特定功能以及删除此类用户和组的能力。 | 是 | 否 |
| _Policy.ReadWrite.PermissionGrant_ | 管理许可和权限授予策略 | 允许此应用代表已登录的用户管理与适用于应用程序的许可和权限授予相关的策略。 | 是 | 否 |
| _Policy.ReadWrite.TrustFramework_ | 读取和写入你组织的信任框架策略 | 允许应用代表已登录用户读取和写入你组织的信任框架策略。 | 是 | 否 |
| _Policy.ReadWrite.AuthenticationMethod_ | 读取和写入你组织的身份验证方法策略 | 允许应用代表已登录用户读取和写入身份验证方法策略。 | 是 | 否 |
| _Policy.ReadWrite.MobilityManagement_ | 读取和写入你组织的身份验证方法策略。 | 允许应用程序代表已登录用户读取和写入移动设备管理策略。 这些控制移动设备管理 (MDM) 和移动应用程序管理 (MAM) 应用程序的设置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Policy.Read.All_ | 阅读你组织的策略 | 允许应用无需登录的用户即可读取你所在组织的所有策略。 | 是 |
| _Policy.Read.PermissionGrant_ | 读取许可和权限授予策略 | 允许此应用没有登录用户的情况下读取与适用于应用程序的许可和权限授予相关的策略。 | 是 |
| _Policy.Read.ApplicationConfiguration_ | 读取组织的应用程序配置策略 | 允许应用在没有已登录用户的情况下读取组织的所有应用程序配置策略。 | 是 |
| _Policy.ReadWrite.AccessReview_ | 读取和写入组织的访问评审策略 | 允许应用无需登录的用户即可读取和写入你所在组织的访问评审策略。 | 是 |
| _Policy.ReadWrite.ApplicationConfiguration_ | 读取和写入组织的应用程序配置策略 | 允许应用在没有已登录用户的情况下读取和写入组织的所有应用程序配置策略。 | 是 |
| _Policy.ReadWrite.AuthenticationFlows_ | 读取和写入你组织的身份验证流策略 | 允许应用在没有已登录用户的情况下读取和写入所有租户身份验证流策略。 | 是 |
| _Policy.ReadWrite.Authorization_ | 读取和写入组织的授权策略 | 允许应用代表已登录用户读取和写入你组织的授权策略。  例如，授权策略可以控制现有用户角色默认拥有的某些权限。 | 是 | 
| _Policy.ReadWrite.ConsentRequest_ | 读取和写入组织的同意请求策略 | 允许应用在没有登录用户的情况下读取和写入你的组织的许可请求策略。 | 是 |
| _Policy.ReadWrite.CrossTenantAccess_ | 读取和写入组织的跨租户访问策略 | 允许应用在没有已登录用户的情况下读取和写入组织的跨租户访问策略。 | 是 |
| _Policy.ReadWrite.AuthenticationMethod_   | 读取和写入所有身份验证方法策略    | 允许应用在没有登录用户的情况下读取和写入所有租户身份验证方法策略。 | 是 |
| _Policy.ReadWrite.FeatureRollout_ | 读取和写入功能推出策略 | 允许用户无需登录的用户即可读取和写入功能推出策略。 包括分配用户和组来推出特定功能以及删除此类用户和组的能力。 | 是 |
| _Policy.ReadWrite.PermissionGrant_ | 管理许可和权限授予策略 | 允许此应用在没有登录用户的情况下管理与适用于应用程序的许可和权限授予相关的策略。 | 是 |
| _Policy.ReadWrite.TrustFramework_ | 读取和写入你组织的信任框架策略 | 允许应用无需登录的用户即可读取和写入你所在组织的信任框架策略。 | 是 |

### <a name="example-usage"></a>用法示例

以下用法对委派权限和应用程序权限均有效：

* _Policy.Read.All_ 读取你所在组织的策略 (`GET /policies`)
* _Policy.Read.All_ 读取你所在组织的信任框架策略 (`GET /beta/trustFramework/policies`)
* _Policy.Read.All_ 读取你所在组织的功能推出策略 (`GET /beta/directory/featureRolloutPolicies`)
* _Policy.ReadWrite.AccessReview_：读取和写入组织的访问评审策略 (`PATCH /beta/policies/accessReviewPolicy`)
* _Policy.ReadWrite.ApplicationConfiguration_：读取和写入组织的应用程序配置策略 (`POST /beta/policies/tokenLifetimePolicies`)
* _Policy.ReadWrite.AuthenticationFlows_：读取和写入你组织的身份验证流策略 (`PATCH /beta/policies/authenticationFlowsPolicy`)
* _Policy.ReadWrite.AuthenticationMethod_: 使用此权限管理身份验证方法策略的设置，包括启用和禁用身份验证方法、允许用户和组使用这些方法，以及配置与用户可在租户中注册和使用的身份验证方法相关的其他设置。
* _Policy.ReadWrite.ConditionalAccess_：读取和写入你组织的条件访问策略 (`POST /beta/identity/conditionalAccess/policies`)
* _Policy.ReadWrite.CrossTenantAccess_： 读取和写入组织的跨租户访问策略 （`PATCH /beta/policies/crossTenantAccessPolicy`）
* _Policy.ReadWrite.FeatureRollout_：读取和写入你组织的功能推出策略 (`POST /beta/directory/featureRolloutPolicies`)
* _Policy.ReadWrite.TrustFramework_：读取和写入你组织的信任框架策略 (`POST /beta/trustFramework/policies`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="presence-permissions"></a>状态权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Presence.Read_ | 读取用户的状态信息 | 允许应用代表已登录的用户读取状态信息。 状态信息包括活动、可用性、状态备注、日历外出邮件、时区和位置。 | 否 |
| _Presence.Read.All_ |   读取组织中所有用户的状态信息 | 允许应用代表已登录的用户读取目录中所有用户的状态信息。 状态信息包括活动、可用性、状态备注、日历外出邮件、时区和位置。 | 否 |
| _Presence.ReadWrite_ | 读取和写入用户的状态信息 | 允许应用代表已登录用户读取状态信息以及写入活动和可用性。 状态信息包括活动、可用性、状态备注、日历外出邮件、时区和位置。 | 是 |

#### <a name="application-permissions"></a>应用程序权限
|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Presence.ReadWrite.All_ | 读取和写入所有用户的状态信息 | 允许应用在没有登录用户的情况下读取目录中所有用户的所有状态信息以及写入活动和可用性。 状态信息包括活动、可用性、状态备注、日历外出邮件、时区和位置。 | 是 |

### <a name="example-usage"></a>用法示例

* _Presence.Read_：如果你已登录，则检索你自己的状态信息 (`GET /me/presence`)
* _Presence.Read.All_：检索其他用户的状态信息 (`GET /users/{id}/presence`)
* _Presence.Read.All_：检索多个用户的状态信息 (`POST /communications/getPresencesByUserId`)
* _Presence.ReadWrite_：
  * 如果已登录，请设置状态会话的状态（`POST /me/presence/setPresence`）
  * 如果已登录，请设置自己的首选状态（`POST /me/presence/setUserPreferredPresence`）
* _Presence.ReadWrite.All_：
  * 将用户的状态会话的状态设置为应用程序（`POST /users/{id}/presence/setPresence`）
  * 将用户的首选状态设置为应用程序（`POST /users/{id}/presence/setUserPreferredPresence`）

---

## <a name="programs-and-program-controls-permissions"></a>程序和程序控制权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ProgramControl.Read.All_ |   读取所有程序  | 允许应用代表已登录的用户读取程序。 | 是 | 否 |
| _ProgramControl.ReadWrite.All_ |   管理所有程序  | 允许应用代表已登录的用户读取和写入程序。 | 是 | 否 |


#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _ProgramControl.Read.All_ |   读取所有程序 | 允许应用在没有登录的用户的情况下读取程序。 | 是 |
| _ProgramControl.ReadWrite.All_ |   管理所有程序 | 允许应用在没有登录的用户的情况下读取和写入程序。 | 是 |

### <a name="remarks"></a>说明

_ProgramControl.Read.All_ 和 _ProgramControl.ReadWrite.All_ 仅对工作或学校帐户有效。

对于通过委派权限读取程序和程序控件的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员、安全管理员、安全读取者或用户管理员。 对于通过委派权限写入程序和程序控件的应用，登录的用户必须是以下管理员角色之一的成员：全局管理员、安全管理员、安全读取者或用户管理员。  若要详细了解管理员角色，请参阅[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

---

## <a name="reports-permissions"></a>报告权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Reports.Read.All_ | 读取所有使用情况报告 | 允许应用代表已登录的用户读取所有服务使用情况报告。提供使用情况报告的服务包括 Microsoft 365 和 Azure Active Directory。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Reports.Read.All_ | 读取所有使用情况报告 | 允许应用在没有登录用户的情况下读取所有服务使用情况报告。提供使用情况报告的服务包括 Microsoft 365 和 Azure Active Directory。 | 是 |

### <a name="remarks"></a>注解
- 这些报告权限仅对工作或学校帐户有效。
- 若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配的 Azure AD 受限管理员角色。有关更多详细信息，请参阅[ API 授权，读取 Microsoft 365使用情况报告](reportroot-authorization.md)。

### <a name="example-usage"></a>用法示例

#### <a name="application"></a>应用程序

* _Reports.Read.All_：读取电子邮件应用程序在 7 天内的使用情况详情报告 (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`)。
* _Reports.Read.All_：读取电子邮件在日期“2017-01-01”的的活动详情报告 (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`)。
* _Reports.Read.All_：读取 Microsoft 365 激活详情报告 (`GET /reports/Office365Activations(view='Detail')/content`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="role-management-permissions"></a>角色管理权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _RoleAssignmentSchedule.Read.Directory_ | 读取公司目录中所有活动的角色分配。 | 允许应用代表已登录的用户读取公司目录中活动的基于角色的访问控制 (RBAC) 分配。这包括读取目录角色模板和目录角色。 | 是 | 否 |
| _RoleEligibilitySchedule.Read.Directory_ | 读取公司目录中所有符合条件的角色分配。 | 允许应用代表已登录的用户读取公司目录中符合条件的基于角色的访问控制 (RBAC) 分配。这包括读取目录角色模板和目录角色。 | 是 | 否 |
| _RoleManagement.Read.All_ | 读取所有 RBAC 提供程序的角色管理数据。 | 允许应用代表登录用户读取所有受支持的[ RBAC 提供程序](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true)基于角色的访问控制 (RBAC) 设置。这包括读取角色和角色分配。 | 是 | 否 |
| _RoleManagement.Read.Directory_ | 读取 Azure AD 的角色管理数据。 | 允许应用代表已登录的用户读取公司目录的基于角色的访问控制 (RBAC) 设置。这包括读取目录角色模板、目录角色和成员身份。 | 是 | 否 |
| _RoleManagementPolicy.Read.Directory_ | 读取公司目录中所有特权角色分配的策略。 | 允许应用代表已登录的用户读取公司目录中具有特权的基于角色的访问控制 (RBAC) 分配策略。 | 是 | 否 |
| _RoleAssignmentSchedule.ReadWrite.Directory_ | 读取、更新和删除公司目录中所有活动的角色分配。 | 允许应用代表已登录用户读取和管理公司目录中活动的基于角色的访问控制 （RBAC） 分配。这包括管理目录角色成员身份，以及阅读目录角色模板、目录角色和活动的成员身份。 | 是 | 否 |
| _RoleEligibilitySchedule.ReadWrite.Directory_ | 读取、更新和删除公司目录中所有符合资格的角色分配。 | 允许应用代表登录用户阅读和管理您公司目录基于角色的访问控制 （RBAC） 分配。这包括发送目录角色和管理目录角色成员身份，以及阅读目录角色模板、目录角色和成员身份。 | 是 | 否 |
| _RoleManagement.ReadWrite.Directory_ | 读取和写入 Azure AD 的角色管理数据。 | 允许应用代表登录用户阅读和管理您公司目录基于角色的访问控制 （RBAC） 设置。这包括发送目录角色和管理目录角色成员身份，以及阅读目录角色模板、目录角色和成员身份。 | 是 | 否 |
| _RoleManagementPolicy.ReadWrite.Directory_ | 读取、更新和删除公司目录中所有特权角色分配的策略。 | 允许应用代表已登录的用户读取和管理公司目录的基于角色的访问控制 (RBAC) 分配。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _RoleManagement.Read.All_ | 读取所有 RBAC 提供程序的角色管理数据。 | 允许应用在没有登录用户的情况下读取所有受支持的[ RBAC 提供程序](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true)基于角色的访问控制 (RBAC) 设置。 | 是 |
| _RoleManagement.Read.Directory_ | 读取 Azure AD 的角色管理数据。 | 允许应用代表已登录的用户读取公司目录的基于角色的访问控制 (RBAC) 设置。这包括读取目录角色模板、目录角色和成员身份。 | 是 |
| _RoleManagement.ReadWrite.Directory_ | 读取和写入 Azure AD 的角色管理数据。 | 允许应用无需登录用户即可读取和管理公司目录基于角色的访问控制 (RBAC) 设置。这包括发送目录角色和管理目录角色成员身份，以及读取目录角色模板、目录角色和成员身份。 | 是 |


### <a name="remarks"></a>说明

> [!CAUTION]
> 允许授予授权的权限（如 _RoleManagement.ReadWrite.Directory_）允许应用程序授予自身、其他应用程序或任何用户的其他权限。在授予这些权限中的任何一项时，请小心。

使用 _RoleManagement.Read.Directory_ 权限，应用程序可以读取 directoryRoles 和 directoryRoleTemplates。 这包括读取目录角色的成员身份信息。

使用 _RoleManagement.ReadWrite.Directory_ 权限，应用程序可以读取和写入 directoryRoles（directoryRoleTemplates 是只读资源）。 这包括向目录角色添加成员和从目录角色中删除成员。

角色管理权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

- _RoleManagement.Read.Directory_：读取可用角色模板列表 (`GET /directoryRoleTemplates`)
- _RoleManagement.Read.Directory_：读取你的目录中已激活角色的列表 (`GET /directoryRoles`)
- _RoleManagement.Read.Directory_：读取某一角色的成员列表 (`GET /directoryRoles/<id>/members`)
- _RoleManagement.Read.Directory_：读取某一角色的管理单元范围的成员列表 (`GET /directoryRoles/<id>/scopedMembers`)
- _RoleManagement.ReadWrite.Directory_：激活来自角色模板的目录角色 (`POST /directoryRoles`)
- _RoleManagement.ReadWrite.Directory_：将成员添加到目录角色 (`POST /directoryRoles/<id>/members`)
- _RoleManagement.ReadWrite.Directory_：将管理单元范围的成员添加到目录角色 (`POST /directoryRoles/<id>/scopedMembers`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="schedule-management-permissions-private-preview"></a>计划管理权限（[个人预览版](#permissions-availability-status)）

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Schedule.ReadWrite.All_（个人预览版）| 读写班次服务 (Teams) 数据 | 允许应用在用户未登录的情况下读写班次应用程序中的计划、计划组、班次和关联的实体。| 是 | 否 |
| _Schedule.Read.All_（个人预览版）| 读取班次服务 (Teams) 数据 | 允许应用在用户未登录的情况下读取班次应用程序中的计划、计划组、班次和关联的实体。  | 是 | 否 |

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _Schedule.ReadWrite.All_ | 读写班次服务 (Teams) 数据 | 允许应用代表登录用户读取和写入班次应用中的日程安排、日程分组、班次和相关实体。| 否 | 否 |
| _Schedule.Read.All_ | 读取班次服务 (Teams) 数据 | 允许应用代表登录用户读取班次应用中的日程安排、日程分组、班次和相关实体。  | 否 | 否 |
| _WorkforceIntegration.ReadWrite.All_（个人预览版）| 对员工集成执行读取和写入操作 | 允许应用代表登录用户管理员工集成，将来自 Microsoft Teams Shifts 的数据与集成系统同步。  | 是 | 否 |
| _WorkforceIntegration.Read.All_（个人预览版）| 对员工集成执行读取和写入操作 | 允许应用代表登录用户管理员工集成，将来自 Microsoft Teams Shifts 的数据与集成系统同步。  | 是 | 否 |

## <a name="search-permissions"></a>搜索权限

#### <a name="application-permissions"></a>应用程序权限
|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ExternalConnection.ReadWrite.OwnedBy_ | 读取和写入外部连接和连接设置 | 允许应用在没有已登录用户的情况下读取和写入外部连接及其设置。 应用只能读取和写入其授权的外部连接，也可以创建新的外部连接。 | 是 | 否 |
| _ExternalItem.ReadWrite.OwnedBy_ | 读取和写入外部项目 | 允许应用在没有已登录用户的情况下读取和写入外部项目。 应用只能读取获得授权的连接的外部项目。 | 是 | 否 |
| _ExternalItem.ReadWrite.All_ | 读取和写入所有外部项目 | 允许应用在没有已登录用户的情况下读取和写入所有外部项目。 | 是 | 否 |

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _ExternalItem.Read.All_ | 读取外部数据 | 允许应用查询使用 Microsoft Graph 引入的数据| 是 | 否 |

### <a name="remarks"></a>注解
搜索权限仅对工作或学校帐户有效。

此搜索权限仅适用于通过索引 API 引入的数据。

通过搜索访问数据需要对项目具有读取权限。 示例：_Files.Read.All_ 用于通过搜索访问文件。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _ExternalItem.Read.All_：通过 [搜索 API](/graph/api/resources/search-api-overview) (`POST /search/query`) 访问外部数据。

---

## <a name="search-configuration-permissions"></a>搜索配置权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:-----------------------|
| _SearchConfiguration.Read.All_ | 读取组织的搜索配置 | 允许应用代表已登录用户读取搜索配置。 | 是 | 否 |
| _SearchConfiguration.ReadWrite.All_ | 读取和写入组织的搜索配置 | 允许应用代表已登录用户读取和写入搜索配置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限
|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 
|:----------------|:------------------|:-------------|:-----------------------|
| _SearchConfiguration.Read.All_ | 读取组织的搜索配置 | 允许应用在没有登录用户的情况下读取搜索配置。 | 是 | 
| _SearchConfiguration.ReadWrite.All_ | 读取和写入组织的搜索配置 | 允许应用在没有登录用户的情况下读取和写入搜索配置。 | 是 | 


### <a name="remarks"></a>说明
搜索配置权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated-and-application"></a>委派和应用程序

- _SearchConfiguration.Read.All_： 读取为租户创建的所有书签的列表 （`GET /beta/search/bookmarks`）
- _SearchConfiguration.ReadWrite.All_： 更新或读取为租户创建的所有书签 （`PATCH /beta/search/bookmarks/{id}`）

---

## <a name="security-permissions"></a>安全权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _SecurityEvents.Read.All_        |  读取组织的安全事件 | 允许应用代表已登录用户读取组织的安全事件。 | 是  | 否 |
| _SecurityEvents.ReadWrite.All_   | 读取和更新组织的安全事件。 | 允许应用代表已登录用户读取组织的安全事件。 还允许应用代表已登录用户更新安全事件中的可编辑属性。 | 是  | 否 |
| _SecurityActions.Read.All_        |  读取组织的安全措施 | 允许应用代表登录的用户读取组织的安全措施。 | 是  | 否 |
| _SecurityActions.ReadWrite.All_   | 读取和更新组织的安全措施 | 允许应用代表登录的用户读取或更新组织的安全措施。  | 是  | 否 |
| _ThreatIndicators.ReadWrite.OwnedBy_   | 管理此应用创建或拥有的威胁指标 |允许应用代表已登录的用户创建威胁指标和完全管理这些威胁指标（阅读、更新和删除）。  | 是  | 否 |
| _ThreatIndicators.Read.All_   | 读取组织的威胁指示器 | 允许应用代表已登录的用户读取组织的所有威胁指示器。  | 是  | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _SecurityEvents.Read.All_        |  读取组织的安全事件 | 允许应用读取组织的安全事件。 | 是  |
| _SecurityEvents.ReadWrite.All_   | 读取和更新组织的安全事件。 | 允许应用读取组织的安全事件。 还允许应用更新安全事件中的可编辑属性。 | 是  |
| _SecurityActions.Read.All_        |  读取组织的安全事件 | 允许应用读取组织的安全措施。 | 是  |
| _SecurityActions.ReadWrite.All_   | 创建和读取组织的安全措施 | 允许应用读取或创建安全措施，无需已登录用户。 | 是  |
| _ThreatIndicators.ReadWrite.OwnedBy_   | 管理此应用创建或拥有的威胁指标 | 允许应用创建威胁指标，并完全管理这些威胁指标（阅读、更新和删除），无需已登录用户。  它无法删除其不拥有的任何威胁指标。 | 是  |
| _ThreatIndicators.Read.All_   | 管理此应用创建或拥有的威胁指标 | 允许应用在没有登录用户的情况下读取组织的所有威胁指示器。 | 是  |

### <a name="remarks"></a>说明

安全权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated-and-application"></a>委派和应用程序

- _SecurityEvents.Read.All_：从对租户可用的所有许可安全提供程序中读取所有安全警报的列表 (`GET /beta/security/alerts`)
- _SecurityEvents.ReadWrite.All_：更新或读取对租户可用的所有许可安全提供程序中的安全警报 (`PATCH /beta/security/alerts/{id}`)

---

## <a name="service-communications-permissions"></a>服务通信权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串  | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ServiceHealth.Read.All_ | 读取服务运行状况 | 允许此应用代表登录用户读取租户的服务运行状况信息。 服务运行状况信息可能包括服务问题或服务运行状况概述。 | 是 | 是 |
| _ServiceMessage.Read.All_ | 读取服务消息 | 允许此应用代表已登录的用户读取租户的服务公告消息。 消息可能包含有关新增或已更改功能的信息。 | 是 | 是 |
| _ServiceMessageViewpoint.Write_ | 在服务公告中更新用户状态 | 允许应用代表登录的用户更新服务公告消息的用户状态。 消息状态可以标记为已读、存档或收藏。 | 是 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串  | 说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _ServiceHealth.Read.All_ | 读取服务运行状况 | 允许此应用在没有已登录用户的情况下读取租户的服务运行状况信息。 服务运行状况信息可能包括服务问题或服务运行状况概述。 | 是 |
| _ServiceMessage.Read.All_ | 读取服务消息 | 允许此应用在没有已登录用户的情况下读取租户的服务公告消息。 消息可能包含有关新增或已更改功能的信息。 | 是 |

---

## <a name="short-notes-permissions-private-preview"></a>简短注释权限（[个人预览版](#permissions-availability-status)）

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串  | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ShortNotes.Read_ | 阅读已登录用户的简短注释 | 允许应用读取登录用户有权访问的所有简短注释。 | 否 | 是 |
| _ShortNotes.ReadWrite_ | 阅读、创建、编辑和删除已登录用户的简短注释 | 允许应用阅读、创建、编辑和删除已登录用户的简短注释。 | 否 | 是 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _ShortNotes.Read.All_ | 阅读所有用户的简短注释 | 允许应用在没有已登录用户的情况下读取所有简短注释。 | 是 |
| _ShortNotes.ReadWrite.All_ | 阅读、创建、编辑和删除所有用户的简短注释 | 允许应用阅读、创建、编辑和删除已登录用户的所有简短注释。 | 是 |

---

## <a name="sites-permissions"></a>站点权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Sites.Read.All_        | 读取所有网站集中的项目 | 允许应用代表登录用户读取文档，并列出所有网站集中的项目。 | 否  | 否 |
| _Sites.ReadWrite.All_   | 读取和写入所有网站集中的项目 | 允许应用代表登录用户编辑或删除所有网站集中的文档和列表项。 | 否  | 否 |
| _Sites.Manage.All_      | 创建、编辑和删除所有网站集中的项目和列表 | 允许应用代表登录用户管理和创建所有网站集中的列表、文档和列表项。 | 否 | 否 |
| _Sites.FullControl.All_ | 完全控制所有网站集 | 允许应用代表登录用户具有对所有网站集中的 SharePoint 网站的完全控制权限。  | 是  | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Sites.Read.All_        | 读取所有网站集中的项目 | 允许应用在没有登录用户的情况下读取所有网站集中的文档和列表项。 | 是 |
| _Sites.ReadWrite.All_   | 读取和写入所有网站集中的项目 | 允许应用在没有登录用户的情况下创建、读取、更新和删除所有网站集中的文档和列表项。 | 是 |
| _Sites.Manage.All_      | 创建、编辑和删除所有网站集中的项目和列表 | 允许应用在没有登录用户的情况下管理和创建所有网站集中的列表、文档和列表项。  | 是  |
| _Sites.FullControl.All_ | 完全控制所有网站集 | 允许应用在没有登录用户的情况下具有对所有网站集中的 SharePoint 网站的完全控制权限。  | 是  |
| _Sites.Selected_ | 访问已选中的网站集 | 允许应用程序在不登录用户的情况下访问网站集的子集。  将在 SharePoint Online 中配置特定网站集和已授予的权限。 | 是  |


### <a name="remarks"></a>注解

站点权限仅对工作或学校帐户有效。
_Sites.Selected_ 应用程序权限仅在 Microsoft Graph API 中可用。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _Sites.Read.All_：读取 SharePoint 根网站上的列表 (`GET /v1.0/sites/root/lists`)
* _Sites.ReadWrite.All_：在 SharePoint 列表中新建列表项 (`POST /v1.0/sites/root/lists/123/items`)
* _Sites.Manage.All_：将新列表添加到 SharePoint 网站 (`POST /v1.0/sites/root/lists`)
* _Sites.FullControl.All_：对 SharePoint 网站和列表的完全访问权限。

---

## <a name="subject-rights-request-permissions"></a>主体权利请求权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
SubjectRightsRequest.Read.All | 读取主体权利请求 | 允许应用代表已登录用户读取主体权利请求。 | 是 | 否 |
SubjectRightsRequest.ReadWrite.All | 读取和写入主体权利请求 | 允许应用代表已登录用户读取和写入主体权利请求。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限
无。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>Delegated
- SubjectRightsRequest.Read.All_：获取可供用户 (`GET /privacy/subjectrightsrequests`) 使用的主体权利请求列表。
- _SubjectRightsRequest.ReadWrite.All_：创建主体权利请求 (`POST /privacy/subjectrightsrequests`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

## <a name="tasks-permissions"></a>任务权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Tasks.Read_ | 读取用户的任务和任务列表（预览版） | 允许该应用读取已登录用户的任务和任务列表，包括与用户共享的任何内容。 不包括创建、删除或更新任何内容的权限。 | 否 | 是 |
| _Tasks.Read.Shared_ | 读取用户任务和共享任务（预览版） | 允许应用读取用户有权访问的任务，包括用户个人任务和共享任务。 | 否 | 否 |
| _Tasks.ReadWrite_ | 创建、读取、更新和删除用户的任务和任务列表（预览版） | 允许该应用创建、读取、更新和删除已登录用户的任务和任务列表，包括与用户共享的任何内容。 | 否 | 是 |
| _Tasks.ReadWrite.Shared_ | 读取和写入用户任务和共享任务（预览版） | 允许应用创建、读取、更新和删除用户有权访问的任务，包括用户个人任务和共享任务。 | 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

无。

### <a name="remarks"></a>注解
_任务_ 权限用于控制对待办事项任务和 Outlook 任务（已弃用）的访问权限。Microsoft Planner 任务的访问权限由 [_组_ 权限](#group-permissions)控制。

目前仅工作或学校帐户支持 _共享_ 权限。即使具有 _共享_ 权限，如果未授予拥有共享内容的用户在文件夹内修改内容访问用户权限，读取和写入仍会失败。

### <a name="example-usage"></a>用法示例
#### <a name="delegated"></a>委派

* _Tasks.Read_：获取用户邮箱中的所有任务 (`GET /me/outlook/tasks`)。
* _Tasks.Read.Shared_：在文件夹中访问组织中其他用户与你共享的任务 (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`)。
* _Tasks.ReadWrite_：将事件添加到用户的默认任务文件夹 (`POST /me/outlook/tasks`)。
* _Tasks.Read_：获取用户邮箱中的所有未完成任务 (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`)。
* _Tasks.ReadWrite_：更新用户邮箱中的任务 (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`)。
* _Tasks.ReadWrite.Shared_：代表其他用户完成任务 (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="taxonomy-permissions"></a>分类权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TermStore.Read.All_        | 读取术语库数据 | 允许应用读取术语库中的各种术语、集和组 | 是  | 否 |
| _TermStore.ReadWrite.All_   | 读取和写入所有术语库数据 | 允许应用在术语库中编辑或删除术语、集和组 | 是  | 否 |

### <a name="remarks"></a>注解

分类权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>Delegated

* _TermStore.Read.All_：读取租户的 termStore（`GET /termStore`）
* _TermStore.ReadWrite.All_：在 termStore 中创建新术语（`POST /termStore/sets/123/children`）

---

## <a name="teams-permissions"></a>Teams 权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | 读取团队的名称和说明 | 代表已登录用户读取团队的名称和说明。  | 否 | 否 |
| _Team.Create_  | 创建团队 | 代表已登录用户创建团队。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限 

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | 获取所有团队列表 | 在没有用户登录的情况下获取所有团队列表。   | 是 | 否 |
| _Team.Create_  | 创建团队 | 在没有用户登录的情况下创建团队。 | 是 | 否 |
| _团队合作。迁移。所有_|管理迁移到 Microsoft Teams|创建和管理用于迁移到 Microsoft Teams 的资源|是|是|

## <a name="team-settings-permissions"></a>团队设置权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.All_ | 读取团队设置 | 代表已登录用户读取此团队的设置。  | 是 | 否 |
| _TeamSettings.ReadWrite.All_ | 读取和更改团队的设置 | 代表已登录用户读取和更改所有团队的设置。    | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.All_ | 读取所有团队设置 | 在没有登录用户的情况下读取此团队的设置。 | 是 | 否 |
| _TeamSettings.ReadWrite.All_ | 读取和更改所有团队的设置。 | 在没有登录用户的情况下读取和更改所有团队的设置。  | 是 | 否 |

## <a name="teams-activity-permissions"></a>Teams 活动权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsActivity.阅读_ （[专用预览](#permissions-availability-status)） | 读取用户的团队合作活动源 | 允许应用读取登录用户的团队合作活动源。 | 否 | 否 |
| _TeamsActivity.Send_ | 以用户身份发送团队合作活动 | 允许应用在用户的团队合作活动源中代表已登录的用户创建新的通知。 这些通知不可发现、需要遵从或受合规性策略控制。 | 否 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsActivity.Read.all_ （[专用预览](#permissions-availability-status)） | 读取所有用户的团队合作活动源 | 允许应用在没有登录用户的情况下读取所有用户的团队合作活动源。 | 是 | 否 |
| _TeamsActivity.Send_ | 向任何用户发送团队合作活动。 | 允许应用在未登录用户的情况下，在用户的团队合作活动源中创建新通知。 这些通知不可发现、需要遵从或受合规性策略控制。 | 是 | 否 |

## <a name="teams-app-permissions-deprecated"></a>Teams 应用权限 （不推荐使用）

>[!NOTE]
>这些权限已弃用。 改为使用等效的 TeamsAppInstallation.\*.All 权限。

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsApp.Read.All_ (**Deprecated**)| 读取所有安装的 Teams 应用 | 允许应用读取为已登录用户安装的 Teams 应用以及该用户所属的所有团队中的相关应用。不允许读取应用程序特定的设置。 | 是 | 否 |
| _TeamsApp.ReadWrite.All_ (**Deprecated**)| 管理所有 Teams 应用 | 允许应用代表已登录的用户以及该用户所属团队来读取、安装、升级和卸载 Teams 应用。不允许读取或写入应用程序特定的设置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsApp.Read.All_ (**Deprecated**)| 读取所有用户已安装的 Teams 应用 | 允许应用读取为任何用户安装的 Teams 应用，而无需登录用户。不提供读取应用程序特定设置的能力。 | 是 | 否 |
| _TeamsApp.ReadWrite.All_ (**Deprecated**)| 管理所有用户的 Teams 应用  | 允许应用读取、安装、升级和卸载任何用户的 Teams 应用，而无需登录用户。不提供读取或写入应用程序特定设置的能力。   | 是 | 否 |

## <a name="teams-app-installation-permissions"></a>Teams 应用安装权限

#### <a name="delegated-permissions"></a>委派权限
|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsAppInstallation.ReadForUser_  | 读取用户已安装的 Teams 应用| 允许应用读取为登录用户安装的 Teams 应用。不提供读取应用程序特定设置的能力。| 否 | 否 |
| _TeamsAppInstallation.ReadWriteForUser_ | 管理用户安装的 Teams 应用| 允许应用读取、安装、升级和卸载为已登录的用户安装的 Teams 应用。不提供读取应用程序特定设置的能力。| 是 | 否 |
| _TeamsAppInstallation.ReadWriteSelfForUser_ | 允许应用在 Teams 中管理其自身| 允许 Teams 应用为已登录用户可以访问的团队读取、安装、更新和卸载其自身。| 否 | 否 |
| _TeamsAppInstallation.ReadForTeam_ | 读取团队中已安装的 Teams 应用| 允许应用阅读已登录的用户可以访问的团队中安装的 Teams 应用。不提供读取应用程序特定设置的能力。| 是 | 否 |
| _TeamsAppInstallation.ReadWriteForTeam_ | 管理团队中已安装的 Teams 应用| 允许应用在已登录的用户可以访问的团队中读取、安装、升级和卸载 Teams 应用。不提供读取应用程序特定设置的能力。| 是 | 否 |
| _TeamsAppInstallation.ReadWriteSelfForTeam_ | 允许应用在 Teams 中管理其自身| 允许 Teams 应用为已登录用户可以访问的团队读取、安装、更新和卸载其自身。| 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限
|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _TeamsAppInstallation.ReadForUser.All_ | 读取为所有用户安装的 Teams 应用| 允许应用读取为任何用户安装的 Teams 应用，而无需登录用户。不提供读取应用程序特定设置的能力。| 是 |
| _TeamsAppInstallation.ReadWriteForUser.All_ | 管理所有用户的 Teams 应用| 允许应用读取、安装、升级和卸载任何用户的 Teams 应用，而无需登录用户。不提供读取应用程序特定设置的能力。| 是 |
| _TeamsAppInstallation.ReadWriteSelfForUser.All_  | 允许应用为所有用户管理其自身| 允许 Teams 应用在没有登录用户的情况下为任何用户读取、安装、更新和卸载其自身。| 是 |
| _TeamsAppInstallation.ReadForTeam.All_ | 读取为所有团队安装的 Teams 应用| 允许应用读取任何团队中安装的 Teams 应用，而无需登录用户。不提供读取应用程序特定设置的能力。| 是 |
| _TeamsAppInstallation.ReadWriteForTeam.All_ | 管理所有团队的 Teams 应用| 允许应用在没有登录用户的情况下读取、安装、更新和卸载任何团队中的 Teams 应用。不允许读取特定于应用程序的设置。| 是 |
| _TeamsAppInstallation.ReadWriteSelfForTeam.All_ | 允许 Teams 应用为所有团队管理其自身| 允许 Teams 应用在没有登陆用户的情况下在任何团队中读取、安装、更新和卸载其自身。| 是 |

## <a name="teams-device-management-permissions"></a>Teams 设备管理权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkDevice.Read.All_ | 读取 Teams 设备。 | 允许应用代表已登录用户读取 Teams 设备的管理数据。   | 是 | 否 |
| _TeamworkDevice.ReadWrite.All_ | 读取和写入 Teams 设备。 | 允许应用代表已登录用户读取和写入 Teams 设备的管理数据。  | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkDevice.Read.All_ | 读取 Teams 设备。 | 允许应用在没有登录用户的情况下读取 Teams 设备的管理数据。 | 是 | 否 |
| _TeamworkDevice.ReadWrite.All_ | 读取和写入 Teams 设备。 | 允许应用在没有登录用户的情况下读取和写入 Teams 设备的管理数据。 | 是 | 否 |

## <a name="team-member-permissions"></a>团队成员权限 

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamMember.Read.All_ | 读取团队的成员。 | 代表已登录的用户读取团队的成员。 | 是 | 否 |
| _TeamMember.ReadWrite.All_ | 从团队中添加和删除成员。 | 代表已登录用户从团队中添加和删除成员。 还允许更改成员的角色，例如从所有者到非所有者。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamMember.Read.All_ | 读取所有团队的成员。 | 在没有用户登录的情况下读取所有团队的成员。 | 是 | 否 |
| _TeamMember.ReadWrite.All_ | 从所有团队中添加和删除成员。 | 在没有用户登录的情况下从所有团队中添加和删除成员。 还允许更改团队成员的角色，例如从所有者到非所有者。 | 是 | 否 |

## <a name="team-resource-specific-consent-permissions"></a>团队资源特定的同意权限

#### <a name="application-permissions"></a>应用程序权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamSettings.Read.Group_ | 读取此团队设置。 | 在没有登录用户的情况下读取此团队的设置。 |否 | 否 |
| _TeamSettings.ReadWrite.Group_ | 更新此团队的设置。 | 在没有登录用户的情况下读取和编写此团队的设置。 |否 | 否 |
| _ChannelSettings.Read.Group_ | 读取此团队频道的名称、说明和设置。 | 在没有登录用户的情况下读取此团队的频道名称、频道说明和频道设置。 |否 | 否 |
| _ChannelSettings.ReadWrite.Group_ | 更新此团队频道的名称、说明和设置。| 在没有登录用户的情况下更新此团队的频道名称、频道说明和频道设置。 |否 | 否 |
| _Channel.Create.Group_ | 在这个团队中创建频道。 | 在没有登录用户的情况下在此团队中创建频道。 |否 | 否 |
| _Channel.Delete.Group_ | 删除此团队的频道。 | 在没有登录用户的情况下删除此团队的频道。 |否 | 否 |
| _ChannelMessage.Read.Group_ | 读取团队频道消息。 | 允许应用在没有登录用户的情况下读取此团队的频道消息。 |否 | 否 |
| _TeamsAppInstallation.Read.Group_ | 查看此团队中已安装的应用。 | 在没有登录用户的情况下查看此团队中安装的应用。 |否 | 否 |
| _TeamsTab.Read.Group_ | 读取此团队的选项卡。 | 在没有登录用户的情况下读取此团队的选项卡。 |否 | 否 |
| _TeamsTab.Create.Group_ | 在此团队中创建选项卡。 | 在没有登录用户的情况下在此团队中创建选项卡。 |否 | 否 |
| _TeamsTab.ReadWrite.Group_ | 更新此团队的选项卡。 | 在没有登录用户的情况下更新此团队的选项卡。 |否 | 否 |
| _TeamsTab.Delete.Group_ | 删除此团队的选项卡。 | 在没有登录用户的情况下删除此团队的选项卡。 |否 | 否 |
| _TeamMember.Read.Group_ | 读取此团队的成员。 | 在没有已登录用户的情况下读取此团队的成员。 |否 | 否 |
| _Member.Read.Group_ | 读取此组的成员。| 在没有已登录用户的情况下读取此团队的成员。 |否 | 否 |
| _Owner.Read.Group_| 读取此组的所有者。 | 在没有已登录用户的情况下读取此团队的所有者。 |否 | 否 |
| _File.Read.Group_| 读取此团队的文件和文件夹。 | **有限支持** <br/> （预览）在没有登录用户的情况下读取此团队的文件和文件夹。 | 否 | 否 |
| _TeamsActivity.Send.Group_| 向此团队中的用户发送活动源通知。 | 允许应用在没有登录用户的情况下，在此团队中用户的团队合作活动源中创建新通知。 | 否 | 否 |

## <a name="teams-settings-permissions"></a>Teams 设置权限

### <a name="delegated-permissions"></a>委派权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | 读取团队的名称和说明| 代表已登录用户读取团队的名称和说明。|否| 否 |
| _TeamSettings.Read.All_ | 读取团队设置| 代表已登录用户读取所有团队的设置。|是| 否 |
| _TeamSettings.ReadWrite.All_ | 读取和更改团队的设置。| 代表已登录用户读取和更改所有团队的设置。|是| 否 |

### <a name="application-permissions"></a>应用程序权限

| 权限 | 显示字符串 | 说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Team.ReadBasic.All_ | 获取所有团队列表。| 在没有用户登录的情况下获取所有团队列表。|是| 否 |
| _TeamSettings.Read.All_ | 读取所有团队设置| 在没有登录用户的情况下读取此团队的设置。|是| 否 |
| _TeamSettings.ReadWrite.All_ | 读取和更改所有团队的设置| 在没有登录用户的情况下读取和更改所有团队的设置。|否 | 否 |

## <a name="teams-tab-permissions"></a>Teams 选项卡权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsTab.Read.All_ | 读取 Microsoft Teams 中的选项卡。 | 允许应用读取为已登录用户安装的 Teams 应用以及该用户所属的所有团队中的相关应用。不允许读取应用程序特定的设置。 | 是 | 否 |
| _TeamsTab.ReadWrite.All_ | 读取和写入 Microsoft Teams 中的选项卡。 | 允许应用代表已登录的用户以及该用户所属团队来读取、安装、升级和卸载 Teams 应用。不允许读取或写入应用程序特定的设置。    | 是 | 否 |
| _TeamsTab.Create_ | 在Microsoft Teams 中创建选项卡。 | 允许应用代表已登录的用户在 Microsoft Teams 中的任何团队内创建选项卡。 这不会授予在选项卡创建后读取、修改或删除这些选项卡的权限，也不会授予访问选项卡中的内容的权限。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamsTab.Read.All_ | 读取 Microsoft Teams 中的选项卡。 | 在没有登录用户的情况下，读取 Microsoft Teams 中任何团队内的选项卡的名称和设置。 这不会授予访问选项卡中的内容的权限。 | 是 | 否 |
| _TeamsTab.ReadWrite.All_ | 读取和写入 Microsoft Teams 中的选项卡。 | 在没有登录用户的情况下读取和写入 Microsoft Teams 中任何团队内的选项卡。 这不会授予访问选项卡中的内容的权限。 | 是 | 否 |
| _TeamsTab.Create_ | 在Microsoft Teams 中创建选项卡。 | 允许用户在没有登录用户的情况下在 Microsoft Teams 中的任何团队内创建选项卡。 这不会授予在选项卡创建后读取、修改或删除这些选项卡的权限，也不会授予访问选项卡中的内容的权限。 | 是 | 否 |

## <a name="teams-tag-permissions"></a>Teams 标记权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkTag.ReadWrite_| 读取和写入 Microsoft Teams 中的标记。 | 允许应用代表已登录的用户在 Teams 中读取和写入标签。   | 是 | 否 |
| _TeamworkTag.Read_ | 读取 Microsoft Teams 中的标记。 | 允许应用代表已登录的用户在 Teams 中读取标签。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _TeamworkTag.ReadWrite.All_| 读取和写入 Microsoft Teams 中的标记。 | 允许应用在没有登录的用户的情况下读取和写入 Teams 中的标记。   | 是 | 否 |
| _TeamworkTag.Read.All_ | 读取 Microsoft Teams 中的标记。 | 允许应用在没有登录的用户的情况下读 Teams 中的标记 | 是 | 否 |


## <a name="terms-of-use-permissions"></a>使用条款权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Agreement.Read.All_ | 阅读所有使用条款协议 | 允许应用代表登录用户阅读使用条款协议。 | 是 | 否 |
| _Agreement.ReadWrite.All_ | 阅读和编写所有使用协议条款 | 允许应用代表登录用户阅读和编写使用条款协议。 | 是 | 否 |
| _AgreementAcceptance.Read_ | 阅读用户使用条款接受状态 | 允许应用代表登录用户阅读使用条款接受状态。 | 是 | 否 |
| _AgreementAcceptance.Read.All_ | 阅读用户可以访问的使用条款接受状态 | 允许应用代表登录用户阅读使用条款接受状态。 | 是 | 否 |

### <a name="remarks"></a>注解

上述所有权限仅对工作或学校帐户有效。

若要使应用能够阅读或编写委派权限的所有协议或协议接受情况，登录用户必须分配有全局管理员、条件访问管理员或安全管理员角色。如需了解有关管理员角色的更多信息，请参阅[在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

### <a name="example-usage"></a>示例用法

#### <a name="delegated"></a>委派
以下使用对两种委派权限均有效：

* _Agreement.Read.All_：阅读所有使用条款协议 (`GET /beta/agreements`)
* _Agreement.ReadWrite.All_：阅读和编写所有使用条款协议 (`POST /beta/agreements`)
* _AgreementAcceptance.Read_：阅读用户使用条款接受状态 (`GET /beta/me/agreementAcceptances`)

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

---

## <a name="threat-assessment-permissions"></a>威胁评估权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _ThreatAssessment.ReadWrite.All_ | 读取和写入威胁评估请求 | 允许应用代表已登录用户读取组织的威胁评估请求。 还允许应用创建新请求来代表已登录用户评估组织收到的威胁。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _ThreatAssessment.Read.All_ | 读取威胁评估请求 | 允许应用在无需用户登录的情况下读取组织的威胁评估请求。 | 是 |

### <a name="remarks"></a>备注

威胁评估权限仅对工作或学校帐户有效。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _ThreatAssessment.ReadWrite.All_：读取和写入评估请求 (`POST /informationProtection/threatAssessmentRequests`)

#### <a name="application"></a>应用程序

* _ThreatAssessment.Read.All_：读取威胁评估请求 (`GET /informationProtection/threatAssessmentRequests`)

---

## <a name="universal-print-permissions"></a>Universal Print permissions

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _Printer.Create_ | 注册打印机 | 允许应用代表已登录的用户创建（注册）打印机。 | 是 | 否 |
| _Printer.FullControl.All_ | 注册、读取、更新和注销打印机 | 允许应用代表已登录用户创建（注册）、读取、更新和删除（取消注册）打印机。 | 是 | 否 |
| _Printer.Read.All_ | 读取打印机 | 允许应用代表已登录用户读取打印机。 | 是 | 否 |
| _Printer.ReadWrite.All_ | 读取和更新打印机 | 允许应用代表已登录用户读取和更新打印机。 不允许创建（正在注册）或删除（正在注销）打印机。 | 是 | 否 |
| _PrinterShare.ReadBasic.All_ | 读取有关打印机共享的基本信息 | 允许应用程序代表已登录用户读取有关打印机共享的基本信息。不允许读取访问控制信息。 | 否 | 否 |
| _PrinterShare.Read.All_ | 读取打印机共享 | 允许应用代表已登录用户读取打印机共享。 | 否 | 否 |
| _PrinterShare.ReadWrite.All_ | 读写打印机共享 | 允许应用代表已登录用户读取和更新打印机共享。 | 是 | 否 |
| _PrintJob.Create_ | 创建打印作业 | 允许应用程序代表已登录用户创建打印作业，并将文档内容上传到已登录用户创建的打印作业。 | 否 | 否 |
| _PrintJob.Read_ | 读取用户的打印作业 | 允许应用读取已登录用户所创建打印作业的元数据和文档内容。 | 否 | 否 |
| _PrintJob.Read.All_ | 读取打印作业 | 允许应用代表已登录用户读取打印作业的元数据和文档内容。 | 是 | 否 |
| _PrintJob.ReadBasic_ | 读取用户打印作业的基本信息 | 允许应用读取已登录用户所创建打印作业的元数据。 不允许访问打印作业文档内容。 | 否 | 否 |
| _PrintJob.ReadBasic.All_ | 读取打印作业的基本信息 | 允许应用代表已登录用户读取打印作业的元数据。 不允许访问打印作业文档内容。 | 是 | 否 |
| _PrintJob.ReadWrite_ | 读取和写入用户的打印作业 | 允许应用读取和更新已登录用户所创建打印作业的元数据和文档内容。 | 否 | 否 |
| _PrintJob.ReadWrite.All_ | 读取和写入打印作业 | 允许应用代表已登录用户读取和更新打印作业的元数据和文档内容。 | 是 | 否 |
| _PrintJob.ReadWriteBasic_ | 读写用户打印作业的基本信息 | 允许应用读取和更新已登录用户所创建打印作业的元数据。 不允许访问打印作业文档内容。 | 否 | 否 |
| _PrintJob.ReadWriteBasic.All_ | 读取和写入打印作业的基本信息 | 允许应用代表已登录用户读取和更新打印作业的元数据。 不允许访问打印作业文档内容。 | 是 | 否 |
| _PrintConnector.Read.All_ | 读取连接器 | 允许应用程序代表已登录的用户读取连接器。 | 是 | 否 |
| _PrintConnector.ReadWrite.All_ | 读取和写入打印连接器 | 允许应用程序代表已登录的用户读取和写入打印连接器。 | 是 | 否 |
| _PrintSettings.Read.All_ | 读取租户范围的打印设置 | 允许应用程序代表已登录的用户读取打印设置。 | 是 | 否 |
| _PrintSettings.ReadWrite.All_ | 读取和写入租户范围的打印设置 | 允许应用程序代表已登录的用户读取和更新打印设置。 | 是 | 否 |

#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _Printer.Read.All_ | 读取打印机 | 允许应用在没有登录用户的情况下读取打印机。 | 是 |
| _Printer.ReadWrite.All_ | 读取和更新打印机 | 允许应用在没有登录用户的情况下读取和更新打印机。 不允许创建（正在注册）或删除（正在注销）打印机。 | 是 |
| _PrintJob.Manage.All_ | 在打印作业上执行高级操作 | 允许应用执行高级操作，如在没有登录用户的情况下重定向打印作业至其他打印机。 允许应用读取和更新打印作业的元数据。 | 是 |
| _PrintJob.Read.All_ | 读取打印作业 | 允许应用在没有登录用户的情况下读取打印作业的元数据和文档内容。 | 是 |
| _PrintJob.ReadBasic.All_ | 读取打印作业的基本信息 | 允许应用在没有登录用户的情况下读取打印作业的元数据。 不允许访问打印作业文档内容。 | 是 |
| _PrintJob.ReadWrite.All_ | 读取和写入打印作业 | 允许应用在没有登录用户的情况下读取和更新打印作业的元数据和文档内容。 | 是 |
| _PrintJob.ReadWriteBasic.All_ | 读取和写入打印作业的基本信息 | 允许应用在没有登录用户的情况下读取和更新打印作业的元数据。 不允许访问打印作业文档内容。 | 是 |
| _PrintTaskDefinition.ReadWrite.All_ | 读取、写入和更新打印任务定义 | 允许应用在没有登录用户的情况下读取和更新打印任务定义。 | 是 |

### <a name="remarks"></a>注解

* 若要使用通用打印服务，用户或应用的租户除了前面列出的权限外，还必须具有有效的通用打印订阅。

* 某些权限可区分打印作业元数据和有效负载。 元数据描述了打印作业的配置（其名称和文档配置，例如应该装订还是彩色打印）。 有效负载是文档数据本身（要打印的 PDF 或 XPS 文件。）

* 所有 PrintJob.* 权限还至少需要 Printer.Read.All（或更多特权权限），因为打印作业存储在打印机中。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>Delegated

* _Printer.Read.All_：获取租户中所有打印机的列表 (`GET /print/printers`)
* _PrintJob.Read.All_：获取排队到打印机的所有打印作业的列表 (`GET /print/printers/{id}/jobs`)
* _Printer.FullControl.All_：删除（注销）打印机 (`DELETE /print/printers/{id}`)
* _PrintJob.ReadWriteBasic.All_：更新打印作业的元数据（例如当前状态）(`PATCH /print/printers/{id}/jobs/{id}`)
* _PrintJob.ReadWrite.All_：创建打印作业并向其上传文档数据 (`POST /print/printers/{id}/jobs`)

#### <a name="application"></a>应用程序

* _Printer.Read.All_：获取租户中所有打印机的列表 (`GET /print/printers`)

---

## <a name="user-permissions"></a>用户权限

#### <a name="delegated-permissions"></a>委派权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 | 支持的 Microsoft 帐户 |
|:----------------|:------------------|:-------------|:-----------------------|:--------------|
| _User.Read_       |    登录并读取用户个人资料 | 允许用户登录应用，并允许应用读取登录用户的个人资料。它还允许应用读取登录用户的基本公司信息。| 否 | 是 |
| _User.ReadWrite_ |    对用户个人资料的读写权限 | 允许应用读取登录用户的完整个人资料。 此外，它还允许应用代表登录用户来更新其个人资料信息。 | 否 | 是 |
| _User.ReadBasic.All_ |    读取所有用户的基本个人资料 | 允许应用代表登录用户读取组织中其他用户的一套基本个人资料属性。 其中包括显示名称、名字和姓氏、电子邮件地址、开放扩展和照片。 此外，还允许应用读取已登录用户的完整个人资料。 | 否 | 否 |
| _User.Read.All_  |     读取所有用户的完整个人资料           | 允许应用代表登录用户读取组织中其他用户的整套个人资料属性、下属和经理。 | 是 | 否 |
| _User.ReadWrite.All_ |     读取和写入所有用户的完整个人资料 | 允许应用代表登录用户读取和写入组织中其他用户的整套个人资料属性、下属和经理。还允许应用代表已登录用户创建和删除用户以及重置用户密码。 | 是 | 否 |
| _User.Invite.All_  |     将来宾用户邀请到组织 | 允许应用代表已登录用户将来宾用户邀请到你的组织。 | 是 | 否 |
| _User.Export.All_       |    导出用户数据 | 当由公司管理员执行时，允许应用导出组织的用户数据。| 是 | 否 |
| _User.ManageIdentities.All_       |    管理用户标识 | 允许应用程序读取、更新和删除与登录用户有权访问的用户帐户相关联的标识。这控制了用户可以使用哪些标识进行登录。 | 是 | 否 |


#### <a name="application-permissions"></a>应用程序权限

|   权限    |  显示字符串   |  说明 | 需经过管理员同意 |
|:----------------|:------------------|:-------------|:-----------------------|
| _User.Read.All_ |    读取所有用户的完整个人资料 | 允许应用在没有登录用户的情况下读取组织中其他用户的整套个人资料属性、组成员身份、下属和经理。| 是 |
| _User.ReadWrite.All_ |   读取和写入所有用户的完整个人资料 | 允许应用在没有登录用户的情况下读取和写入组织中其他用户的整套个人资料属性、组成员身份、下属和经理。还允许应用创建和删除非管理用户。不允许重置用户密码。 | 是 |
| _User.Invite.All_  |     将来宾用户邀请到组织 | 允许应用无需具有已登录用户即可将来宾用户邀请到你的组织。 | 是 |
| _User.Export.All_       |    导出用户数据 | 允许应用导出组织用户数据，而无需是登录用户。| 是 |
| _User.ManageIdentities.All_       |    管理所有用户标识 | 允许应用程序在没有登录用户的情况下读取、更新和删除与用户帐户相关联的标识。这控制了用户可以使用哪些标识进行登录。 |  是 |

### <a name="remarks"></a>说明

通过 _User.Read_ 权限，应用还可以通过 [organization](/graph/api/resources/organization) 资源读取工作或学校帐户的已登录用户的基本公司信息。以下属性可用：ID、displayName 和 verifiedDomains。

对于工作或学校帐户，完整个人资料包括 [User](/graph/api/resources/user) 资源的所有声明属性。在读取时，默认情况下仅返回有限数量的属性。若要读取不在默认设置中的属性，请使用 `$select`。默认属性包括：

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

使用 _User.ReadWrite.All_ 委派或应用程序权限，仅允许非管理员或分配了以下角色之一的用户更新其他用户的 **businessPhones**、 **mobilePhone** 或 **other邮件** ：目录读取者、来宾邀请者、 消息中心读取器和报表读取器。有关更多详细信息，请参阅支持人员（密码）管理员 [Azure AD可用角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。

要读取或写入工作或学校帐户的直接下属 (`directReports`) 或经理 (`manager`)，应用必须具有 _User.Read.All_（只读）或 _User.ReadWrite.All_。

_User.ReadBasic.All_ 权限限制应用访问称为基本个人资料的有限属性集。这是因为完整的个人资料可能包含敏感的目录信息。基本个人资料仅包括以下属性：

- displayName
- givenName
- mail
- photo
- surname
- userPrincipalName

若要读取用户的组成员资格 (`memberOf`)，则应用必须具有 [_Group.Read.All_](#group-permissions) 或 [_Group.ReadWrite.All_](#group-permissions)。但是，如果用户还具有 [directoryRole](/graph/api/resources/directoryrole) 或 [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true) 中的成员资格，则应用还将需要有效权限来读取这些资源，否则 Microsoft Graph 将返回错误。这意味着应用还需要 [目录权限](#directory-permissions)，而对于委派权限来说，已登录的用户还需要组织内的足够特权来访问目录角色和管理单元。

使用 _User.ManageIdentities.All_ 委派权限或应用程序权限，可以更新用户标识 (`identities`)。 这包括具有基于电子邮件地址或姓名的登录名的联合标识（亦称为“社交标识”）或本地标识。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派

* _User.Read_：读取登录用户的完整配置文件 (`GET /me`)。
* _User.ReadWrite_：更新登录用户的照片 (`PUT /me/photo/$value`)。
* _User.ReadBasic.All_：查找名称以“David”开头的所有用户 (`GET /users?$filter=startswith(displayName,'David')`)。
* _User.Read.All_：读取用户的经理 (`GET /users/{id | userPrincipalName}/manager`)。

#### <a name="application"></a>应用程序

* _User.Read.All_：通过 delta 查询读取所有用户和关系 (`GET /beta/users/delta?$select=displayName,givenName,surname`)。
* _User.ReadWrite.All_：更新组织中任意用户的照片 (`PUT /users/{id | userPrincipalName}/photo/$value`)。

有关涉及多个权限的更复杂的情况，请参阅[权限方案](#permission-scenarios)。

## <a name="user-activity-permissions"></a>用户活动权限

#### <a name="delegated-permissions"></a>委派权限

|权限    |显示字符串   |说明 |需经过管理员同意 | 支持的 Microsoft 帐户 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|:-----------------|
| _UserActivity.ReadWrite.CreatedByApp_ |将应用活动读取和写入到用户的活动源 |允许应用读取和报告登录用户在应用中的活动。 |否 | 是 |

#### <a name="application-permissions"></a>应用程序权限
无。

### <a name="remarks"></a>说明
*UserActivity.ReadWrite.CreatedByApp* 对 Microsoft 帐户和工作或学校帐户均有效。

与此权限相关联的 *CreatedByApp* 约束指示服务将基于调用应用的标识（MSA 应用 ID 或针对跨平台应用程序标识配置的一组应用 ID）对结果应用隐式筛选。

### <a name="example-usage"></a>用法示例

#### <a name="delegated"></a>委派
* _UserActivity.ReadWrite.CreatedByApp_：基于最后一天发布的相关联的历史记录项来获取最近特定用户活动的列表。(GET /me/activities/recent)。
* _UserActivity.ReadWrite.CreatedByApp_：发布或更新可能由应用程序用户恢复的用户活动。(PUT /me/activities/%2Farticle%3F12345)。
*   _UserActivity.ReadWrite.CreatedByApp_：发布或更新指定用户活动的历史记录项，以表示用户参与的时间段。(PUT /me/activities/{id}/historyItems/{id})。
*   _UserActivity.ReadWrite.CreatedByApp_：根据用户发起的请求删除用户活动或删除无效数据。(DELETE /me/activities/{id})。
*   _UserActivity.ReadWrite.CreatedByApp_：根据用户发起的请求删除历史记录项或删除无效数据。(DELETE /me/activities/{id}/historyItems/{id})。

---

## <a name="user-authentication-method-permissions-preview"></a>用户身份验证方法权限（[预览版](#permissions-availability-status)）

#### <a name="delegated-permissions"></a>委派权限

|权限                              |显示字符串                        |说明        |需经过管理员同意 | 支持的 Microsoft 帐户 |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|:----------------------------|
|_UserAuthenticationMethod.Read_（预览版）        |读取自己的身份验证方法       |允许该应用读取已登录用户的身份验证方法，包括电话号码和 Authenticator 应用设置。 这不允许该应用查看已登录用户的密码之类的机密信息，也无法登录或以其他方式使用已登录用户的身份验证方法。 |是|否|
|_UserAuthenticationMethod.Read.All_（预览版）    |读取用户的身份验证方法    |允许此应用读取已登录用户有权访问的组织中所有用户的身份验证方法。 身份验证方法包括用户的电话号码和 Authenticator 应用设置之类的内容。 这不允许该应用查看密码之类的机密信息，也无法登录或以其他方式使用身份验证方法。 |是|否|
|_UserAuthenticationMethod.ReadWrite_（预览版）   |管理自己的身份验证方法     |允许该应用读取和写入已登录用户的身份验证方法，包括电话号码和 Authenticator 应用设置。 这不允许该应用查看已登录用户的密码之类的机密信息，也无法登录或以其他方式使用已登录用户的身份验证方法。 |是|否|
|_UserAuthenticationMethod.ReadWrite.All_（预览版）|管理用户的身份验证方法  |允许此应用读取和写入已登录用户有权访问的组织中所有用户的身份验证方法。 身份验证方法包括用户的电话号码和 Authenticator 应用设置之类的内容。 这不允许该应用查看密码之类的机密信息，也无法登录或以其他方式使用身份验证方法。 |是|否|

#### <a name="application-permissions"></a>应用程序权限

|权限                              |显示字符串                        |说明        |需经过管理员同意 |
|:---------------------------------------|:-------------------------------------|:------------------|:----------------------|
|_UserAuthenticationMethod.Read.All_（预览版）   |读取用户的身份验证方法    |允许此应用读取组织中所有用户的身份验证方法，无已登录用户。 身份验证方法包括用户的电话号码和 Authenticator 应用设置之类的内容。 这不允许该应用查看密码之类的机密信息，也无法登录或以其他方式使用身份验证方法。 |是|
|_UserAuthenticationMethod.ReadWrite.All_（预览版）|管理用户的身份验证方法  |允许此应用程序读取和写入组织中所有用户的身份验证方法，无已登录用户。 身份验证方法包括用户的电话号码和 Authenticator 应用设置之类的内容。 这不允许该应用查看密码之类的机密信息，也无法登录或以其他方式使用身份验证方法。 |是|

### <a name="remarks"></a>备注

用户身份验证方法权限用于管理用户的身份验证方法。借助这些权限，委派的用户或应用程序可以注册用户的新身份验证方法，读取用户已注册的身份验证方法，更新这些身份验证方法，以及从用户中删除它们。

借助这些权限，可以读取和管理用户的所有身份验证方法。这包括用于以下方面的方法：

* 主要身份验证（密码）
* 多重身份验证/MFA（电话号码）的第二因素
* 自助密码重置/SSPR（电子邮件地址）

## <a name="windows-updates-permissions"></a>Windows 更新权限

#### <a name="delegated-permissions"></a>委派权限

|权限|显示字符串|说明|需经过管理员同意|支持的 Microsoft 帐户|
|:---|:---|:---|:---|:---|
|_WindowsUpdates.ReadWrite.All_|读取和写入所有 Windows 更新部署设置|允许应用代表已登录的用户读取和写入组织的所有 Windows 更新部署设置。|是|否|

#### <a name="application-permissions"></a>应用程序权限

|权限|显示字符串|说明|需经过管理员同意|
|:---|:---|:---|:---|
|_WindowsUpdates.ReadWrite.All_|读取和写入所有 Windows 更新部署设置|允许应用在没有登录用户的情况下读取和写入组织的所有 Windows 更新部署设置。|是|

### <a name="remarks"></a>注解

上述所有权限仅对工作或学校帐户有效。

对于使用委派权限读取或写入所有 Windows 更新部署设置的应用，已登录用户必须分配为全局管理员、Intune 管理员或 Windows 更新部署管理员角色。有关管理员角色的详细信息，请参阅 [在 Azure Active Directory 中分配管理员角色](/azure/active-directory/active-directory-assign-admin-roles)。

### <a name="example-usage"></a>示例用法

#### <a name="delegated"></a>委派

* _WindowsUpdates.ReadWrite.All_：创建部署(`POST /beta/admin/windows/updates/deployments`)。

#### <a name="application"></a>应用程序

* _WindowsUpdates.ReadWrite.All_：创建部署(`POST /beta/admin/windows/updates/deployments`)。

## <a name="permission-scenarios"></a>权限方案

本节介绍一些面向组织中 [user](/graph/api/resources/user) 和 [group](/graph/api/resources/group) 资源的常见方案。这些表显示了应用执行方案要求的特定操作所需的权限。请注意，在某些情况下，应用执行特定操作的能力取决于权限是应用程序权限还是委派权限。如果是委派权限，应用的有效权限还将取决于组织内已登录用户的特权。有关详细信息，请参阅[委派权限、应用程序权限和有效权限](auth/auth-concepts.md#microsoft-graph-permissions)。

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
| 应用想要提交数据策略操作请求，以导出用户的个人数据 | _User.Export.All_ | 导出用户的个人数据。 |


### <a name="access-scenarios-on-the-group-resource"></a>关于组资源的访问方案

| **涉及组的应用任务**  |  **必需的权限** |  **权限字符串** |
|:-------------------------------|:---------------------|:---------------|
| 应用想要读取基本组信息（仅限显示名称和图片），例如展示组挑选经验  | _Group.Read.All_  | 读取所有组|
| 应用想要读取所有 Microsoft 365 组中的全部内容（包括文件、对话）。它还需要显示组成员，能够更新组成员（若是所有者）。  |  _Group.Read.All_ | 读取所有网站集中的项、读取所有组|
| 应用想要读取和写入所有 Microsoft 365 组中的全部内容（包括文件、对话）。它还需要显示组成员，能够更新组成员（若是所有者）。  |    _Group.ReadWrite.All_, _Sites.ReadWrite.All_ |  读取和写入所有组、编辑或删除所有网站集中的项 |
| 应用想要发现（找到）Microsoft 365 组。它允许用户搜索特定组，然后从枚举列表中选择一个组，从而允许用户加入组。   | _Group.ReadWrite.All_ | 读取和写入所有组|
| 应用想要通过 AAD Graph 创建一个组 |   _Group.ReadWrite.All_ | 读取和写入所有组|


## <a name="all-permissions-and-ids"></a>所有权限和 ID

| 权限                                              | 类型        | ID                                   |
|---------------------------------------------------------|-------------|--------------------------------------|
| AccessReview.Read.All                                   | 应用程序 | d07a8cc0-3d51-4b77-b3b0-32704d1f69fa |
| AccessReview.Read.All                                   | 委派   | ebfcd32b-babb-40f4-a14b-42706e83bd28 |
| AccessReview.ReadWrite.All                              | 应用程序 | ef5f7d5c-338f-44b0-86c3-351f46c8bb5f |
| AccessReview.ReadWrite.All                              | 委派   | e4aa47b9-9a69-4109-82ed-36ec70d85ff1 |
| AccessReview.ReadWrite.Membership                       | 应用程序 | 18228521-a591-40f1-b215-5fad4488c117 |
| AccessReview.ReadWrite.Membership                       | 委派   | 5af8c3f5-baca-439a-97b0-ea58a435e269 |
| AdministrativeUnit.Read.All                             | 应用程序 | 134fd756-38ce-4afd-ba33-e9623dbe66c2 |
| AdministrativeUnit.Read.All                             | 委派   | 3361d15d-be43-4de6-b441-3c746d05163d |
| AdministrativeUnit.ReadWrite.All                        | 应用程序 | 5eb59dd3-1da2-4329-8733-9dabdc435916 |
| AdministrativeUnit.ReadWrite.All                        | 委派   | 7b8a2d34-6b3f-4542-a343-54651608ad81 |
| Agreement.Read.All                                      | 应用程序 | 2f3e6f8c-093b-4c57-a58b-ba5ce494a169 |
| Agreement.Read.All                                      | 委派   | af2819c9-df71-4dd3-ade7-4d7c9dc653b7 |
| Agreement.ReadWrite.All                                 | 应用程序 | c9090d00-6101-42f0-a729-c41074260d47 |
| Agreement.ReadWrite.All                                 | 委派   | ef4b5d93-3104-4664-9053-a5c49ab44218 |
| AgreementAcceptance.Read                                | 委派   | 0b7643bb-5336-476f-80b5-18fbfbc91806 |
| AgreementAcceptance.Read.All                            | 应用程序 | d8e4ec18-f6c0-4620-8122-c8b1f2bf400e |
| AgreementAcceptance.Read.All                            | 委派   | a66a5341-e66e-4897-9d52-c2df58c2bfb9 |
| Analytics.Read                                          | 委派   | e03cf23f-8056-446a-8994-7d93dfc8b50e |
| APIConnectors.Read.All                                  | 应用程序 | b86848a7-d5b1-41eb-a9b4-54a4e6306e97 |
| APIConnectors.Read.All                                  | 委派   | 1b6ff35f-31df-4332-8571-d31ea5a4893f |
| APIConnectors.ReadWrite.All                             | 应用程序 | 1dfe531a-24a6-4f1b-80f4-7a0dc5a0a171 |
| APIConnectors.ReadWrite.All                             | 委派   | c67b52c5-7c69-48b6-9d48-7b3af3ded914 |
| AppCatalog.Read.All                                     | 应用程序 | e12dae10-5a57-4817-b79d-dfbec5348930 |
| AppCatalog.Read.All                                     | 委派   | 88e58d74-d3df-44f3-ad47-e89edf4472e4 |
| AppCatalog.ReadWrite.All                                | 应用程序 | dc149144-f292-421e-b185-5953f2e98d7f |
| AppCatalog.ReadWrite.All                                | 委派   | 1ca167d5-1655-44a1-8adf-1414072e1ef9 |
| AppCatalog.Submit                                       | 委派   | 3db89e36-7fa6-4012-b281-85f3d9d9fd2e |
| Application.Read.All                                    | 应用程序 | 9a5d68dd-52b0-4cc2-bd40-abcf44ac3a30 |
| Application.Read.All                                    | 委派   | c79f8feb-a9db-4090-85f9-90d820caa0eb |
| Application.ReadWrite.All                               | 应用程序 | 1bfefb4e-e0b5-418b-a88f-73c46d2cc8e9 |
| Application.ReadWrite.All                               | 委派   | bdfbf15f-ee85-4955-8675-146e8e5296b5 |
| Application.ReadWrite.OwnedBy                           | 应用程序 | 18a4783c-866b-4cc7-a460-3d5e5662c884 |
| AppRoleAssignment.ReadWrite.All                         | 应用程序 | 06b708a9-e830-4db3-a914-8e69da51d44f |
| AppRoleAssignment.ReadWrite.All                         | 委派   | 84bccea3-f856-4a8a-967b-dbe0a3d53a64 |
| Approval.Read.All                                       | 委派   | 1196552e-b226-4363-b01e-b8901fe10a11 |
| Approval.ReadWrite.All                                  | 委派   | 1d3d0bc7-4b3a-427a-ae9f-6de4e1edc95f |
| AuditLog.Read.All                                       | 应用程序 | b0afded3-3588-46d8-8b3d-9842eff778da |
| AuditLog.Read.All                                       | 委派   | e4c9e354-4dc5-45b8-9e7c-e1393b0b1a20 |
| BitlockerKey.Read.All                                   | 应用程序 | 57f1cf28-c0c4-4ec3-9a30-19a2eaaf2f6e |
| BitlockerKey.Read.All                                   | 委派   | b27a61ec-b99c-4d6a-b126-c4375d08ae30 |
| BitlockerKey.ReadBasic.All                              | 应用程序 | f690d423-6b29-4d04-98c6-694c42282419 |
| BitlockerKey.ReadBasic.All                              | 委派   | 5a107bfc-4f00-4e1a-b67e-66451267bc68 |
| Bookings.Manage.All                                     | 委派   | 7f36b48e-542f-4d3b-9bcb-8406f0ab9fdb |
| Bookings.Read.All                                       | 委派   | 33b1df99-4b29-4548-9339-7a7b83eaeebc |
| Bookings.ReadWrite.All                                  | 委派   | 948eb538-f19d-4ec5-9ccc-f059e1ea4c72 |
| BookingsAppointment.ReadWrite.All                       | 委派   | 02a5a114-36a6-46ff-a102-954d89d9ab02 |
| Calendars.Read                                          | 应用程序 | 798ee544-9d2d-430c-a058-570e29e34338 |
| Calendars.Read                                          | 委派   | 465a38f9-76ea-45b9-9f34-9e8b0d4b0b42 |
| Calendars.Read.Shared                                   | 委派   | 2b9c4092-424d-4249-948d-b43879977640 |
| Calendars.ReadWrite                                     | 应用程序 | ef54d2bf-783f-4e0f-bca1-3210c0444d99 |
| Calendars.ReadWrite                                     | 委派   | 1ec239c2-d7c9-4623-a91a-a9775856bb36 |
| Calendars.ReadWrite.Shared                              | 委派   | 12466101-c9b8-439a-8589-dd09ee67e8e9 |
| CallRecord-PstnCalls.Read.All                           | 应用程序 | a2611786-80b3-417e-adaa-707d4261a5f0 |
| CallRecords.Read.All                                    | 应用程序 | 45bbb07e-7321-4fd7-a8f6-3ff27e6a81c8 |
| Calls.AccessMedia.All                                   | 应用程序 | a7a681dc-756e-4909-b988-f160edc6655f |
| Calls.Initiate.All                                      | 应用程序 | 284383ee-7f6e-4e40-a2a8-e85dcb029101 |
| Calls.InitiateGroupCall.All                             | 应用程序 | 4c277553-8a09-487b-8023-29ee378d8324 |
| Calls.JoinGroupCall.All                                 | 应用程序 | f6b49018-60ab-4f81-83bd-22caeabfed2d |
| Calls.JoinGroupCallAsGuest.All                          | 应用程序 | fd7ccf6b-3d28-418b-9701-cd10f5cd2fd4 |
| Channel.Create                                          | 应用程序 | f3a65bd4-b703-46df-8f7e-0174fea562aa |
| Channel.Create                                          | 委派   | 101147cf-4178-4455-9d58-02b5c164e759 |
| Channel.Delete.All                                      | 应用程序 | 6a118a39-1227-45d4-af0c-ea7b40d210bc |
| Channel.Delete.All                                      | 委派   | cc83893a-e232-4723-b5af-bd0b01bcfe65 |
| Channel.ReadBasic.All                                   | 应用程序 | 59a6b24b-4225-4393-8165-ebaec5f55d7a |
| Channel.ReadBasic.All                                   | 委派   | 9d8982ae-4365-4f57-95e9-d6032a4c0b87 |
| ChannelMember.Read.All                                  | 应用程序 | 3b55498e-47ec-484f-8136-9013221c06a9 |
| ChannelMember.Read.All                                  | 委派   | 2eadaff8-0bce-4198-a6b9-2cfc35a30075 |
| ChannelMember.ReadWrite.All                             | 应用程序 | 35930dcf-aceb-4bd1-b99a-8ffed403c974 |
| ChannelMember.ReadWrite.All                             | 委派   | 0c3e411a-ce45-4cd1-8f30-f99a3efa7b11 |
| ChannelMessage.Delete                                   | 委派   | 32ea53ac-4a89-4cde-bac4-727c6fb9ac29 |
| ChannelMessage.Edit                                     | 委派   | 2b61aa8a-6d36-4b2f-ac7b-f29867937c53 |
| ChannelMessage.Read.All                                 | 应用程序 | 7b2449af-6ccd-4f4d-9f78-e550c193f0d1 |
| ChannelMessage.Read.All                                 | 委派   | 767156cb-16ae-4d10-8f8b-41b657c8c8c8 |
| ChannelMessage.Send                                     | 委派   | ebf0f66e-9fb1-49e4-a278-222f76911cf4 |
| ChannelMessage.UpdatePolicyViolation.All                | 应用程序 | 4d02b0cc-d90b-441f-8d82-4fb55c34d6bb |
| ChannelSettings.Read.All                                | 应用程序 | c97b873f-f59f-49aa-8a0e-52b32d762124 |
| ChannelSettings.Read.All                                | 委派   | 233e0cf1-dd62-48bc-b65b-b38fe87fcf8e |
| ChannelSettings.ReadWrite.All                           | 应用程序 | 243cded2-bd16-4fd6-a953-ff8177894c3d |
| ChannelSettings.ReadWrite.All                           | 委派   | d649fb7c-72b4-4eec-b2b4-b15acf79e378 |
| Chat.Create                                             | 应用程序 | d9c48af6-9ad9-47ad-82c3-63757137b9af |
| Chat.Create                                             | 委派   | 38826093-1258-4dea-98f0-00003be2b8d0 |
| Chat.Read                                               | 委派   | f501c180-9344-439a-bca0-6cbf209fd270 |
| Chat.Read.All                                           | 应用程序 | 6b7d71aa-70aa-4810-a8d9-5d9fb2830017 |
| Chat.ReadBasic                                          | 委派   | 9547fcb5-d03f-419d-9948-5928bbf71b0f |
| Chat.ReadBasic.All                                      | 应用程序 | b2e060da-3baf-4687-9611-f4ebc0f0cbde |
| Chat.ReadWrite                                          | 委派   | 9ff7295e-131b-4d94-90e1-69fde507ac11 |
| Chat.ReadWrite.All                                      | 应用程序 | 294ce7c9-31ba-490a-ad7d-97a7d075e4ed |
| Chat.UpdatePolicyViolation.All                          | 应用程序 | 7e847308-e030-4183-9899-5235d7270f58 |
| ChatMember.Read                                         | 委派   | c5a9e2b1-faf6-41d4-8875-d381aa549b24 |
| ChatMember.Read.All                                     | 应用程序 | a3410be2-8e48-4f32-8454-c29a7465209d |
| ChatMember.ReadWrite                                    | 委派   | dea13482-7ea6-488f-8b98-eb5bbecf033d |
| ChatMember.ReadWrite.All                                | 应用程序 | 57257249-34ce-4810-a8a2-a03adf0c5693 |
| ChatMessage.Read                                        | 委派   | cdcdac3a-fd45-410d-83ef-554db620e5c7 |
| ChatMessage.Read.All                                    | 应用程序 | b9bb2381-47a4-46cd-aafb-00cb12f68504 |
| ChatMessage.Send                                        | 委派   | 116b7235-7cc6-461e-b163-8e55691d839e |
| CloudPC.Read.All                                        | 应用程序 | a9e09520-8ed4-4cde-838e-4fdea192c227 |
| CloudPC.Read.All                                        | 委派   | 5252ec4e-fd40-4d92-8c68-89dd1d3c6110 |
| CloudPC.ReadWrite.All                                   | 应用程序 | 3b4349e1-8cf5-45a3-95b7-69d1751d3e6a |
| CloudPC.ReadWrite.All                                   | 委派   | 9d77138f-f0e2-47ba-ab33-cd246c8b79d1 |
| ConsentRequest.Read.All                                 | 应用程序 | 1260ad83-98fb-4785-abbb-d6cc1806fd41 |
| ConsentRequest.Read.All                                 | 委派   | f3bfad56-966e-4590-a536-82ecf548ac1e |
| ConsentRequest.ReadWrite.All                            | 应用程序 | 9f1b81a7-0223-4428-bfa4-0bcb5535f27d |
| ConsentRequest.ReadWrite.All                            | 委派   | 497d9dfa-3bd1-481a-baab-90895e54568c |
| Contacts.Read                                           | 应用程序 | 089fe4d0-434a-44c5-8827-41ba8a0b17f5 |
| Contacts.Read                                           | 委派   | ff74d97f-43af-4b68-9f2a-b77ee6968c5d |
| Contacts.Read.Shared                                    | 委派   | 242b9d9e-ed24-4d09-9a52-f43769beb9d4 |
| Contacts.ReadWrite                                      | 应用程序 | 6918b873-d17a-4dc1-b314-35f528134491 |
| Contacts.ReadWrite                                      | 委派   | d56682ec-c09e-4743-aaf4-1a3aac4caa21 |
| Contacts.ReadWrite.Shared                               | 委派   | afb6c84b-06be-49af-80bb-8f3f77004eab |
| CrossTenantInformation.ReadBasic.All                    | 应用程序 | cac88765-0581-4025-9725-5ebc13f729ee |
| CrossTenantInformation.ReadBasic.All                    | 委派   | 81594d25-e88e-49cf-ac8c-fecbff49f994 |
| CrossTenantUserProfileSharing.Read                      | 委派   | cb1ba48f-d22b-4325-a07f-74135a62ee41 |
| CrossTenantUserProfileSharing.Read.All                  | 应用程序 | 8b919d44-6192-4f3d-8a3b-f86f8069ae3c |
| CrossTenantUserProfileSharing.Read.All                  | 委派   | 759dcd16-3c90-463c-937e-abf89f991c18 |
| CrossTenantUserProfileSharing.ReadWrite                 | 委派   | eed0129d-dc60-4f30-8641-daf337a39ffd |
| CrossTenantUserProfileSharing.ReadWrite.All             | 应用程序 | 306785c5-c09b-4ba0-a4ee-023f3da165cb |
| CrossTenantUserProfileSharing.ReadWrite.All             | 委派   | 64dfa325-cbf8-48e3-938d-51224a0cac01 |
| CustomSecAttributeAssignment.Read.All                   | 应用程序 | 3b37c5a4-1226-493d-bec3-5d6c6b866f3f |
| CustomSecAttributeAssignment.Read.All                   | 委派   | b46ffa80-fe3d-4822-9a1a-c200932d54d0 |
| CustomSecAttributeAssignment.ReadWrite.All              | 应用程序 | de89b5e4-5b8f-48eb-8925-29c2b33bd8bd |
| CustomSecAttributeAssignment.ReadWrite.All              | 委派   | ca46335e-8453-47cd-a001-8459884efeae |
| CustomSecAttributeDefinition.Read.All                   | 应用程序 | b185aa14-d8d2-42c1-a685-0f5596613624 |
| CustomSecAttributeDefinition.Read.All                   | 委派   | ce026878-a0ff-4745-a728-d4fedd086c07 |
| CustomSecAttributeDefinition.ReadWrite.All              | 应用程序 | 12338004-21f4-4896-bf5e-b75dfaf1016d |
| CustomSecAttributeDefinition.ReadWrite.All              | 委派   | 8b0160d4-5743-482b-bb27-efc0a485ca4a |
| DelegatedAdminRelationship.Read.All                     | 应用程序 | f6e9e124-4586-492f-adc0-c6f96e4823fd |
| DelegatedAdminRelationship.Read.All                     | 委派   | 0c0064ea-477b-4130-82a5-4c2cc4ff68aa |
| DelegatedAdminRelationship.ReadWrite.All                | 应用程序 | cc13eba4-8cd8-44c6-b4d4-f93237adce58 |
| DelegatedAdminRelationship.ReadWrite.All                | 委派   | 885f682f-a990-4bad-a642-36736a74b0c7 |
| DelegatedPermissionGrant.ReadWrite.All                  | 应用程序 | 8e8e4742-1d95-4f68-9d56-6ee75648c72a |
| DelegatedPermissionGrant.ReadWrite.All                  | 委派   | 41ce6ca6-6826-4807-84f1-1c82854f7ee5 |
| Device.Command                                          | 委派   | bac3b9c2-b516-4ef4-bd3b-c2ef73d8d804 |
| Device.Read                                             | 委派   | 11d4cd79-5ba5-460f-803f-e22c8ab85ccd |
| Device.Read.All                                         | 应用程序 | 7438b122-aefc-4978-80ed-43db9fcc7715 |
| Device.Read.All                                         | 委派   | 951183d1-1a61-466f-a6d1-1fde911bfd95 |
| Device.ReadWrite.All                                    | 应用程序 | 1138cb37-bd11-4084-a2b7-9f71582aeddb |
| DeviceManagementApps.Read.All                           | 应用程序 | 7a6ee1e7-141e-4cec-ae74-d9db155731ff |
| DeviceManagementApps.Read.All                           | 委派   | 4edf5f54-4666-44af-9de9-0144fb4b6e8c |
| DeviceManagementApps.ReadWrite.All                      | 应用程序 | 78145de6-330d-4800-a6ce-494ff2d33d07 |
| DeviceManagementApps.ReadWrite.All                      | 委派   | 7b3f05d5-f68c-4b8d-8c59-a2ecd12f24af |
| DeviceManagementConfiguration.Read.All                  | 应用程序 | dc377aa6-52d8-4e23-b271-2a7ae04cedf3 |
| DeviceManagementConfiguration.Read.All                  | 委派   | f1493658-876a-4c87-8fa7-edb559b3476a |
| DeviceManagementConfiguration.ReadWrite.All             | 应用程序 | 9241abd9-d0e6-425a-bd4f-47ba86e767a4 |
| DeviceManagementConfiguration.ReadWrite.All             | 委派   | 0883f392-0a7a-443d-8c76-16a6d39c7b63 |
| DeviceManagementManagedDevices.PrivilegedOperations.All | 应用程序 | 5b07b0dd-2377-4e44-a38d-703f09a0dc3c |
| DeviceManagementManagedDevices.PrivilegedOperations.All | 委派   | 3404d2bf-2b13-457e-a330-c24615765193 |
| DeviceManagementManagedDevices.Read.All                 | 应用程序 | 2f51be20-0bb4-4fed-bf7b-db946066c75e |
| DeviceManagementManagedDevices.Read.All                 | 委派   | 314874da-47d6-4978-88dc-cf0d37f0bb82 |
| DeviceManagementManagedDevices.ReadWrite.All            | 应用程序 | 243333ab-4d21-40cb-a475-36241daa0842 |
| DeviceManagementManagedDevices.ReadWrite.All            | 委派   | 44642bfe-8385-4adc-8fc6-fe3cb2c375c3 |
| DeviceManagementRBAC.Read.All                           | 应用程序 | 58ca0d9a-1575-47e1-a3cb-007ef2e4583b |
| DeviceManagementRBAC.Read.All                           | 委派   | 49f0cc30-024c-4dfd-ab3e-82e137ee5431 |
| DeviceManagementRBAC.ReadWrite.All                      | 应用程序 | e330c4f0-4170-414e-a55a-2f022ec2b57b |
| DeviceManagementRBAC.ReadWrite.All                      | 委派   | 0c5e8a55-87a6-4556-93ab-adc52c4d862d |
| DeviceManagementServiceConfig.Read.All                  | 应用程序 | 06a5fe6d-c49d-46a7-b082-56b1b14103c7 |
| DeviceManagementServiceConfig.Read.All                  | 委派   | 8696daa5-bce5-4b2e-83f9-51b6defc4e1e |
| DeviceManagementServiceConfig.ReadWrite.All             | 应用程序 | 5ac13192-7ace-4fcf-b828-1a26f28068ee |
| DeviceManagementServiceConfig.ReadWrite.All             | 委派   | 662ed50a-ac44-4eef-ad86-62eed9be2a29 |
| Directory.AccessAsUser.All                              | 委派   | 0e263e50-5827-48a4-b97c-d940288653c7 |
| Directory.Read.All                                      | 应用程序 | 7ab1d382-f21e-4acd-a863-ba3e13f7da61 |
| Directory.Read.All                                      | 委派   | 06da0dbc-49e2-44d2-8312-53f166ab848a |
| Directory.ReadWrite.All                                 | 应用程序 | 19dbc75e-c2e2-444c-a770-ec69d8559fc7 |
| Directory.ReadWrite.All                                 | 委派   | c5366453-9fb0-48a5-a156-24f0c49a4b84 |
| Directory.Write.Restricted                              | 应用程序 | f20584af-9290-4153-9280-ff8bb2c0ea7f |
| Directory.Write.Restricted                              | 委派   | cba5390f-ed6a-4b7f-b657-0efc2210ed20 |
| DirectoryRecommendations.Read.All                       | 应用程序 | ae73097b-cb2a-4447-b064-5d80f6093921 |
| DirectoryRecommendations.Read.All                       | 委派   | 34d3bd24-f6a6-468c-b67c-0c365c1d6410 |
| DirectoryRecommendations.ReadWrite.All                  | 应用程序 | 0e9eea12-4f01-45f6-9b8d-3ea4c8144158 |
| DirectoryRecommendations.ReadWrite.All                  | 委派   | f37235e8-90a0-4189-93e2-e55b53867ccd |
| Domain.Read.All                                         | 应用程序 | dbb9058a-0e50-45d7-ae91-66909b5d4664 |
| Domain.Read.All                                         | 委派   | 2f9ee017-59c1-4f1d-9472-bd5529a7b311 |
| Domain.ReadWrite.All                                    | 应用程序 | 7e05723c-0bb0-42da-be95-ae9f08a6e53c |
| Domain.ReadWrite.All                                    | 委派   | 0b5d694c-a244-4bde-86e6-eb5cd07730fe |
| EAS.AccessAsUser.All                                    | 委派   | ff91d191-45a0-43fd-b837-bd682c4a0b0f |
| eDiscovery.Read.All                                     | 应用程序 | 50180013-6191-4d1e-a373-e590ff4e66af |
| eDiscovery.Read.All                                     | 委派   | 99201db3-7652-4d5a-809a-bdb94f85fe3c |
| eDiscovery.ReadWrite.All                                | 应用程序 | b2620db1-3bf7-4c5b-9cb9-576d29eac736 |
| eDiscovery.ReadWrite.All                                | 委派   | acb8f680-0834-4146-b69e-4ab1b39745ad |
| EduAdministration.Read                                  | 委派   | 8523895c-6081-45bf-8a5d-f062a2f12c9f |
| EduAdministration.Read.All                              | 应用程序 | 7c9db06a-ec2d-4e7b-a592-5a1e30992566 |
| EduAdministration.ReadWrite                             | 委派   | 63589852-04e3-46b4-bae9-15d5b1050748 |
| EduAdministration.ReadWrite.All                         | 应用程序 | 9bc431c3-b8bc-4a8d-a219-40f10f92eff6 |
| EduAssignments.Read                                     | 委派   | 091460c9-9c4a-49b2-81ef-1f3d852acce2 |
| EduAssignments.Read.All                                 | 应用程序 | 4c37e1b6-35a1-43bf-926a-6f30f2cdf585 |
| EduAssignments.ReadBasic                                | 委派   | c0b0103b-c053-4b2e-9973-9f3a544ec9b8 |
| EduAssignments.ReadBasic.All                            | 应用程序 | 6e0a958b-b7fc-4348-b7c4-a6ab9fd3dd0e |
| EduAssignments.ReadWrite                                | 委派   | 2f233e90-164b-4501-8bce-31af2559a2d3 |
| EduAssignments.ReadWrite.All                            | 应用程序 | 0d22204b-6cad-4dd0-8362-3e3f2ae699d9 |
| EduAssignments.ReadWriteBasic                           | 委派   | 2ef770a1-622a-47c4-93ee-28d6adbed3a0 |
| EduAssignments.ReadWriteBasic.All                       | 应用程序 | f431cc63-a2de-48c4-8054-a34bc093af84 |
| EduRoster.Read                                          | 委派   | a4389601-22d9-4096-ac18-36a927199112 |
| EduRoster.Read.All                                      | 应用程序 | e0ac9e1b-cb65-4fc5-87c5-1a8bc181f648 |
| EduRoster.ReadBasic                                     | 委派   | 5d186531-d1bf-4f07-8cea-7c42119e1bd9 |
| EduRoster.ReadBasic.All                                 | 应用程序 | 0d412a8c-a06c-439f-b3ec-8 abcf54d2f96 |
| EduRoster.ReadWrite                                     | 委派   | 359e19a6-e3fa-4d7f-bcab-d28ec592b51e |
| EduRoster.ReadWrite.All                                 | 应用程序 | d1808e82-ce13-47af-ae0d-f9b254e6d58a |
| 电子邮件                                                   | 委派   | 64a6cdd6-aab1-4aaf-94b8-3cc8405e90d0 |
| EntitlementManagement.Read.All                          | 应用程序 | c74fd47d-ed3c-45c3-9a9e-b8676de685d2 |
| EntitlementManagement.Read.All                          | 委派   | 5449aa12-1393-4ea2-a7c7-d0e06c1a56b2 |
| EntitlementManagement.ReadWrite.All                     | 应用程序 | 9acd699f-1e81-4958-b001-93b1d2506e19 |
| EntitlementManagement.ReadWrite.All                     | 委派   | ae7a573d-81d7-432b-ad44-4ed5c9d89038 |
| EWS.AccessAsUser.All                                    | 委派   | 9769c687-087d-48ac-9cb3-c37dde652038 |
| ExternalConnection.Read.All                             | 应用程序 | 1914711b-a1cb-4793-b019-c2ce0ed21b8c |
| ExternalConnection.Read.All                             | 委派   | a38267a5-26b6-4d76-9493-935b7599116b |
| ExternalConnection.ReadWrite.All                        | 应用程序 | 34c37bc0-2b40-4d5e-85e1-2365cd256d79 |
| ExternalConnection.ReadWrite.All                        | 委派   | bbbbd9b3-3566-4931-ac37-2b2180d9e334 |
| ExternalConnection.ReadWrite.OwnedBy                    | 应用程序 | f431331c-49a6-499f-be1c-62af19c34a9d |
| ExternalConnection.ReadWrite.OwnedBy                    | 委派   | 4082ad95-c812-4f02-be92-780c4c4f1830 |
| ExternalItem.Read.All                                   | 应用程序 | 7a7cffad-37d2-4f48-afa4-c6ab129adcc2 |
| ExternalItem.Read.All                                   | 委派   | 922f9392-b1b7-483c-a4be-0089be7704fb |
| ExternalItem.ReadWrite.All                              | 应用程序 | 38c3d6ee-69ee-422f-b954-e17819665354 |
| ExternalItem.ReadWrite.All                              | 委派   | b02c54f8-eb48-4c50-a9f0-a149e5a2012f |
| ExternalItem.ReadWrite.OwnedBy                          | 应用程序 | 8116ae0f-55c2-452d-9944-d18420f5b2c8 |
| ExternalItem.ReadWrite.OwnedBy                          | 委派   | 4367b9d7-cee7-4995-853c-a0bdfe95c1f9 |
| Family.Read                                             | 委派   | 3a1e4806-a744-4c70-80fc-223bf8582c46 |
| Files.Read                                              | 委派   | 10465720-29dd-4523-a11a-6a75c743c9d9 |
| Files.Read.All                                          | 应用程序 | 01d4889c-1287-42c6-ac1f-5d1e02578ef6 |
| Files.Read.All                                          | 委派   | df85f4d6-205c-4ac5-a5ea-6bf408dba283 |
| Files.Read.Selected                                     | 委派   | 5447fe39-cb82-4c1a-b977-520e67e724eb |
| Files.ReadWrite                                         | 委派   | 5c28f0bf-8a70-41f1-8ab2-9032436ddb65 |
| Files.ReadWrite.All                                     | 应用程序 | 75359482-378d-4052-8f01-80520e7db3cd |
| Files.ReadWrite.All                                     | 委派   | 863451e7-0667-486c-a5d6-d135439485f0 |
| Files.ReadWrite.AppFolder                               | 委派   | 8019c312-3263-48e6-825e-2b833497195b |
| Files.ReadWrite.Selected                                | 委派   | 17dde5bd-8c17-420f-a486-969730c1b827 |
| Financials.ReadWrite.All                                | 委派   | f534bf13-55d4-45a9-8f3c-c92fe64d6131 |
| Group.Create                                            | 应用程序 | bf7b1a76-6e77-406b-b258-bf5c7720e98f |
| Group.Read.All                                          | 应用程序 | 5b567255-7703-4780-807c-7be8301ae99b |
| Group.Read.All                                          | 委派   | 5f8c59db-677d-491f-a6b8-5f174b11ec1d |
| Group.ReadWrite.All                                     | 应用程序 | 62a82d76-70ea-41e2-9197-370581804d09 |
| Group.ReadWrite.All                                     | 委派   | 4e46008b-f24c-477d-8fff-7bb4ec7aafe0 |
| GroupMember.Read.All                                    | 应用程序 | 98830695-27a2-44f7-8c18-0c3ebc9698f6 |
| GroupMember.Read.All                                    | 委派   | bc024368-1153-4739-b217-4326f2e966d0 |
| GroupMember.ReadWrite.All                               | 应用程序 | dbaae8cf-10b5-4b86-a4a1-f871c94c6695 |
| GroupMember.ReadWrite.All                               | 委派   | f81125ac-d3b7-4573-a3b2-7099cc39df9e |
| IdentityProvider.Read.All                               | 应用程序 | e321f0bb-e7f7-481e-bb28-e3b0b32d4bd0 |
| IdentityProvider.Read.All                               | 委派   | 43781733-b5a7-4d1b-98f4-e8edff23e1a9 |
| IdentityProvider.ReadWrite.All                          | 应用程序 | 90db2b9a-d928-4d33-a4dd-8442ae3d41e4 |
| IdentityProvider.ReadWrite.All                          | 委派   | f13ce604-1677-429f-90bd-8a10b9f01325 |
| IdentityRiskEvent.Read.All                              | 应用程序 | 6e472fd1-ad78-48da-a0f0-97ab2c6b769e |
| IdentityRiskEvent.Read.All                              | 委派   | 8f6a01e7-0391-4ee5-aa22-a3af122cef27 |
| IdentityRiskEvent.ReadWrite.All                         | 应用程序 | db06fb33-1953-4b7b-a2ac-f1e2c854f7ae |
| IdentityRiskEvent.ReadWrite.All                         | 委派   | 9e4862a5-b68f-479e-848a-4e07e25c9916 |
| IdentityRiskyServicePrincipal.Read.All                  | 应用程序 | 607c7344-0eed-41e5-823a-9695ebe1b7b0 |
| IdentityRiskyServicePrincipal.Read.All                  | 委派   | ea5c4ab0-5a73-4f35-8272-5d5337884e5d |
| IdentityRiskyServicePrincipal.ReadWrite.All             | 应用程序 | cb8d6980-6bcb-4507-afec-ed6de3a2d798 |
| IdentityRiskyServicePrincipal.ReadWrite.All             | 委派   | bb6f654c-d7fd-4ae3-85c3-fc380934f515 |
| IdentityRiskyUser.Read.All                              | 应用程序 | dc5007c0-2d7d-4c42-879c-2dab87571379 |
| IdentityRiskyUser.Read.All                              | 委派   | d04bb851-cb7c-4146-97c7-ca3e71baf56c |
| IdentityRiskyUser.ReadWrite.All                         | 应用程序 | 656f6061-f9fe-4807-9708-6a2e0934df76 |
| IdentityRiskyUser.ReadWrite.All                         | 委派   | e0a7cdbb-08b0-4697-8264-0069786e9674 |
| IdentityUserFlow.Read.All                               | 应用程序 | 1b0c317f-dd31-4305-9932-259a8b6e8099 |
| IdentityUserFlow.Read.All                               | 委派   | 2903d63d-4611-4d43-99ce-a33f3f52e343 |
| IdentityUserFlow.ReadWrite.All                          | 应用程序 | 65319a09-a2be-469d-8782-f6b07debf789 |
| IdentityUserFlow.ReadWrite.All                          | 委派   | 281892cc-4dbf-4e3a-b6cc-b21029bb4e82 |
| IMAP.AccessAsUser.All                                   | 委派   | 652390e4-393a-48de-9484-05f9b1212954 |
| InformationProtectionPolicy.Read                        | 委派   | 4ad84827-5578-4e18-ad7a-86530b12f884 |
| InformationProtectionPolicy.Read.All                    | 应用程序 | 19da66cb-0fb0-4390-b071-ebc76a349482 |
| Mail.Read                                               | 应用程序 | 810c84a8-4a9e-49e6-bf7d-12d183f40d01 |
| Mail.Read                                               | 委派   | 570282fd-fa5c-430d-a7fd-fc8dc98a9dca |
| Mail.Read.Shared                                        | 委派   | 7b9103a5-4610-446b-9670-80643382c1fa |
| Mail.ReadBasic                                          | 应用程序 | 6be147d2-ea4f-4b5a-a3fa-3eab6f3c140a |
| Mail.ReadBasic                                          | 委派   | a4b8392a-d8d1-4954-a029-8e668a39a170 |
| Mail.ReadBasic.All                                      | 应用程序 | 693c5e45-0940-467d-9b8a-1022fb9d42ef |
| Mail.ReadWrite                                          | 应用程序 | e2a3a72e-5f79-4c64-b1b1-878b674786c9 |
| Mail.ReadWrite                                          | 委派   | 024d486e-b451-40bb-833d-3e66d98c5c73 |
| Mail.ReadWrite.Shared                                   | 委派   | 5df07973-7d5d-46ed-9847-1271055cbd51 |
| Mail.Send                                               | 应用程序 | b633e1c5-b582-4048-a93e-9f11b44c7e96 |
| Mail.Send                                               | 委派   | e383f46e-2787-4529-855e-0e479a3ffac0 |
| Mail.Send.Shared                                        | 委派   | a367ab51-6b49-43bf-a716-a1fb06d2a174 |
| MailboxSettings.Read                                    | 应用程序 | 40f97065-369a-49f4-947c-6a255697ae91 |
| MailboxSettings.Read                                    | 委派   | 87f447af-9fa4-4c32-9dfa-4a57a73d18ce |
| MailboxSettings.ReadWrite                               | 应用程序 | 6931bccd-447a-43d1-b442-00a195474933 |
| MailboxSettings.ReadWrite                               | 委派   | 818c620a-27a9-40bd-a6a5-d96f7d610b4b |
| ManagedTenants.Read.All                                 | 委派   | dc34164e-6c4a-41a0-be89-3ae2fbad7cd3 |
| ManagedTenants.ReadWrite.All                            | 委派   | b31fa710-c9b3-4d9e-8f5e-8036eecddab9 |
| Member.Read.Hidden                                      | 应用程序 | 658aa5d8-239f-45c4-aa12-864f4fc7e490 |
| Member.Read.Hidden                                      | 委派   | f6a3db3e-f7e8-4ed2-a414-557c8c9830be |
| Notes.Create                                            | 委派   | 9d822255-d64d-4b7a-afdb-833b9a97ed02 |
| Notes.Read                                              | 委派   | 371361e4-b9e2-4a3f-8315-2a301a3b0a3d |
| Notes.Read.All                                          | 应用程序 | 3aeca27b-ee3a-4c2b-8ded-80376e2134a4 |
| Notes.Read.All                                          | 委派   | dfabfca6-ee36-4db2-8208-7a28381419b3 |
| Notes.ReadWrite                                         | 委派   | 615e26af-c38a-4150-ae3e-c3b0d4cb1d6a |
| Notes.ReadWrite.All                                     | 应用程序 | 0c458cef-11f3-48c2-a568-c66751c238c0 |
| Notes.ReadWrite.All                                     | 委派   | 64ac0503-b4fa-45d9-b544-71a463f05da0 |
| Notes.ReadWrite.CreatedByApp                            | 委派   | ed68249d-017c-4df5-9113-e684c7f8760b |
| Notifications.ReadWrite.CreatedByApp                    | 委派   | 89497502-6e42-46a2-8cb2-427fd3df970a |
| offline_access                                          | 委派   | 7427e0e9-2fba-42fe-b0c0-848c9e6a8182 |
| OnlineMeetingArtifact.Read.All                          | 应用程序 | df01ed3b-eb61-4eca-9965-6b3d789751b2 |
| OnlineMeetingArtifact.Read.All                          | 委派   | 110e5abb-a10c-4b59-8b55-9b4daa4ef743 |
| OnlineMeetings.Read                                     | 委派   | 9be106e1-f4e3-4df5-bdff-e4bc531cbe43 |
| OnlineMeetings.Read.All                                 | 应用程序 | c1684f21-1984-47fa-9d61-2dc8c296bb70 |
| OnlineMeetings.ReadWrite                                | 委派   | a65f2972-a4f8-4f5e-afd7-69ccb046d5dc |
| OnlineMeetings.ReadWrite.All                            | 应用程序 | b8bb2037-6e08-44ac-a4ea-4674e010e2a4 |
| OnPremisesPublishingProfiles.ReadWrite.All              | 应用程序 | 0b57845e-aa49-4e6f-8109-ce654fffa618 |
| OnPremisesPublishingProfiles.ReadWrite.All              | 委派   | 8c4d5184-71c2-4bf8-bb9d-bc3378c9ad42 |
| openid                                                  | 委派   | 37f7f235-527c-4136-accd-4a02d197296e |
| Organization.Read.All                                   | 应用程序 | 498476ce-e0fe-48b0-b801-37ba7e2685c6 |
| Organization.Read.All                                   | 委派   | 4908d5b9-3fb2-4b1e-9336-1888b7937185 |
| Organization.ReadWrite.All                              | 应用程序 | 292d869f-3427-49a8-9dab-8c70152b74e9 |
| Organization.ReadWrite.All                              | 委派   | 46ca0847-7e6b-426e-9775-ea810a948356 |
| OrgContact.Read.All                                     | 应用程序 | e1a88a34-94c4-4418-be12-c87b00e26bea |
| OrgContact.Read.All                                     | 委派   | 08432d1b-5911-483c-86df-7980af5cdee0 |
| People.Read                                             | 委派   | ba47897c-39ec-4d83-8086-ee8256fa737d |
| People.Read.All                                         | 应用程序 | b528084d-ad10-4598-8b93-929746b4d7d6 |
| People.Read.All                                         | 委派   | b89f9189-71a5-4e70-b041-9887f0bc7e4a |
| Place.Read                                              | 委派   | 40f6bacc-b201-40da-90a5-09775cc4a863 |
| Place.Read.All                                          | 应用程序 | 913b9306-0ce1-42b8-9137-6a7df690a760 |
| Place.Read.All                                          | 委派   | cb8f45a0-5c2e-4ea1-b803-84b870a7d7ec |
| Place.Read.Shared                                       | 委派   | 0b3f56bc-fecd-4036-8930-660fc672e342 |
| Place.ReadWrite                                         | 委派   | 012ba4a5-ca82-4a76-95ba-6c27f44364c3 |
| Place.ReadWrite.All                                     | 委派   | 4c06a06a-098a-4063-868e-5dfee3827264 |
| Policy.Read.All                                         | 应用程序 | 246dd0d5-5bd0-4def-940b-0421030a5b68 |
| Policy.Read.All                                         | 委派   | 572fea84-0151-49b2-9301-11cb16974376 |
| Policy.Read.ConditionalAccess                           | 应用程序 | 37730810-e9ba-4e46-b07e-8ca78d182097 |
| Policy.Read.ConditionalAccess                           | 委派   | 633e0fce-8c58-4cfb-9495-12bbd5a24f7c |
| Policy.Read.PermissionGrant                             | 应用程序 | 9e640839-a198-48fb-8b9a-013fd6f6cbcd |
| Policy.Read.PermissionGrant                             | 委派   | 414de6ea-2d92-462f-b120-6e2a809a6d01 |
| Policy.ReadWrite.ApplicationConfiguration               | 应用程序 | be74164b-cff1-491c-8741-e671cb536e13 |
| Policy.ReadWrite.ApplicationConfiguration               | 委派   | b27add92-efb2-4f16-84f5-8108ba77985c |
| Policy.ReadWrite.AuthenticationFlows                    | 应用程序 | 25f85f3c-f66c-4205-8cd5-de92dd7f0cec |
| Policy.ReadWrite.AuthenticationFlows                    | 委派   | edb72de9-4252-4d03-a925-451deef99db7 |
| Policy.ReadWrite.AuthenticationMethod                   | 应用程序 | 29c18626-4985-4dcd-85c0-193eef327366 |
| Policy.ReadWrite.AuthenticationMethod                   | 委派   | 7e823077-d88e-468f-a337-e18f1f0e6c7c |
| Policy.ReadWrite.Authorization                          | 应用程序 | fb221be6-99f2-473f-bd32-01c6a0e9ca3b |
| Policy.ReadWrite.Authorization                          | 委派   | edd3c878-b384-41fd-95ad-e7407dd775be |
| Policy.ReadWrite.ConditionalAccess                      | 应用程序 | 01c0a623-fc9b-48e9-b794-0756f8e8f067 |
| Policy.ReadWrite.ConditionalAccess                      | 委派   | ad902697-1014-4ef5-81ef-2b4301988e8c |
| Policy.ReadWrite.ConsentRequest                         | 应用程序 | 999f8c63-0a38-4f1b-91fd-ed1947bdd1a9 |
| Policy.ReadWrite.ConsentRequest                         | 委派   | 4d135e65-66b8-41a8-9f8b-081452c91774 |
| Policy.ReadWrite.CrossTenantAccess                      | 应用程序 | 338163d7-f101-4c92-94ba-ca46fe52447c |
| Policy.ReadWrite.CrossTenantAccess                      | 委派   | 014b43d0-6ed4-4fc6-84dc-4b6f7bae7d85 |
| Policy.ReadWrite.DeviceConfiguration                    | 委派   | 40b534c3-9552-4550-901b-23879c90bcf9 |
| Policy.ReadWrite.FeatureRollout                         | 应用程序 | 2044e4f1-e56c-435b-925c-44cd8f6ba89a |
| Policy.ReadWrite.FeatureRollout                         | 委派   | 92a38652-f13b-4875-bc77-6e1dbb63e1b2 |
| Policy.ReadWrite.MobilityManagement                     | 委派   | a8ead177-1889-4546-9387-f25e658e2a79 |
| Policy.ReadWrite.PermissionGrant                        | 应用程序 | a402ca1c-2696-4531-972d-6e5ee4aa11ea |
| Policy.ReadWrite.PermissionGrant                        | 委派   | 2672f8bb-fd5e-42e0-85e1-ec764dd2614e |
| Policy.ReadWrite.TrustFramework                         | 应用程序 | 79a677f7-b79d-40d0-a36a-3e6f8688dd7a |
| Policy.ReadWrite.TrustFramework                         | 委派   | cefba324-1a70-4a6e-9c1d-fd670b7ae392 |
| POP.AccessAsUser.All                                    | 委派   | d7b7f2d9-0f45-4ea1-9d42-e50810c06991 |
| Presence.Read                                           | 委派   | 76bc735e-aecd-4a1d-8b4c-2b915deabb79 |
| Presence.Read.All                                       | 委派   | 9c7a330d-35b3-4aa1-963d-cb2b9f927841 |
| Presence.ReadWrite                                      | 委派   | 8d3c54a7-cf58-4773-bf81-c0cd6ad522bb |
| Presence.ReadWrite.All                                  | 应用程序 | 83cded22-8297-4ff6-a7fa-e97e9545a259 |
| PrintConnector.Read.All                                 | 委派   | d69c2d6d-4f72-4f99-a6b9-663e32f8cf68 |
| PrintConnector.ReadWrite.All                            | 委派   | 79ef9967-7d59-4213-9c64-4b10687637d8 |
| Printer.Create                                          | 委派   | 90c30bed-6fd1-4279-bf39-714069619721 |
| Printer.FullControl.All                                 | 委派   | 93dae4bd-43a1-4a23-9a1a-92957e1d9121 |
| Printer.Read.All                                        | 应用程序 | 9709bb33-4549-49d4-8ed9-a8f65e45bb0f |
| Printer.Read.All                                        | 委派   | 3a736c8a-018e-460a-b60c-863b2683e8bf |
| Printer.ReadWrite.All                                   | 应用程序 | f5b3f73d-6247-44df-a74c-866173fddab0 |
| Printer.ReadWrite.All                                   | 委派   | 89f66824-725f-4b8f-928e-e1c5258dc565 |
| PrinterShare.Read.All                                   | 委派   | ed11134d-2f3f-440d-a2e1-411efada2502 |
| PrinterShare.ReadBasic.All                              | 委派   | 5fa075e9-b951-4165-947b-c63396ff0a37 |
| PrinterShare.ReadWrite.All                              | 委派   | 06ceea37-85e2-40d7-bec3-91337a46038f |
| PrintJob.Create                                         | 委派   | 21f0d9c0-9f13-48b3-94e0-b6b231c7d320 |
| PrintJob.Manage.All                                     | 应用程序 | 58a52f47-9e36-4b17-9ebe-ce4ef7f3e6c8 |
| PrintJob.Read                                           | 委派   | 248f5528-65c0-4c88-8326-876c7236df5e |
| PrintJob.Read.All                                       | 应用程序 | ac6f956c-edea-44e4-bd06-64b1b4b9aec9 |
| PrintJob.Read.All                                       | 委派   | afdd6933-a0d8-40f7-bd1a-b5d778e8624b |
| PrintJob.ReadBasic                                      | 委派   | 6a71a747-280f-4670-9ca0-a9cbf882b274 |
| PrintJob.ReadBasic.All                                  | 应用程序 | fbf67eee-e074-4ef7-b965-ab5ce1c1f689 |
| PrintJob.ReadBasic.All                                  | 委派   | 04ce8d60-72ce-4867-85cf-6d82f36922f3 |
| PrintJob.ReadWrite                                      | 委派   | b81dd597-8abb-4b3f-a07a-820b0316ed04 |
| PrintJob.ReadWrite.All                                  | 应用程序 | 5114b07b-2898-4de7-a541-53b0004e2e13 |
| PrintJob.ReadWrite.All                                  | 委派   | 036b9544-e8c5-46ef-900a-0646cc42b271 |
| PrintJob.ReadWriteBasic                                 | 委派   | 6f2d22f2-1cb6-412c-a17c-3336817eaa82 |
| PrintJob.ReadWriteBasic.All                             | 应用程序 | 57878358-37f4-4d3a-8c20-4816e0d457b1 |
| PrintJob.ReadWriteBasic.All                             | 委派   | 3a0db2f6-0d2a-4c19-971b-49109b19ad3d |
| PrintSettings.Read.All                                  | 应用程序 | b5991872-94cf-4652-9765-29535087c6d8 |
| PrintSettings.Read.All                                  | 委派   | 490f32fd-d90f-4dd7-a601-ff6cdc1a3f6c |
| PrintSettings.ReadWrite.All                             | 委派   | 9ccc526a-c51c-4e5c-a1fd-74726ef50b8f |
| PrintTaskDefinition.ReadWrite.All                       | 应用程序 | 456b71a7-0ee0-4588-9842-c123fcc8f664 |
| PrivilegedAccess.Read.AzureAD                           | 应用程序 | 4cdc2547-9148-4295-8d11-be0db1391d6b |
| PrivilegedAccess.Read.AzureAD                           | 委派   | b3a539c9-59cb-4ad5-825a-041ddbdc2bdb |
| PrivilegedAccess.Read.AzureADGroup                      | 应用程序 | 01e37dc9-c035-40bd-b438-b2879c4870a6 |
| PrivilegedAccess.Read.AzureADGroup                      | 委派   | d329c81c-20ad-4772-abf9-3f6fdb7e5988 |
| PrivilegedAccess.Read.AzureResources                    | 应用程序 | 5df6fe86-1be0-44eb-b916-7bd443a71236 |
| PrivilegedAccess.Read.AzureResources                    | 委派   | 1d89d70c-dcac-4248-b214-903c457af83a |
| PrivilegedAccess.ReadWrite.AzureAD                      | 应用程序 | 854d9ab1-6657-4ec8-be45-823027bcd009 |
| PrivilegedAccess.ReadWrite.AzureAD                      | 委派   | 3c3c74f5-cdaa-4a97-b7e0-4e788bfcfb37 |
| PrivilegedAccess.ReadWrite.AzureADGroup                 | 应用程序 | 2f6817f8-7b12-4f0f-bc18-eeaf60705a9e |
| PrivilegedAccess.ReadWrite.AzureADGroup                 | 委派   | 32531c59-1f32-461f-b8df-6f8a3b89f73b |
| PrivilegedAccess.ReadWrite.AzureResources               | 应用程序 | 6f9d5 abc-2db6-400b-a267-7de22a40fb87 |
| PrivilegedAccess.ReadWrite.AzureResources               | 委派   | a84a9652-ffd3-496e-a991-22ba5529156a |
| 个人资料                                                 | 委派   | 14dad69e-099b-42c9-810b-d002981feec1 |
| ProgramControl.Read.All                                 | 应用程序 | eedb7fdd-7539-4345-a38b-4839e4a84cbd |
| ProgramControl.Read.All                                 | 委派   | c492a2e1-2f8f-4caa-b076-99bbf6e40fe4 |
| ProgramControl.ReadWrite.All                            | 应用程序 | 60a901ed-09f7-4aa5-a16e-7dd3d6f9de36 |
| ProgramControl.ReadWrite.All                            | 委派   | 50fd364f-9d93-4ae1-b170-300e87cccf84 |
| Reports.Read.All                                        | 应用程序 | 230c1aed-a721-4c5d-9cb4-a90514e508ef |
| Reports.Read.All                                        | 委派   | 02e97553-ed7b-43d0-ab3c-f8bace0d040c |
| RoleAssignmentSchedule.Read.Directory                   | 委派   | 344a729c-0285-42c6-9014-f12b9b8d6129 |
| RoleAssignmentSchedule.ReadWrite.Directory              | 委派   | 8c026be3-8e26-4774-9372-8d5d6f21daff |
| RoleEligibilitySchedule.Read.Directory                  | 委派   | eb0788c2-6d4e-4658-8c9e-c0fb8053f03d |
| RoleEligibilitySchedule.ReadWrite.Directory             | 委派   | 62ade113-f8e0-4bf9-a6ba-5acb31db32fd |
| RoleManagement.Read.All                                 | 应用程序 | c7fbd983-d9aa-4fa7-84b8-17382c103bc4 |
| RoleManagement.Read.All                                 | 委派   | 48fec646-b2ba-4019-8681-8eb31435aded |
| RoleManagement.Read.CloudPC                             | 应用程序 | 031a549a-bb80-49b6-8032-2068448c6a3c |
| RoleManagement.Read.CloudPC                             | 委派   | 9619b88a-8a25-48a7-9571-d23be0337a79 |
| RoleManagement.Read.Directory                           | 应用程序 | 483bed4a-2ad3-4361-a73b-c83ccdbdc53c |
| RoleManagement.Read.Directory                           | 委派   | 741c54c3-0c1e-44a1-818b-3f97ab4e8c83 |
| RoleManagement.ReadWrite.CloudPC                        | 应用程序 | 274d0592-d1b6-44bd-af1d-26d259bcb43a |
| RoleManagement.ReadWrite.CloudPC                        | 委派   | 501d06f8-07b8-4f18-b5c6-c191a4af7a82 |
| RoleManagement.ReadWrite.Directory                      | 应用程序 | 9e3f62cf-ca93-4989-b6ce-bf83c28f9fe8 |
| RoleManagement.ReadWrite.Directory                      | 委派   | d01b97e9-cbc0-49fe-810a-750afd5527a3 |
| RoleManagementPolicy.Read.Directory                     | 委派   | 3de2cdbe-0ff5-47d5-bdee-7f45b4749ead |
| RoleManagementPolicy.ReadWrite.Directory                | 委派   | 1ff1be21-34eb-448c-9ac9-ce1f506b2a68 |
| Schedule.Read.All                                       | 应用程序 | 7b2ebf90-d836-437f-b90d-7b62722c4456 |
| Schedule.Read.All                                       | 委派   | fccf6dd8-5706-49fa-811f-69e2e1b585d0 |
| Schedule.ReadWrite.All                                  | 应用程序 | b7760610-0545-4e8a-9ec3-cce9e63db01c |
| Schedule.ReadWrite.All                                  | 委派   | 63f27281-c9d9-4f29-94dd-6942f7f1feb0 |
| SearchConfiguration.Read.All                            | 应用程序 | ada977a5-b8b1-493b-9a91-66c206d76ecf |
| SearchConfiguration.Read.All                            | 委派   | 7d307522-aa38-4cd0-bd60-90c6f0ac50bd |
| SearchConfiguration.ReadWrite.All                       | 应用程序 | 0e778b85-fefa-466d-9eec-750569d92122 |
| SearchConfiguration.ReadWrite.All                       | 委派   | b1a7d408-cab0-47d2-a2a5-a74a3733600d |
| SecurityActions.Read.All                                | 应用程序 | 5e0edab9-c148-49d0-b423-ac253e121825 |
| SecurityActions.Read.All                                | 委派   | 1638cddf-07a4-4de2-8645-69c96cacad73 |
| SecurityActions.ReadWrite.All                           | 应用程序 | f2bf083f-0179-402a-bedb-b2784de8a49b |
| SecurityActions.ReadWrite.All                           | 委派   | dc38509c-b87d-4da0-bd92-6bec988bac4a |
| SecurityAlert.Read.All                                  | 应用程序 | 472e4a4d-bb4a-4026-98d1-0b0d74cb74a5 |
| SecurityAlert.Read.All                                  | 委派   | bc257fb8-46b4-4b15-8713-01e91bfbe4ea |
| SecurityAlert.ReadWrite.All                             | 应用程序 | ed4fca05-be46-441f-9803-1873825f8f8fdb |
| SecurityAlert.ReadWrite.All                             | 委派   | 471f2a7f-2a42-4d45-a2bf-594d0838070d |
| SecurityEvents.Read.All                                 | 应用程序 | bf394140-e372-4bf9-a898-299cfc7564e5 |
| SecurityEvents.Read.All                                 | 委派   | 64733abd-851e-478a-bffb-e47a14b18235 |
| SecurityEvents.ReadWrite.All                            | 应用程序 | d903a879-88e0-4c09-b0c9-82f6a1333f84 |
| SecurityEvents.ReadWrite.All                            | 委派   | 6aedf524-7e1c-45a7-bd76-ded8cab8d0fc |
| SecurityIncident.Read.All                               | 应用程序 | 45cc0394-e837-488b-a098-1918f48d186c |
| SecurityIncident.Read.All                               | 委派   | b9abcc4f-94fc-4457-9141-d20ce80ec952 |
| SecurityIncident.ReadWrite.All                          | 应用程序 | 34bf0e97-1971-4929-b999-9e2442d941d7 |
| SecurityIncident.ReadWrite.All                          | 委派   | 128ca929-1a19-45e6-a3b8-435ec44a36ba |
| ServiceHealth.Read.All                                  | 应用程序 | 79c261e0-fe76-4144-aad5-bdc68fbe4037 |
| ServiceHealth.Read.All                                  | 委派   | 55896846-df78-47a7-aa94-8d3d4442ca7f |
| ServiceMessage.Read.All                                 | 应用程序 | 1b620472-6534-4fe6-9df2-4680e8aa28ec |
| ServiceMessage.Read.All                                 | 委派   | eda39fa6-f8cf-4c3c-a909-432c683e4c9b |
| ServiceMessageViewpoint.Write                           | 委派   | 636e1b0b-1cc2-4b1c-9aa9-4eeed9b9761b |
| ServicePrincipalEndpoint.Read.All                       | 应用程序 | 5256681e-b7f6-40c0-8447-2d9db68797a0 |
| ServicePrincipalEndpoint.Read.All                       | 委派   | 9f9ce928-e038-4e3b-8faf-7b59049a8ddc |
| ServicePrincipalEndpoint.ReadWrite.All                  | 应用程序 | 89c8469c-83ad-45f7-8ff2-6e3d4285709e |
| ServicePrincipalEndpoint.ReadWrite.All                  | 委派   | 7297d82c-9546-4aed-91df-3d4f0a9b3ff0 |
| SharePointTenantSettings.Read.All                       | 应用程序 | 83d4163d-a2d8-4d3b-9695-4ae3ca98f888 |
| SharePointTenantSettings.Read.All                       | 委派   | 2ef70e10-5bfd-4ede-a5f6-67720500b258 |
| SharePointTenantSettings.ReadWrite.All                  | 应用程序 | 19b94e34-907c-4f43-bde9-38b1909ed408 |
| SharePointTenantSettings.ReadWrite.All                  | 委派   | aa07f155-3612-49b8-a147-6c590df35536 |
| ShortNotes.Read                                         | 委派   | 50f66e47-eb56-45b7-aaa2-75057d9afe08 |
| ShortNotes.Read.All                                     | 应用程序 | 0c7d31ec-31ca-4f58-b6ec-9950b6b0de69 |
| ShortNotes.ReadWrite                                    | 委派   | 328438b7-4c01-4c07-a840-e625a749bb89 |
| ShortNotes.ReadWrite.All                                | 应用程序 | 842c284c-763d-4a97-838d-79787d129bab |
| Sites.FullControl.All                                   | 应用程序 | a82116e5-55eb-4c41-a434-62fe8a61c773 |
| Sites.FullControl.All                                   | 委派   | 5a54b8b3-347c-476d-8f8e-42d5c7424d29 |
| Sites.Manage.All                                        | 应用程序 | 0c0bf378-bf22-4481-8f81-9e89a9b4960a |
| Sites.Manage.All                                        | 委派   | 65e50fdc-43b7-4915-933e-e8138f11f40a |
| Sites.Read.All                                          | 应用程序 | 332a536c-c7ef-4017-ab91-336970924f0d |
| Sites.Read.All                                          | 委派   | 205e70e5-aba6-4c52-a976-6d2d46c48043 |
| Sites.ReadWrite.All                                     | 应用程序 | 9492366f-7969-46a4-8d15-ed1a20078fff |
| Sites.ReadWrite.All                                     | 委派   | 89fe6a52-be36-487e-b7d8-d061c450a026 |
| Sites.Selected                                          | 应用程序 | 883ea226-0bf2-4a8f-9f9d-92c9162a727d |
| SMTP.Send                                               | 委派   | 258f6531-6087-4cc4-bb90-092c5fb3ed3f |
| SubjectRightsRequest.Read.All                           | 委派   | 9c3af74c-fd0f-4db4-b17a-71939e2a9d77 |
| SubjectRightsRequest.ReadWrite.All                      | 委派   | 2b8fcc74-bce1-4ae3-a0e8-60c53739299d |
| Subscription.Read.All                                   | 委派   | 5f88184c-80bb-4d52-9ff2-757288b2e9b7 |
| Tasks.Read                                              | 委派   | f45671fb-e0fe-4b4b-be20-3d3ce43f1bcb |
| Tasks.Read.Shared                                       | 委派   | 88d21fd4-8e5a-4c32-b5e2-4a1c95f34f72 |
| Tasks.ReadWrite                                         | 委派   | 2219042f-cab5-40cc-b0d2-16b1540b4c5f |
| Tasks.ReadWrite.Shared                                  | 委派   | c5ddf11b-c114-4886-8558-8a4e557cd52b |
| Team.Create                                             | 应用程序 | 23fc2474-f741-46ce-8465-674744c5c361 |
| Team.Create                                             | 委派   | 7825d5d6-6049-4ce7-bdf6-3b8d53f4bcd0 |
| Team.ReadBasic.All                                      | 应用程序 | 2280dda6-0bfd-44ee-a2f4-cb867cfc4c1e |
| Team.ReadBasic.All                                      | 委派   | 485be79e-c497-4b35-9400-0e3fa7f2a5d4 |
| TeamMember.Read.All                                     | 应用程序 | 660b7406-55f1-41ca-a0ed-0b035e182f3e |
| TeamMember.Read.All                                     | 委派   | 2497278c-d82d-46a2-b1ce-39d4cdde5570 |
| TeamMember.ReadWrite.All                                | 应用程序 | 0121dc95-1b9f-4aed-8bac-58c5ac466691 |
| TeamMember.ReadWrite.All                                | 委派   | 4a06efd2-f825-4e34-813e-82a57b03d1ee |
| TeamMember.ReadWriteNonOwnerRole.All                    | 应用程序 | 4437522e-9a86-4a41-a7da-e380edd4a97d |
| TeamMember.ReadWriteNonOwnerRole.All                    | 委派   | 2104a4db-3a2f-4ea0-9dba-143d457dc666 |
| TeamsActivity.Read                                      | 委派   | 0e755559-83fb-4b44-91d0-4cc721b9323e |
| TeamsActivity.Read.All                                  | 应用程序 | 70dec828-f620-4914-aa83-a29117306807 |
| TeamsActivity.Send                                      | 应用程序 | a267235f-af13-44dc-8385-c1dc93023186 |
| TeamsActivity.Send                                      | 委派   | 7ab1d787-bae7-4d5d-8db6-37ea32df9186 |
| TeamsApp.Read                                           | 委派   | daef10fc-047a-48b0-b1a5-da4b5e72fabc |
| TeamsApp.Read.All                                       | 应用程序 | afdb422a-4b2a-4e07-a708-8ceed48196bf |
| TeamsApp.Read.All                                       | 委派   | 9127ba42-f79f-43b1-be80-f23ecd42377e |
| TeamsApp.ReadWrite                                      | 委派   | 2a5addc2-4d9e-4d7d-8527-5215aec410f3 |
| TeamsApp.ReadWrite.All                                  | 应用程序 | eb6b3d76-ed75-4be6-ac36-158d04c0a555 |
| TeamsApp.ReadWrite.All                                  | 委派   | d3f0af02-b22d-4778-a433-14f7e3f2e1e2 |
| TeamsAppInstallation.ReadForChat                        | 委派   | bf3fbf03-f35f-4e93-963e-47e4d874c37a |
| TeamsAppInstallation.ReadForChat.All                    | 应用程序 | cc7e7635-2586-41d6-adaa-a8d3bcad5ee5 |
| TeamsAppInstallation.ReadForTeam                        | 委派   | 5248dcb1-f83b-4ec3-9f4d-a4428a961a72 |
| TeamsAppInstallation.ReadForTeam.All                    | 应用程序 | 1f615aea-6bf9-4b05-84bd-46388e138537 |
| TeamsAppInstallation.ReadForUser                        | 委派   | c395395c-ff9a-4dba-bc1f-8372ba9dca84 |
| TeamsAppInstallation.ReadForUser.All                    | 应用程序 | 9ce09611-f4f7-4abd-a629-a05450422a97 |
| TeamsAppInstallation.ReadWriteForChat                   | 委派   | aa85bf13-d771-4d5d-a9e6-bca04ce44edf |
| TeamsAppInstallation.ReadWriteForChat.All               | 应用程序 | 9e19bae1-2623-4c4f-ab6e-2664615ff9a0 |
| TeamsAppInstallation.ReadWriteForTeam                   | 委派   | 2e25a044-2580-450d-8859-42eeb6e996c0 |
| TeamsAppInstallation.ReadWriteForTeam.All               | 应用程序 | 5dad17ba-f6cc-4954-a5a2-a0dcc95154f0 |
| TeamsAppInstallation.ReadWriteForUser                   | 委派   | 093f8818-d05f-49b8-95bc-9d2a73e9a43c |
| TeamsAppInstallation.ReadWriteForUser.All               | 应用程序 | 74ef0291-ca83-4d02-8c7e-d2391e6a444f |
| TeamsAppInstallation.ReadWriteSelfForChat               | 委派   | 0ce33576-30e8-43b7-99e5-62f8569a4002 |
| TeamsAppInstallation.ReadWriteSelfForChat.All           | 应用程序 | 73a45059-f39c-4baf-9182-4954ac0e55cf |
| TeamsAppInstallation.ReadWriteSelfForTeam               | 委派   | 0f4595f7-64b1-4e13-81bc-11a249df07a9 |
| TeamsAppInstallation.ReadWriteSelfForTeam.All           | 应用程序 | 9f67436c-5415-4e7f-8ac1-3014a7132630 |
| TeamsAppInstallation.ReadWriteSelfForUser               | 委派   | 207e0cb1-3ce7-4922-b991-5a760c346ebc |
| TeamsAppInstallation.ReadWriteSelfForUser.All           | 应用程序 | 908de74d-f8b2-4d6b-a9ed-2a17b3b78179 |
| TeamSettings.Read.All                                   | 应用程序 | 242607bd-1d2c-432c-82eb-bdb27baa23ab |
| TeamSettings.Read.All                                   | 委派   | 48638b3c-ad68-4383-8ac4-e6880ee6ca57 |
| TeamSettings.ReadWrite.All                              | 应用程序 | bdd80a03-d9bc-451d-b7c4-ce7c63fe3c8f |
| TeamSettings.ReadWrite.All                              | 委派   | 39d65650-9d3e-4223-80db-a335590d027e |
| TeamsTab.Create                                         | 应用程序 | 49981c42-fd7b-4530-be03-e77b21aed25e |
| TeamsTab.Create                                         | 委派   | a9ff19c2-f369-4a95-9a25-ba9d460efc8e |
| TeamsTab.Read.All                                       | 应用程序 | 46890524-499a-4bb2-ad64-1476b4f3e1cf |
| TeamsTab.Read.All                                       | 委派   | 59dacb05-e88d-4c13-a684-59f1afc8cc98 |
| TeamsTab.ReadWrite.All                                  | 应用程序 | a96d855f-016b-47d7-b51c-1218a98d791c |
| TeamsTab.ReadWrite.All                                  | 委派   | b98bfd41-87c6-45cc-b104-e2de4f0dafb9 |
| TeamsTab.ReadWriteForChat                               | 委派   | ee928332-e9c2-4747-b4a0-f8c164b68de6 |
| TeamsTab.ReadWriteForChat.All                           | 应用程序 | fd9ce730-a250-40dc-bd44-8dc8d20f39ea |
| TeamsTab.ReadWriteForTeam                               | 委派   | c975dd04-a06e-4fbb-9704-62daad77bb49 |
| TeamsTab.ReadWriteForTeam.All                           | 应用程序 | 6163d4f4-fbf8-43da-a7b4-060fe85ed148 |
| TeamsTab.ReadWriteForUser                               | 委派   | c37c9b61-7762-4bff-a156-afc0005847a0 |
| TeamsTab.ReadWriteForUser.All                           | 应用程序 | 425b4b59-d5af-45c8-832f-bb0b7402348a |
| TeamsTab.ReadWriteSelfForChat                           | 委派   | 0c219d04-3abf-47f7-912d-5pga239e90e6 |
| TeamsTab.ReadWriteSelfForChat.All                       | 应用程序 | 9f62e4a2-a2d6-4350-b28b-d244728c4f86 |
| TeamsTab.ReadWriteSelfForTeam                           | 委派   | f266662f-120a-4314-b26a-99b08617c7ef |
| TeamsTab.ReadWriteSelfForTeam.All                       | 应用程序 | 91c32b81-0ef0-453f-a5c7-4ce2e562f449 |
| TeamsTab.ReadWriteSelfForUser                           | 委派   | 395dfec1-a0b9-465f-a783-8250a430cb8c |
| TeamsTab.ReadWriteSelfForUser.All                       | 应用程序 | 3c42dec6-49e8-4a0a-b469-36cff0d9da93 |
| Teamwork.Migrate.All                                    | 应用程序 | dfb0dd15-61de-45b2-be36-d6a69fba3c79 |
| TeamworkDevice.Read.All                                 | 应用程序 | 0591bafd-7c1c-4c30-a2a5-2b9aacb1dfe8 |
| TeamworkDevice.Read.All                                 | 委派   | b659488b-9d28-4208-b2be-1c6652b3c970 |
| TeamworkDevice.ReadWrite.All                            | 应用程序 | 79c02f5b-bd4f-4713-bc2c-a8a4a66e127b |
| TeamworkDevice.ReadWrite.All                            | 委派   | ddd97ecb-5c31-43db-a235-0ee20e635c40 |
| TeamworkTag.Read                                        | 委派   | 57587d0b-8399-45be-b207-8050cec54575 |
| TeamworkTag.Read.All                                    | 应用程序 | b74fd6c4-4bde-488e-9695-eeb100e4907f |
| TeamworkTag.ReadWrite                                   | 委派   | 539dabd7-b5b6-4117-b164-d60cd15a8671 |
| TeamworkTag.ReadWrite.All                               | 应用程序 | a3371ca5-911d-46d6-901c-42c8c7a937d8 |
| TermStore.Read.All                                      | 应用程序 | ea047cc2-df29-4f3e-83a3-205de61501ca |
| TermStore.Read.All                                      | 委派   | 297f747b-0005-475b-8fef-c890f5152b38 |
| TermStore.ReadWrite.All                                 | 应用程序 | f12eb8d6-28e3-46e6-b2c0-b7e4dc69fc95 |
| TermStore.ReadWrite.All                                 | 委派   | 6c37c71d-f50f-4bff-8fd3-8a41da390140 |
| ThreatAssessment.Read.All                               | 应用程序 | f8f035bb-2cce-47fb-8bf5-7baf3ecbee48 |
| ThreatAssessment.ReadWrite.All                          | 委派   | cac97e40-6730-457d-ad8d-4852fddab7ad |
| ThreatHunting.Read.All                                  | 应用程序 | dd98c7f5-2d42-42d3-a0e4-633161547251 |
| ThreatHunting.Read.All                                  | 委派   | b152eca8-ea73-4a48-8c98-1a6742673d99 |
| ThreatIndicators.Read.All                               | 应用程序 | 197ee4e9-b993-4066-898f-d6aecc55125b |
| ThreatIndicators.Read.All                               | 委派   | 9cc427b4-2004-41c5-aa22-757b755e9796 |
| ThreatIndicators.ReadWrite.OwnedBy                      | 应用程序 | 21792b6c-c986-4ffc-85de-df9da54b52fa |
| ThreatIndicators.ReadWrite.OwnedBy                      | 委派   | 91e7d36d-022a-490f-a748-f8e011357b42 |
| TrustFrameworkKeySet.Read.All                           | 应用程序 | fff194f1-7dce-4428-8301-1badb5518201 |
| TrustFrameworkKeySet.Read.All                           | 委派   | 7ad34336-f5b1-44ce-8682-31d7dfcd9ab9 |
| TrustFrameworkKeySet.ReadWrite.All                      | 应用程序 | 4a771c9a-1cf2-4609-b88e-3d3e02d539cd |
| TrustFrameworkKeySet.ReadWrite.All                      | 委派   | 39244520-1e7d-4b4a-aee0-57c65826e427 |
| UnifiedGroupMember.Read.AsGuest                         | 委派   | 73e75199-7c3e-41bb-9357-167164dbb415 |
| User.Export.All                                         | 应用程序 | 405a51b5-8d8d-430b-9842-8be4b0e9f324 |
| User.Export.All                                         | 委派   | 405a51b5-8d8d-430b-9842-8be4b0e9f324 |
| User.Invite.All                                         | 应用程序 | 09850681-111b-4a89-9bed-3f2cae46d706 |
| User.Invite.All                                         | 委派   | 63dd7cd9-b489-4adf-a28c-ac38b9a0f962 |
| User.ManageIdentities.All                               | 应用程序 | c529cfca-c91b-489c-af2b-d92990b66ce6 |
| User.ManageIdentities.All                               | 委派   | 637d7bec-b31e-4deb-acc9-24275642a2c9 |
| User.Read                                               | 委派   | e1fe6dd8-ba31-4d61-89e7-88639da4683d |
| User.Read.All                                           | 应用程序 | df021288-bdef-4463-88db-98f22de89214 |
| User.Read.All                                           | 委派   | a154be20-db9c-4678-8ab7-66f6cc099a59 |
| User.ReadBasic.All                                      | 委派   | b340eb25-3456-403f-be2f-af7a0d370277 |
| User.ReadWrite                                          | 委派   | b4e74841-8e56-480b-be8b-910348b18b4c |
| User.ReadWrite.All                                      | 应用程序 | 741f803b-c850-494e-b5df-cde7c675a1ca |
| User.ReadWrite.All                                      | 委派   | 204e0828-b5ca-4ad8-b9f3-f32a958e7cc4 |
| UserActivity.ReadWrite.CreatedByApp                     | 委派   | 47607519-5fb1-47d9-99c7-da4b48f369b1 |
| UserAuthenticationMethod.Read                           | 委派   | 1f6b61c5-2f65-4135-9c9f-31c0f8d32b52 |
| UserAuthenticationMethod.Read.All                       | 应用程序 | 38d9df27-64da-44fd-b7c5-a6fbac20248f |
| UserAuthenticationMethod.Read.All                       | 委派   | aec28ec7-4d02-4e8c-b864-50163aea77eb |
| UserAuthenticationMethod.ReadWrite                      | 委派   | 48971fc1-70d7-4245-af77-0beb29b53ee2 |
| UserAuthenticationMethod.ReadWrite.All                  | 应用程序 | 50483e42-d915-4231-9639-7fdb7fd190e5 |
| UserAuthenticationMethod.ReadWrite.All                  | 委派   | b7887744-6746-4312-813d-72daeaee7e2d |
| UserNotification.ReadWrite.CreatedByApp                 | 应用程序 | 4e774092-a092-48d1-90bd-baad67c7eb47 |
| UserNotification.ReadWrite.CreatedByApp                 | 委派   | 26e2f3e8-b2a1-47fc-9620-89bb5b042024 |
| UserShiftPreferences.Read.All                           | 应用程序 | de023814-96df-4f53-9376-1e2891ef5a18 |
| UserShiftPreferences.ReadWrite.All                      | 应用程序 | d1eec298-80f3-49b0-9efb-d90e224798ac |
| UserTimelineActivity.Write.CreatedByApp                 | 委派   | 367492fc-594d-4972-a9b5-0d58c622c91c |
| WindowsUpdates.ReadWrite.All                            | 应用程序 | 7dd1be58-6e76-4401-bf8d-31d1e8180d5b |
| WindowsUpdates.ReadWrite.All                            | 委派   | 11776c0c-6138-4db3-a668-ee621bea2555 |
| WorkforceIntegration.Read.All                           | 委派   | f1ccd5a7-6383-466a-8db8-1a656f7d06fa |
| WorkforceIntegration.ReadWrite.All                      | 应用程序 | 202bf709-e8e6-478e-bcfd-5d63c50b68e3 |
| WorkforceIntegration.ReadWrite.All                      | 委派   | 08c4b377-0d23-4a8b-be2a-23c1c1d88545 |
