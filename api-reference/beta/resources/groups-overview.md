---
title: 在 Microsoft Graph 中使用组
description: 组是用户和其他主体的集合，他们共享对 Microsoft 服务或应用中资源的访问权限。 Microsoft Graph 提供了可用于根据方案创建和管理不同类型组和组功能的 API。 Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。
ms.openlocfilehash: f60d3faf8fd26c5ec4d1e962d11a4c29f4c1bf73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045768"
---
# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="3c29c-105">在 Microsoft Graph 中使用组</span><span class="sxs-lookup"><span data-stu-id="3c29c-105">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="3c29c-106">组是[用户](user.md)和其他主体的集合，他们共享对 Microsoft 服务或应用中资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3c29c-106">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="3c29c-107">Microsoft Graph 提供了可用于根据方案创建和管理不同类型组和组功能的 API。</span><span class="sxs-lookup"><span data-stu-id="3c29c-107">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="3c29c-108">Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。</span><span class="sxs-lookup"><span data-stu-id="3c29c-108">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="3c29c-109">**注意**：只能通过工作或学校帐户创建组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-109">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="3c29c-110">个人 Microsoft 帐户不支持组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-110">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="3c29c-111">类型</span><span class="sxs-lookup"><span data-stu-id="3c29c-111">Type</span></span>              | <span data-ttu-id="3c29c-112">用例</span><span class="sxs-lookup"><span data-stu-id="3c29c-112">Use case</span></span> | <span data-ttu-id="3c29c-113">groupType</span><span class="sxs-lookup"><span data-stu-id="3c29c-113">groupType</span></span> | <span data-ttu-id="3c29c-114">启用邮件</span><span class="sxs-lookup"><span data-stu-id="3c29c-114">mail-enabled</span></span> | <span data-ttu-id="3c29c-115">启用安全机制</span><span class="sxs-lookup"><span data-stu-id="3c29c-115">security-enabled</span></span> | <span data-ttu-id="3c29c-116">是否可通过 API 创建？</span><span class="sxs-lookup"><span data-stu-id="3c29c-116">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="3c29c-117">Office 365 组</span><span class="sxs-lookup"><span data-stu-id="3c29c-117">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="3c29c-118">促进用户与共享 Microsoft Online 资源的协作。</span><span class="sxs-lookup"><span data-stu-id="3c29c-118">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="3c29c-119">可访问</span><span class="sxs-lookup"><span data-stu-id="3c29c-119">Yes</span></span> |
| [<span data-ttu-id="3c29c-120">安全组</span><span class="sxs-lookup"><span data-stu-id="3c29c-120">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="3c29c-121">控制用户对应用中资源的访问。</span><span class="sxs-lookup"><span data-stu-id="3c29c-121">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="3c29c-122">是</span><span class="sxs-lookup"><span data-stu-id="3c29c-122">Yes</span></span> |
| [<span data-ttu-id="3c29c-123">启用邮件的安全组</span><span class="sxs-lookup"><span data-stu-id="3c29c-123">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="3c29c-124">使用共享的组邮箱，控制用户对应用中资源的访问。</span><span class="sxs-lookup"><span data-stu-id="3c29c-124">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="3c29c-125">否</span><span class="sxs-lookup"><span data-stu-id="3c29c-125">No</span></span> |
| <span data-ttu-id="3c29c-126">通讯组</span><span class="sxs-lookup"><span data-stu-id="3c29c-126">Distribution groups</span></span> | <span data-ttu-id="3c29c-127">将邮件分发给组中的成员。</span><span class="sxs-lookup"><span data-stu-id="3c29c-127">Distributing mail to the members of the group.</span></span> <span data-ttu-id="3c29c-128">建议使用 Office 365 组，因为它提供的资源集更丰富。</span><span class="sxs-lookup"><span data-stu-id="3c29c-128">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="3c29c-129">否</span><span class="sxs-lookup"><span data-stu-id="3c29c-129">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="3c29c-130">Office 365 组</span><span class="sxs-lookup"><span data-stu-id="3c29c-130">Office 365 groups</span></span>
<span data-ttu-id="3c29c-131">Office 365 组的强大之处在于它的协作本质，它是项目或团队中相互协作的用户的理想之选。</span><span class="sxs-lookup"><span data-stu-id="3c29c-131">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="3c29c-132">创建时，它们包含组成员共享的资源，包括：</span><span class="sxs-lookup"><span data-stu-id="3c29c-132">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="3c29c-133">Outlook 对话</span><span class="sxs-lookup"><span data-stu-id="3c29c-133">Outlook conversations</span></span>
- <span data-ttu-id="3c29c-134">Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="3c29c-134">Outlook calendar</span></span>
- <span data-ttu-id="3c29c-135">SharePoint 文件</span><span class="sxs-lookup"><span data-stu-id="3c29c-135">SharePoint files</span></span>
- <span data-ttu-id="3c29c-136">OneNote 笔记本</span><span class="sxs-lookup"><span data-stu-id="3c29c-136">OneNote notebook</span></span>
- <span data-ttu-id="3c29c-137">SharePoint 团队网站</span><span class="sxs-lookup"><span data-stu-id="3c29c-137">SharePoint team site</span></span>
- <span data-ttu-id="3c29c-138">Planner 计划</span><span class="sxs-lookup"><span data-stu-id="3c29c-138">Planner plans</span></span>
- <span data-ttu-id="3c29c-139">Intune 设备管理</span><span class="sxs-lookup"><span data-stu-id="3c29c-139">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="3c29c-140">Outlook 中的组示例</span><span class="sxs-lookup"><span data-stu-id="3c29c-140">Group in Outlook example</span></span>

<span data-ttu-id="3c29c-141">下面是 Outlook 中组的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c29c-141">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="3c29c-142">若要详细了解 Office 365 组和管理员体验，请参阅[了解 Office 365 组](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)。</span><span class="sxs-lookup"><span data-stu-id="3c29c-142">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="3c29c-143">安全组和启用邮件的安全组</span><span class="sxs-lookup"><span data-stu-id="3c29c-143">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="3c29c-144">安全组用于控制用户对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="3c29c-144">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="3c29c-145">通过检查用户是否是安全组的成员，应用可以在用户尝试访问应用中的某些安全资源时决定是否授权。</span><span class="sxs-lookup"><span data-stu-id="3c29c-145">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="3c29c-146">安全组的成员可以是用户和其他安全组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-146">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="3c29c-147">启用邮件的安全组的使用方式与安全组基本相同，不同之处在于添加了组的共享邮箱功能。</span><span class="sxs-lookup"><span data-stu-id="3c29c-147">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="3c29c-148">无法通过 API 创建启用邮件的安全组，但其他组操作仍适用。</span><span class="sxs-lookup"><span data-stu-id="3c29c-148">Mail-enabled security groups can't be created through the API, but other group operations work.</span></span> <span data-ttu-id="3c29c-149">启用邮件的安全组为只读。</span><span class="sxs-lookup"><span data-stu-id="3c29c-149">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="3c29c-150">若要了解更多信息，请参阅 Exchange 文章[管理启用邮件的安全组](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="3c29c-150">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="3c29c-151">安全组示例</span><span class="sxs-lookup"><span data-stu-id="3c29c-151">Security group example</span></span>

<span data-ttu-id="3c29c-152">下面是安全组的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c29c-152">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="3c29c-153">动态成员资格</span><span class="sxs-lookup"><span data-stu-id="3c29c-153">Dynamic membership</span></span> 

<span data-ttu-id="3c29c-154">所有类型的组都可以有成员资格规则，用于根据用户属性自动在组中添加或删除成员。</span><span class="sxs-lookup"><span data-stu-id="3c29c-154">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="3c29c-155">例如，“市场营销部员工”组包含所有 department 属性设置为“Marketing”的用户，这样可以将新入职的市场营销部员工自动添加到组中，并自动在组中删除从市场营销部离职的员工。</span><span class="sxs-lookup"><span data-stu-id="3c29c-155">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="3c29c-156">在组创建期间，可以在“membershipRule”字段中将此规则指定为 `"membershipRule": 'user.department -eq "Marketing"'`。</span><span class="sxs-lookup"><span data-stu-id="3c29c-156">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="3c29c-157">GroupType 还必须包括 `"DynamicMembership"`。</span><span class="sxs-lookup"><span data-stu-id="3c29c-157">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="3c29c-158">下面的请求为市场营销部员工新建 Office 365 组：</span><span class="sxs-lookup"><span data-stu-id="3c29c-158">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="3c29c-159">若要详细了解如何表述 membershipRules，请参阅[在 Azure Active Directory 中创建基于属性的动态组成员资格规则](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="3c29c-159">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="3c29c-160">**注意**：动态成员资格规则要求租户必须在 [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) 或更高层拥有许可证。</span><span class="sxs-lookup"><span data-stu-id="3c29c-160">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="3c29c-161">其他类型的组</span><span class="sxs-lookup"><span data-stu-id="3c29c-161">Other types of groups</span></span>

<span data-ttu-id="3c29c-162">Yammer 中的 office 365 组用于通过 Yammer 帖子促进用户协作。</span><span class="sxs-lookup"><span data-stu-id="3c29c-162">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="3c29c-163">可以通过读取请求返回这种类型的组，但无法通过 API 访问它们的帖子。</span><span class="sxs-lookup"><span data-stu-id="3c29c-163">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="3c29c-164">如果对组启用了 Yammer 帖子和对话源，将会禁用默认的 Office 365 组对话。</span><span class="sxs-lookup"><span data-stu-id="3c29c-164">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="3c29c-165">若要了解详细信息，请参阅 [Yammer 开发人员 API 文档](https://developer.yammer.com/docs)。</span><span class="sxs-lookup"><span data-stu-id="3c29c-165">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="group-based-licensing"></a><span data-ttu-id="3c29c-166">基于组的许可</span><span class="sxs-lookup"><span data-stu-id="3c29c-166">Group-based licensing</span></span> 

<span data-ttu-id="3c29c-167">基于组的许可功能可用于将一个或多个产品许可证分配给 Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-167">Group-based licensing capability can be used to assign one or more product licenses to an Azure AD group.</span></span> <span data-ttu-id="3c29c-168">Azure AD 确保许可证已分配给组的所有成员。</span><span class="sxs-lookup"><span data-stu-id="3c29c-168">Azure AD ensures that the licenses are assigned to all members of the group.</span></span> <span data-ttu-id="3c29c-169">加入的组的任何新成员分配相应的许可证。</span><span class="sxs-lookup"><span data-stu-id="3c29c-169">Any new members who join the group are assigned the appropriate licenses.</span></span> <span data-ttu-id="3c29c-170">当他们离开该组时，将删除这些许可证。</span><span class="sxs-lookup"><span data-stu-id="3c29c-170">When they leave the group, those licenses are removed.</span></span> <span data-ttu-id="3c29c-171">此功能仅可与安全组和 Office 365 组具有 securityEnabled = TRUE。</span><span class="sxs-lookup"><span data-stu-id="3c29c-171">The feature can only be used with security groups, and Office 365 groups that have securityEnabled=TRUE.</span></span> <span data-ttu-id="3c29c-172">若要了解有关基于组的许可，请参阅[此处](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="3c29c-172">To learn more about group-based licensing see [here](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="3c29c-173">常见用例</span><span class="sxs-lookup"><span data-stu-id="3c29c-173">Common use cases</span></span>

<span data-ttu-id="3c29c-174">使用 Microsoft Graph，可以执行下面的常见操作。</span><span class="sxs-lookup"><span data-stu-id="3c29c-174">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="3c29c-175">**用例**</span><span class="sxs-lookup"><span data-stu-id="3c29c-175">**Use cases**</span></span>  | <span data-ttu-id="3c29c-176">**REST 资源**</span><span class="sxs-lookup"><span data-stu-id="3c29c-176">**REST resources**</span></span> | <span data-ttu-id="3c29c-177">**另请参阅**</span><span class="sxs-lookup"><span data-stu-id="3c29c-177">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="3c29c-178">**组对象和方法**</span><span class="sxs-lookup"><span data-stu-id="3c29c-178">**Group object and methods**</span></span> | | |
| <span data-ttu-id="3c29c-179">创建新组、获取现有组、更新组的属性和删除组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-179">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="3c29c-180">目前，只有 Outlook 中的安全组和组才能通过 API 创建。</span><span class="sxs-lookup"><span data-stu-id="3c29c-180">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="3c29c-181">group</span><span class="sxs-lookup"><span data-stu-id="3c29c-181">group</span></span>](group.md) | [<span data-ttu-id="3c29c-182">新建组</span><span class="sxs-lookup"><span data-stu-id="3c29c-182">Create new groups</span></span>](../api/group-post-groups.md) <br/> [<span data-ttu-id="3c29c-183">列出组</span><span class="sxs-lookup"><span data-stu-id="3c29c-183">List groups</span></span>](../api/group-list.md) <br/> [<span data-ttu-id="3c29c-184">更新组</span><span class="sxs-lookup"><span data-stu-id="3c29c-184">Update groups</span></span>](../api/group-update.md) <br/> [<span data-ttu-id="3c29c-185">删除组</span><span class="sxs-lookup"><span data-stu-id="3c29c-185">Delete groups</span></span>](../api/group-delete.md) |
| <span data-ttu-id="3c29c-186">**组成员资格方法**</span><span class="sxs-lookup"><span data-stu-id="3c29c-186">**Group membership methods**</span></span> | | |
| <span data-ttu-id="3c29c-187">列出组中的成员，并添加或删除成员。</span><span class="sxs-lookup"><span data-stu-id="3c29c-187">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="3c29c-188">user</span><span class="sxs-lookup"><span data-stu-id="3c29c-188">user</span></span>](user.md) <br/> [<span data-ttu-id="3c29c-189">group</span><span class="sxs-lookup"><span data-stu-id="3c29c-189">group</span></span>](group.md)| [<span data-ttu-id="3c29c-190">列出成员</span><span class="sxs-lookup"><span data-stu-id="3c29c-190">List members</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="3c29c-191">添加成员</span><span class="sxs-lookup"><span data-stu-id="3c29c-191">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="3c29c-192">删除成员</span><span class="sxs-lookup"><span data-stu-id="3c29c-192">Remove member</span></span>](../api/group-delete-members.md)|
| <span data-ttu-id="3c29c-193">确定用户是否是组成员，并获取用户所属的全部组。</span><span class="sxs-lookup"><span data-stu-id="3c29c-193">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="3c29c-194">user</span><span class="sxs-lookup"><span data-stu-id="3c29c-194">user</span></span>](user.md) <br/> [<span data-ttu-id="3c29c-195">group</span><span class="sxs-lookup"><span data-stu-id="3c29c-195">group</span></span>](group.md)| [<span data-ttu-id="3c29c-196">检查成员组</span><span class="sxs-lookup"><span data-stu-id="3c29c-196">Check member groups</span></span>](../api/group-checkmembergroups.md) <br/> [<span data-ttu-id="3c29c-197">获取成员组</span><span class="sxs-lookup"><span data-stu-id="3c29c-197">Get member groups</span></span>](../api/group-getmembergroups.md)|
| <span data-ttu-id="3c29c-198">列出组的所有者，并添加或删除所有者。</span><span class="sxs-lookup"><span data-stu-id="3c29c-198">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="3c29c-199">user</span><span class="sxs-lookup"><span data-stu-id="3c29c-199">user</span></span>](user.md) <br/> [<span data-ttu-id="3c29c-200">group</span><span class="sxs-lookup"><span data-stu-id="3c29c-200">group</span></span>](group.md)| [<span data-ttu-id="3c29c-201">列出所有者</span><span class="sxs-lookup"><span data-stu-id="3c29c-201">List owners</span></span>](../api/group-list-members.md) <br/> [<span data-ttu-id="3c29c-202">添加成员</span><span class="sxs-lookup"><span data-stu-id="3c29c-202">Add member</span></span>](../api/group-post-members.md) <br/> [<span data-ttu-id="3c29c-203">删除成员</span><span class="sxs-lookup"><span data-stu-id="3c29c-203">Remove member</span></span>](../api/group-delete-members.md)|
