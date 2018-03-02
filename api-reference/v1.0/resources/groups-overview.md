# <a name="working-with-groups-in-microsoft-graph"></a><span data-ttu-id="c805e-101">在 Microsoft Graph 中使用组</span><span class="sxs-lookup"><span data-stu-id="c805e-101">Working with groups in Microsoft Graph</span></span>

<span data-ttu-id="c805e-102">组是[用户](user.md)和其他主体的集合，他们共享对 Microsoft 服务或应用中资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c805e-102">Groups are collections of [users](user.md) and other principals who share access to resources in Microsoft services or in your app.</span></span> <span data-ttu-id="c805e-103">Microsoft Graph 提供了可用于根据方案创建和管理不同类型组和组功能的 API。</span><span class="sxs-lookup"><span data-stu-id="c805e-103">Microsoft Graph provides APIs that you can use to create and manage different types of groups and group functionality according to your scenario.</span></span> <span data-ttu-id="c805e-104">Microsoft Graph 中所有与组相关的操作都需要征得管理员同意。</span><span class="sxs-lookup"><span data-stu-id="c805e-104">All group-related operations in Microsoft Graph require administrator consent.</span></span>

> <span data-ttu-id="c805e-105">**注意**：只能通过工作或学校帐户创建组。</span><span class="sxs-lookup"><span data-stu-id="c805e-105">**Note**: Groups can only be created through work or school accounts.</span></span> <span data-ttu-id="c805e-106">个人 Microsoft 帐户不支持组。</span><span class="sxs-lookup"><span data-stu-id="c805e-106">Personal Microsoft accounts don't support groups.</span></span>

| <span data-ttu-id="c805e-107">类型</span><span class="sxs-lookup"><span data-stu-id="c805e-107">Type</span></span>              | <span data-ttu-id="c805e-108">用例</span><span class="sxs-lookup"><span data-stu-id="c805e-108">Use case</span></span> | <span data-ttu-id="c805e-109">groupType</span><span class="sxs-lookup"><span data-stu-id="c805e-109">groupType</span></span> | <span data-ttu-id="c805e-110">启用邮件</span><span class="sxs-lookup"><span data-stu-id="c805e-110">mail-enabled</span></span> | <span data-ttu-id="c805e-111">启用安全机制</span><span class="sxs-lookup"><span data-stu-id="c805e-111">security-enabled</span></span> | <span data-ttu-id="c805e-112">是否可通过 API 创建？</span><span class="sxs-lookup"><span data-stu-id="c805e-112">Can be created via API?</span></span> |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [<span data-ttu-id="c805e-113">Office 365 组</span><span class="sxs-lookup"><span data-stu-id="c805e-113">Office 365 groups</span></span>](#office-365-groups) | <span data-ttu-id="c805e-114">促进用户与共享 Microsoft Online 资源的协作。</span><span class="sxs-lookup"><span data-stu-id="c805e-114">Facilitating user collaboration with shared Microsoft online resources.</span></span> | `["Unified"]` | `true` | `false` | <span data-ttu-id="c805e-115">可访问</span><span class="sxs-lookup"><span data-stu-id="c805e-115">Yes</span></span> |
| [<span data-ttu-id="c805e-116">安全组</span><span class="sxs-lookup"><span data-stu-id="c805e-116">Security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="c805e-117">控制用户对应用中资源的访问。</span><span class="sxs-lookup"><span data-stu-id="c805e-117">Controlling user access to in-app resources.</span></span> | `[]` | `false` | `true` | <span data-ttu-id="c805e-118">是</span><span class="sxs-lookup"><span data-stu-id="c805e-118">Yes</span></span> |
| [<span data-ttu-id="c805e-119">启用邮件的安全组</span><span class="sxs-lookup"><span data-stu-id="c805e-119">Mail-enabled security groups</span></span>](#security-groups-and-mail-enabled-security-groups) | <span data-ttu-id="c805e-120">使用共享的组邮箱，控制用户对应用中资源的访问。</span><span class="sxs-lookup"><span data-stu-id="c805e-120">Controlling user access to in-app resources, with a shared group mailbox.</span></span> | `[]` | `true` | `true` | <span data-ttu-id="c805e-121">否</span><span class="sxs-lookup"><span data-stu-id="c805e-121">No</span></span> |
| <span data-ttu-id="c805e-122">通讯组</span><span class="sxs-lookup"><span data-stu-id="c805e-122">Distribution groups</span></span> | <span data-ttu-id="c805e-123">将邮件分发给组中的成员。</span><span class="sxs-lookup"><span data-stu-id="c805e-123">Distributing mail to the members of the group.</span></span> <span data-ttu-id="c805e-124">建议使用 Office 365 组，因为它提供的资源集更丰富。</span><span class="sxs-lookup"><span data-stu-id="c805e-124">It is recommended to use Office 365 groups due to the richer set of resources it provides.</span></span> | `[]` | `true` | `false` | <span data-ttu-id="c805e-125">否</span><span class="sxs-lookup"><span data-stu-id="c805e-125">No</span></span> |

## <a name="office-365-groups"></a><span data-ttu-id="c805e-126">Office 365 组</span><span class="sxs-lookup"><span data-stu-id="c805e-126">Office 365 groups</span></span>
<span data-ttu-id="c805e-127">Office 365 组的强大之处在于它的协作本质，它是项目或团队中相互协作的用户的理想之选。</span><span class="sxs-lookup"><span data-stu-id="c805e-127">The power of Office 365 groups is in its collaborative nature, perfect for people who work together on a project or a team.</span></span> <span data-ttu-id="c805e-128">创建时，它们包含组成员共享的资源，包括：</span><span class="sxs-lookup"><span data-stu-id="c805e-128">They are created with resources that members of the group share, including:</span></span>

- <span data-ttu-id="c805e-129">Outlook 对话</span><span class="sxs-lookup"><span data-stu-id="c805e-129">Outlook conversations</span></span>
- <span data-ttu-id="c805e-130">Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="c805e-130">Outlook calendar</span></span>
- <span data-ttu-id="c805e-131">SharePoint 文件</span><span class="sxs-lookup"><span data-stu-id="c805e-131">SharePoint files</span></span>
- <span data-ttu-id="c805e-132">OneNote 笔记本</span><span class="sxs-lookup"><span data-stu-id="c805e-132">OneNote notebook</span></span>
- <span data-ttu-id="c805e-133">SharePoint 团队网站</span><span class="sxs-lookup"><span data-stu-id="c805e-133">SharePoint team site</span></span>
- <span data-ttu-id="c805e-134">Planner 计划</span><span class="sxs-lookup"><span data-stu-id="c805e-134">Planner plans</span></span>
- <span data-ttu-id="c805e-135">Intune 设备管理</span><span class="sxs-lookup"><span data-stu-id="c805e-135">Intune device management</span></span>

### <a name="group-in-outlook-example"></a><span data-ttu-id="c805e-136">Outlook 中的组示例</span><span class="sxs-lookup"><span data-stu-id="c805e-136">Group in Outlook example</span></span>

<span data-ttu-id="c805e-137">下面是 Outlook 中组的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c805e-137">The following is a JSON representation of groups in Outlook.</span></span> 

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
<span data-ttu-id="c805e-138">若要详细了解 Office 365 组和管理员体验，请参阅[了解 Office 365 组](https://support.office.com/zh-CN/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2)。</span><span class="sxs-lookup"><span data-stu-id="c805e-138">To learn more about Office 365 groups and the administrator experiences, see [Learn about Office 365 Groups](https://support.office.com/zh-CN/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).</span></span>

## <a name="security-groups-and-mail-enabled-security-groups"></a><span data-ttu-id="c805e-139">安全组和启用邮件的安全组</span><span class="sxs-lookup"><span data-stu-id="c805e-139">Security groups and mail-enabled security groups</span></span>

<span data-ttu-id="c805e-140">安全组用于控制用户对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="c805e-140">Security groups are for controlling user access to resources.</span></span> <span data-ttu-id="c805e-141">通过检查用户是否是安全组的成员，应用可以在用户尝试访问应用中的某些安全资源时决定是否授权。</span><span class="sxs-lookup"><span data-stu-id="c805e-141">By checking whether a user is a member of a security group, your app can make authorization decisions when that user is trying to access some secure resources in your app.</span></span> <span data-ttu-id="c805e-142">安全组的成员可以是用户和其他安全组。</span><span class="sxs-lookup"><span data-stu-id="c805e-142">Security groups can have users and other security groups as members.</span></span>

<span data-ttu-id="c805e-143">启用邮件的安全组的使用方式与安全组基本相同，不同之处在于添加了组的共享邮箱功能。</span><span class="sxs-lookup"><span data-stu-id="c805e-143">Mail-enabled security groups are used in the same way that security groups are, but with the added feature of a shared mailbox for the groups.</span></span> <span data-ttu-id="c805e-144">无法通过 API 创建启用邮件的安全组，但其他组操作仍适用。</span><span class="sxs-lookup"><span data-stu-id="c805e-144">Mail-enabled security groups can't be created through the API, but other group operations will still work here.</span></span>  <span data-ttu-id="c805e-145">启用邮件的安全组为只读。</span><span class="sxs-lookup"><span data-stu-id="c805e-145">Mail-enabled security groups are read only.</span></span> <span data-ttu-id="c805e-146">若要了解更多信息，请参阅 Exchange 文章[管理启用邮件的安全组](https://technet.microsoft.com/zh-CN/library/bb123521%28v=exchg.160%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c805e-146">Learn more in the [Manage mail-enabled security groups Exchange article](https://technet.microsoft.com/zh-CN/library/bb123521%28v=exchg.160%29.aspx).</span></span>

### <a name="security-group-example"></a><span data-ttu-id="c805e-147">安全组示例</span><span class="sxs-lookup"><span data-stu-id="c805e-147">Security group example</span></span>

<span data-ttu-id="c805e-148">下面是安全组的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c805e-148">The following is a JSON representation of a security group.</span></span> 

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
## <a name="dynamic-membership"></a><span data-ttu-id="c805e-149">动态成员资格</span><span class="sxs-lookup"><span data-stu-id="c805e-149">Dynamic membership</span></span> 

<span data-ttu-id="c805e-150">所有类型的组都可以有成员资格规则，用于根据用户属性自动在组中添加或删除成员。</span><span class="sxs-lookup"><span data-stu-id="c805e-150">All types of groups can have dynamic membership rules that automatically add or remove members from the group based on user properties.</span></span> <span data-ttu-id="c805e-151">例如，“市场营销部员工”组包含所有 department 属性设置为“Marketing”的用户，这样可以将新入职的市场营销部员工自动添加到组中，并自动在组中删除从市场营销部离职的员工。</span><span class="sxs-lookup"><span data-stu-id="c805e-151">For example, a "Marketing employees" group would include every user with the department property set to "Marketing", so that new marketing employees are automatically added to the group and employees who leave the department are automatically removed from the group.</span></span> <span data-ttu-id="c805e-152">在组创建期间，可以在“membershipRule”字段中将此规则指定为 `"membershipRule": 'user.department -eq "Marketing"'`。</span><span class="sxs-lookup"><span data-stu-id="c805e-152">This rule can be specified in a "membershipRule" field during group creation as `"membershipRule": 'user.department -eq "Marketing"'`.</span></span> <span data-ttu-id="c805e-153">GroupType 还必须包括 `"DynamicMembership"`。</span><span class="sxs-lookup"><span data-stu-id="c805e-153">GroupType must also include `"DynamicMembership"`.</span></span> <span data-ttu-id="c805e-154">下面的请求为市场营销部员工新建 Office 365 组：</span><span class="sxs-lookup"><span data-stu-id="c805e-154">The following request creates a new Office 365 group for the marketing employees:</span></span> 

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

<span data-ttu-id="c805e-155">若要详细了解如何表述 membershipRules，请参阅[在 Azure Active Directory 中创建基于属性的动态组成员资格规则](https://docs.microsoft.com/zh-CN/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="c805e-155">To learn more about formulating membershipRules, see [Create attribute-based rules for dynamic group membership in Azure Active Directory](https://docs.microsoft.com/zh-CN/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).</span></span>

> <span data-ttu-id="c805e-156">**注意**：动态成员资格规则要求租户必须在 [Azure Active Directory Premium P1](https://azure.microsoft.com/zh-CN/pricing/details/active-directory/) 或更高层拥有许可证。</span><span class="sxs-lookup"><span data-stu-id="c805e-156">**Note**: Dynamic membership rules requires the tenant to have a license at tier [Azure Active Directory Premium P1](https://azure.microsoft.com/zh-CN/pricing/details/active-directory/) or greater.</span></span>

## <a name="other-types-of-groups"></a><span data-ttu-id="c805e-157">其他类型的组</span><span class="sxs-lookup"><span data-stu-id="c805e-157">Other types of groups</span></span>

<span data-ttu-id="c805e-158">Yammer 中的 office 365 组用于通过 Yammer 帖子促进用户协作。</span><span class="sxs-lookup"><span data-stu-id="c805e-158">Office 365 groups in Yammer are used to facilitate user collaboration through Yammer posts.</span></span> <span data-ttu-id="c805e-159">可以通过读取请求返回这种类型的组，但无法通过 API 访问它们的帖子。</span><span class="sxs-lookup"><span data-stu-id="c805e-159">This type of group can be returned through a read request, but their posts can't be accessed through the API.</span></span> <span data-ttu-id="c805e-160">如果对组启用了 Yammer 帖子和对话源，将会禁用默认的 Office 365 组对话。</span><span class="sxs-lookup"><span data-stu-id="c805e-160">When Yammer posts and conversation feeds are enabled on a group, default Office 365 group conversations are disabled.</span></span> <span data-ttu-id="c805e-161">若要了解详细信息，请参阅 [Yammer 开发人员 API 文档](https://developer.yammer.com/docs)。</span><span class="sxs-lookup"><span data-stu-id="c805e-161">To learn more, see [Yammer developer API docs](https://developer.yammer.com/docs).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="c805e-162">常见用例</span><span class="sxs-lookup"><span data-stu-id="c805e-162">Common use cases</span></span>

<span data-ttu-id="c805e-163">使用 Microsoft Graph，可以执行下面的常见操作。</span><span class="sxs-lookup"><span data-stu-id="c805e-163">Using Microsoft Graph, you can perform the following common operations.</span></span>

| <span data-ttu-id="c805e-164">**用例**</span><span class="sxs-lookup"><span data-stu-id="c805e-164">**Use cases**</span></span>  | <span data-ttu-id="c805e-165">**REST 资源**</span><span class="sxs-lookup"><span data-stu-id="c805e-165">**REST resources**</span></span> | <span data-ttu-id="c805e-166">**另请参阅**</span><span class="sxs-lookup"><span data-stu-id="c805e-166">**See also**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c805e-167">**组对象和方法**</span><span class="sxs-lookup"><span data-stu-id="c805e-167">**Group object and methods**</span></span> | | |
| <span data-ttu-id="c805e-168">创建新组、获取现有组、更新组的属性和删除组。</span><span class="sxs-lookup"><span data-stu-id="c805e-168">Create new groups, get existing groups, update the properties on groups, and delete groups.</span></span> <span data-ttu-id="c805e-169">目前，只有 Outlook 中的安全组和组才能通过 API 创建。</span><span class="sxs-lookup"><span data-stu-id="c805e-169">Currently, only security groups and groups in Outlook can be created through the API.</span></span> | [<span data-ttu-id="c805e-170">group</span><span class="sxs-lookup"><span data-stu-id="c805e-170">group</span></span>](group.md) | [<span data-ttu-id="c805e-171">新建组</span><span class="sxs-lookup"><span data-stu-id="c805e-171">Create new groups</span></span>](../api/group_post_groups.md) <br/> [<span data-ttu-id="c805e-172">列出组</span><span class="sxs-lookup"><span data-stu-id="c805e-172">List groups</span></span>](../api/group_list.md) <br/> [<span data-ttu-id="c805e-173">更新组</span><span class="sxs-lookup"><span data-stu-id="c805e-173">Update groups</span></span>](../api/group_update.md) <br/> [<span data-ttu-id="c805e-174">删除组</span><span class="sxs-lookup"><span data-stu-id="c805e-174">Delete groups</span></span>](../api/group_delete.md) |
| <span data-ttu-id="c805e-175">**组成员资格方法**</span><span class="sxs-lookup"><span data-stu-id="c805e-175">**Group membership methods**</span></span> | | |
| <span data-ttu-id="c805e-176">列出组中的成员，并添加或删除成员。</span><span class="sxs-lookup"><span data-stu-id="c805e-176">List the members of a group, and add or remove members.</span></span> | [<span data-ttu-id="c805e-177">user</span><span class="sxs-lookup"><span data-stu-id="c805e-177">user</span></span>](user.md) <br/> [<span data-ttu-id="c805e-178">group</span><span class="sxs-lookup"><span data-stu-id="c805e-178">group</span></span>](group.md)| [<span data-ttu-id="c805e-179">列出成员</span><span class="sxs-lookup"><span data-stu-id="c805e-179">List members</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="c805e-180">添加成员</span><span class="sxs-lookup"><span data-stu-id="c805e-180">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="c805e-181">删除成员</span><span class="sxs-lookup"><span data-stu-id="c805e-181">Remove member</span></span>](../api/group_delete_members.md)|
| <span data-ttu-id="c805e-182">确定用户是否是组成员，并获取用户所属的全部组。</span><span class="sxs-lookup"><span data-stu-id="c805e-182">Determine whether a user is a member of a group, get all the groups the user is a member of.</span></span> | [<span data-ttu-id="c805e-183">user</span><span class="sxs-lookup"><span data-stu-id="c805e-183">user</span></span>](user.md) <br/> [<span data-ttu-id="c805e-184">group</span><span class="sxs-lookup"><span data-stu-id="c805e-184">group</span></span>](group.md)| [<span data-ttu-id="c805e-185">检查成员组</span><span class="sxs-lookup"><span data-stu-id="c805e-185">Check member groups</span></span>](../api/group_checkmembergroups.md) <br/> [<span data-ttu-id="c805e-186">获取成员组</span><span class="sxs-lookup"><span data-stu-id="c805e-186">Get member groups</span></span>](../api/group_getmembergroups.md)|
| <span data-ttu-id="c805e-187">列出组的所有者，并添加或删除所有者。</span><span class="sxs-lookup"><span data-stu-id="c805e-187">List the owners of a group, and add or remove owners.</span></span> | [<span data-ttu-id="c805e-188">user</span><span class="sxs-lookup"><span data-stu-id="c805e-188">user</span></span>](user.md) <br/> [<span data-ttu-id="c805e-189">group</span><span class="sxs-lookup"><span data-stu-id="c805e-189">group</span></span>](group.md)| [<span data-ttu-id="c805e-190">列出所有者</span><span class="sxs-lookup"><span data-stu-id="c805e-190">List owners</span></span>](../api/group_list_members.md) <br/> [<span data-ttu-id="c805e-191">添加成员</span><span class="sxs-lookup"><span data-stu-id="c805e-191">Add member</span></span>](../api/group_post_members.md) <br/> [<span data-ttu-id="c805e-192">删除成员</span><span class="sxs-lookup"><span data-stu-id="c805e-192">Remove member</span></span>](../api/group_delete_members.md)|
