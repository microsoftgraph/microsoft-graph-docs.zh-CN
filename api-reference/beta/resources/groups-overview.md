---
title: 在 Microsoft Graph 中使用组
description: 组是在 Microsoft 服务或你的应用中共享资源访问权限的主体集合。 不同的主体（如用户、其他组、设备和应用程序）构成组的各个部分。 使用组有助于避免使用单个主体，并简化资源的访问管理。
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: conceptualPageType
ms.openlocfilehash: 799fd82f5754d07a58fd570205f10fbe6d306f8a
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061130"
---
# <a name="working-with-groups-in-microsoft-graph"></a>在 Microsoft Graph 中使用组

组是在 Microsoft 服务或你的应用中共享资源访问权限的主体集合。 不同的主体（如用户、其他组、设备和应用程序）构成组的各个部分。 使用组有助于避免使用单个主体，并简化资源的访问管理。

Microsoft Graph 公开组 API，以创建和管理不同类型的组和组功能。 

> [!NOTE]
> 1. 组只能通过工作或学校帐户创建。 个人 Microsoft 帐户不支持组。
> 2. Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。

## <a name="group-types-in-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 中的组类型

Azure Active Directory (Azure AD) 支持以下类型的组。

- Microsoft 365 组
- 安全组
- 启用邮件功能的安全组
- 通讯组

只有 Microsoft 365 和安全组才能通过 Microsoft Graph 组 API 进行管理。 Microsoft Graph 的启用邮件和通讯组为只读模式。

在 Microsoft Graph 中，可以通过设置 **groupType**、**mailEnabled** 和 **securityEnabled** 属性来标识组类型，如下表所示。

| 类型 |groupType | mailEnabled | securityEnabled | 通过组 API 创建和管理 |
|--|--|--|--|--|
| [Microsoft 365 组](#microsoft-365-groups) | `["Unified"]` | `true` | `true` 或 `false` | 可访问 |
| [安全组](#security-groups-and-mail-enabled-security-groups) | `[]` | `false` | `true` | 是 |
| [启用邮件的安全组](#security-groups-and-mail-enabled-security-groups) | `[]` | `true` | `true` | 否 |
| 通讯组 | `[]` | `true` | `false` | 否 |

有关组的详细信息，请参阅以下部分。 有关 Azure AD 组的详细信息，请参阅[Azure AD 中的比较组](/microsoft-365/admin/create-groups/compare-groups)。

## <a name="microsoft-365-groups"></a>Microsoft 365 组

Microsoft 365 组的强大之处在于它的协作本质，它是项目或团队中相互协作的用户的理想之选。 它们由组成员共享的资源创建，包括：

- Outlook 对话
- Outlook 日历
- SharePoint 文件
- OneNote 笔记本
- SharePoint 团队网站
- Planner 计划
- Intune 设备管理

调用 Microsoft Graph 组 API 时，以下 JSON 对象显示组的示例表示形式。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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

**安全组** 用于控制用户对资源的访问。 通过检查用户是否是安全组的成员，应用可以在用户尝试访问应用中的某些安全资源时决定是否授权。 安全组的成员可以是用户、其他安全组、设备和服务主体。

**启用邮件的安全组** 的使用方式与安全组基本相同，不同之处在于添加了组的共享邮箱功能。 无法通过 API 创建或更新启用邮件的安全组；相反，它们为只读模式。 若要了解更多信息，请参阅 Exchange 文章[管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups)。

调用 Microsoft Graph 组 API 时，以下 JSON 对象显示组的示例表示形式。

```http
HTTP/1.1 201 Created
Content-type: application/json

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

## <a name="dynamic-membership"></a>动态成员身份

所有类型的组都可以有动态成员资格规则，用于根据主体属性自动在组中添加或删除成员。 例如，“营销员工”组可以定义动态成员身份规则，只有其部门属性设置为“市场营销”的用户才能成为该组的成员。 在这种情况下，离开部门的任何用户都会自动从组中删除。 

在创建组期间，通过 **membershipRule** 属性指定动态成员身份规则。 例如，`"membershipRule": 'user.department -eq "Marketing"'`。 **groupType** 属性还必须包含集合中的 `"DynamicMembership"` 值。 可以通过 **membershipRuleProcessingState** 属性打开或关闭动态成员身份规则。

以下示例请求创建一个新的 Microsoft 365 组，该组只能包含市场营销部门中的员工。

```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

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
    "membershipRule": "'user.department -eq 'Marketing'",
    "membershipRuleProcessingState": "on"
}
```

若要详细了解如何制定成员资格规则，请参阅 [Azure Active Directory 中组的动态成员资格规则](/azure/active-directory/enterprise-users/groups-dynamic-membership)。

> **注意**：动态成员身份规则要求租户至少为属于一个或多个动态组成员的每个唯一用户拥有 Azure AD Premium P1 许可证。

## <a name="other-types-of-groups"></a>其他类型的组

Yammer 中的 Microsoft 365 组用于通过 Yammer 帖子促进用户协作。 可以通过读取请求返回这种类型的组，但无法通过 API 访问它们的帖子。 如果对组启用了 Yammer 帖子和对话源，将会禁用默认的 Microsoft 365 组对话。 若要了解详细信息，请参阅 [Yammer 开发人员 API 文档](https://developer.yammer.com/docs)。

## <a name="group-search-limitations-for-guest-users-in-organizations"></a>组织中来宾用户的组搜索限制

组搜索功能允许应用对 `/groups` 资源(例如 `https://graph.microsoft.com/beta/groups`)执行查询，以搜索组织目录中的任何组。管理员和成员用户都具有此功能；但来宾用户没有。

如果登录用户是来宾用户，应用程序可以读取特定组的配置文件（例如，`https://graph.microsoft.com/beta/group/fc06287e-d082-4aab-9d5e-d6fd0ed7c8bc`），具体视应用程序获得的授权而定；不过，不能对可能返回多个资源的 `/groups` 资源执行查询。

借助授予的适当权限，应用程序可以读取组的配置文件，具体是通过导航属性中的链接获取；例如，`/groups/{id}/members`。

有关来宾用户可以对组执行的操作的详细信息，请参阅[比较成员和来宾默认权限](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions)。

## <a name="group-based-licensing"></a>基于组的许可

基于组的许可功能可以用于将一个或多个产品许可证分配给 Azure AD 组。 Azure AD 可确保许可证分配给组的所有成员。 任何加入该组的新成员都获得了相应的许可证。 他们离开组时，将移除这些许可证。 此功能只能与安全组和将 **securityEnabled** 属性设置为 `true` 的 Microsoft 365 组一起使用。 若要了解基于组的许可的详细信息，请参阅[什么是 Azure Active Directory 中基于组的许可？](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal?context=/azure/active-directory/enterprise-users/context/ugr-context)

## <a name="common-use-cases-for-the-groups-api-in-microsoft-graph"></a>Microsoft Graph 中组 API 的常见用例

使用 Microsoft Graph，可以执行下面的常见操作。

| **用例** | **REST 资源** | **另请参阅** |
|:-|:-|:-|
| **创建组、管理组特征** |  |  |
| 创建新组、获取现有组、更新组的属性和删除组。 目前，只有 Outlook 中的安全组和组才能通过 API 创建。 | [group](group.md) | [新建组](../api/group-post-groups.md) <br/> [列出组](../api/group-list.md) <br/> [更新组](../api/group-update.md) <br/> [删除组](../api/group-delete.md) |
| **管理组成员身份** |  |  |
| 列出组中的成员，并添加或删除成员。 | [user](user.md) <br/> [group](group.md) | [列出成员](../api/group-list-members.md) <br/> [添加成员](../api/group-post-members.md) <br/> [删除成员](../api/group-delete-members.md) |
| 确定用户是否是组成员，并获取用户所属的全部组。 | [user](user.md) <br/> [组](group.md) <br/> [servicePrincipal](serviceprincipal.md) <br/> [orgContact](orgcontact.md) | [检查成员组](../api/directoryobject-checkmembergroups.md) <br/> [获取成员组](../api/directoryobject-getmembergroups.md) |
| 列出组的所有者，并添加或删除所有者。 | [user](user.md) <br/> [group](group.md) | [列出所有者](../api/group-list-members.md) <br/> [添加成员](../api/group-post-members.md) <br/> [Remove member](../api/group-delete-members.md) |

## <a name="whats-new"></a>最近更新

了解组 API 的[最新功能和更新](/graph/whats-new-overview)。