---
title: 在 Microsoft Graph 中使用组
description: 组是用户和其他主体的集合，他们共享对 Microsoft 服务或应用中资源的访问权限。 Microsoft Graph 提供了可用于根据方案创建和管理不同类型组和组功能的 API。 Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 10f64d951a7fed740a3f947bf4aa1e3ed6153624
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587236"
---
# <a name="working-with-groups-in-microsoft-graph"></a>在 Microsoft Graph 中使用组

组是[用户](user.md)和其他主体的集合，他们共享对 Microsoft 服务或应用中资源的访问权限。 Microsoft Graph 提供了可用于根据方案创建和管理不同类型组和组功能的 API。 Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。

> [!NOTE]
> 组只能通过工作或学校帐户创建。 个人 Microsoft 帐户不支持组。

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 中的组类型

Azure AD 支持以下类型的组。

- Microsoft 365 组
- 安全组
- 启用邮件功能的安全组
- 通讯组

有关 Azure AD 组的详细信息，请参阅Azure AD 中的[比较组](/microsoft-365/admin/create-groups/compare-groups)。

在 Microsoft Graph 中，可以通过设置 **groupType**、**mailEnabled** 和 **securityEnabled** 属性来标识组类型，如下表所示。

| 类型                                                                              | 用例                                                                                                                                     | groupType     | mailEnabled | securityEnabled   | 通过 API 创建和管理 |
| --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ----------- | ----------------- | --------------------------- |
| [Microsoft 365 组](#microsoft-365-groups)                                     | 促进用户与共享 Microsoft Online 资源的协作。                                                                      | `["Unified"]` | `true`      | `true` 或 `false` | 可访问                         |
| [安全组](#security-groups-and-mail-enabled-security-groups)              | 控制用户对应用中资源的访问。                                                                                                 | `[]`          | `false`     | `true`            | 是                         |
| [启用邮件的安全组](#security-groups-and-mail-enabled-security-groups) | 使用共享的组邮箱，控制用户对应用中资源的访问。                                                                    | `[]`          | `true`      | `true`            | 否                          |
| 通讯组                                                               | 将邮件分发给组中的成员。 建议使用 Microsoft 365 组，因为它提供的资源集更丰富。 | `[]`          | `true`      | `false`           | 否                          |

## <a name="microsoft-365-groups"></a>Microsoft 365 组

Microsoft 365 组的强大之处在于它的协作本质，它是项目或团队中相互协作的用户的理想之选。 创建时，它们包含组成员共享的资源，包括：

- Outlook 对话
- Outlook 日历
- SharePoint 文件
- OneNote 笔记本
- SharePoint 团队网站
- Planner 计划
- Intune 设备管理

### <a name="group-in-outlook-example"></a>Outlook 中的组示例

下面是 Outlook 中组的 JSON 表示形式。

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

若要详细了解 Microsoft 365 组和管理员体验，请参阅[了解 Microsoft 365 组](https://support.office.com/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)。

## <a name="security-groups-and-mail-enabled-security-groups"></a>安全组和启用邮件的安全组

安全组用于控制用户对资源的访问。 通过检查用户是否是安全组的成员，应用可以在用户尝试访问应用中的某些安全资源时决定是否授权。 安全组的成员可以是用户和其他安全组。

启用邮件的安全组的使用方式与安全组基本相同，不同之处在于添加了组的共享邮箱功能。 无法通过 API 创建启用邮件的安全组，但其他组操作仍适用。 启用邮件的安全组为只读。 若要了解更多信息，请参阅 Exchange 文章[管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups)。

### <a name="security-group-example"></a>安全组示例

下面是安全组的 JSON 表示形式。

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```

## <a name="dynamic-membership"></a>动态成员资格

所有类型的组都可以有成员资格规则，用于根据用户属性自动在组中添加或删除成员。 例如，“市场营销部员工”组包含所有 department 属性设置为“Marketing”的用户，这样可以将新入职的市场营销部员工自动添加到组中，并自动在组中删除从市场营销部离职的员工。 在组创建期间，可以在“membershipRule”字段中将此规则指定为 `"membershipRule": 'user.department -eq "Marketing"'`。 GroupType 还必须包括 `"DynamicMembership"`。 下面的请求为市场营销部员工新建 Microsoft 365 组：

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

若要详细了解如何表述 membershipRules，请参阅[在 Azure Active Directory 中创建基于属性的动态组成员资格规则](/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)。

> **注意**：动态成员资格规则要求租户必须在 [Azure Active Directory Premium P1](https://azure.microsoft.com/pricing/details/active-directory/) 或更高层拥有许可证。

## <a name="other-types-of-groups"></a>其他类型的组

Yammer 中的 Microsoft 365 组用于通过 Yammer 帖子促进用户协作。 可以通过读取请求返回这种类型的组，但无法通过 API 访问它们的帖子。 如果对组启用了 Yammer 帖子和对话源，将会禁用默认的 Microsoft 365 组对话。 若要了解详细信息，请参阅 [Yammer 开发人员 API 文档](https://developer.yammer.com/docs)。

## <a name="group-based-licensing"></a>基于组的许可

基于组的许可功能可以用于将一个或多个产品许可证分配给 Azure AD 组。 Azure AD 可确保许可证分配给组的所有成员。 任何加入该组的新成员都获得了相应的许可证。 他们离开组时，将移除这些许可证。 该功能只能用于安全组和其中 securityEnabled=TRUE 的 Microsoft 365 组。 若要进一步了解基于组的许可，请参阅[此处](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。

## <a name="common-use-cases"></a>常见用例

使用 Microsoft Graph，可以执行下面的常见操作。

| **用例**                                                                                                                                                                     | **REST 资源**                                                                                                      | **另请参阅**                                                                                                                                                                           |
| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **组对象和方法**                                                                                                                                                      |                                                                                                                         |                                                                                                                                                                                        |
| 创建新组、获取现有组、更新组的属性和删除组。 目前，只有 Outlook 中的安全组和组才能通过 API 创建。 | [group](group.md)                                                                                                       | [新建组](../api/group-post-groups.md) <br/> [列出组](../api/group-list.md) <br/> [更新组](../api/group-update.md) <br/> [删除组](../api/group-delete.md) |
| **组成员资格方法**                                                                                                                                                      |                                                                                                                         |                                                                                                                                                                                        |
| 列出组中的成员，并添加或删除成员。                                                                                                                           | [user](user.md) <br/> [group](group.md)                                                                                 | [列出成员](../api/group-list-members.md) <br/> [添加成员](../api/group-post-members.md) <br/> [删除成员](../api/group-delete-members.md)                                    |
| 确定用户是否是组成员，并获取用户所属的全部组。                                                                                      | [user](user.md) <br/> [组](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md) | [检查成员组](../api/directoryobject-checkmembergroups.md) <br/> [获取成员组](../api/directoryobject-getmembergroups.md)                                                |
| 列出组的所有者，并添加或删除所有者。                                                                                                                             | [user](user.md) <br/> [group](group.md)                                                                                 | [列出所有者](../api/group-list-members.md) <br/> [添加成员](../api/group-post-members.md) <br/> [Remove member](../api/group-delete-members.md)                                     |

## <a name="whats-new"></a>最近更新

了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
