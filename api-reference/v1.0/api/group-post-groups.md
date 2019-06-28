---
title: 创建组
description: '创建请求正文中指定的新组。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ff8d4c28e4b2fed0858650d704dca34feb8eb79a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277782"
---
# <a name="create-group"></a><span data-ttu-id="74c8e-103">创建组</span><span class="sxs-lookup"><span data-stu-id="74c8e-103">Create group</span></span>
<span data-ttu-id="74c8e-104">创建请求正文中指定的新组。</span><span class="sxs-lookup"><span data-stu-id="74c8e-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="74c8e-105">你可以创建以下类型的组：</span><span class="sxs-lookup"><span data-stu-id="74c8e-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="74c8e-106">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="74c8e-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="74c8e-107">安全组</span><span class="sxs-lookup"><span data-stu-id="74c8e-107">Security group</span></span>

<span data-ttu-id="74c8e-108">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="74c8e-109">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="74c8e-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="74c8e-110">若要获取_非_默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="74c8e-p103">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="74c8e-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c8e-113">权限</span><span class="sxs-lookup"><span data-stu-id="74c8e-113">Permissions</span></span>
<span data-ttu-id="74c8e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74c8e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74c8e-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="74c8e-116">Permission type</span></span>      | <span data-ttu-id="74c8e-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74c8e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74c8e-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74c8e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="74c8e-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74c8e-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="74c8e-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74c8e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c8e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="74c8e-121">Not supported.</span></span>    |
|<span data-ttu-id="74c8e-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="74c8e-122">Application</span></span> | <span data-ttu-id="74c8e-123">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c8e-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74c8e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74c8e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="74c8e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="74c8e-125">Request headers</span></span>
| <span data-ttu-id="74c8e-126">名称</span><span class="sxs-lookup"><span data-stu-id="74c8e-126">Name</span></span>       | <span data-ttu-id="74c8e-127">类型</span><span class="sxs-lookup"><span data-stu-id="74c8e-127">Type</span></span> | <span data-ttu-id="74c8e-128">说明</span><span class="sxs-lookup"><span data-stu-id="74c8e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74c8e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="74c8e-129">Authorization</span></span>  | <span data-ttu-id="74c8e-130">string</span><span class="sxs-lookup"><span data-stu-id="74c8e-130">string</span></span>  | <span data-ttu-id="74c8e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74c8e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74c8e-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74c8e-133">Content-Type</span></span>  | <span data-ttu-id="74c8e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="74c8e-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74c8e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="74c8e-135">Request body</span></span>
<span data-ttu-id="74c8e-136">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="74c8e-137">属性</span><span class="sxs-lookup"><span data-stu-id="74c8e-137">Property</span></span> | <span data-ttu-id="74c8e-138">类型</span><span class="sxs-lookup"><span data-stu-id="74c8e-138">Type</span></span> | <span data-ttu-id="74c8e-139">说明</span><span class="sxs-lookup"><span data-stu-id="74c8e-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="74c8e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="74c8e-140">displayName</span></span> | <span data-ttu-id="74c8e-141">string</span><span class="sxs-lookup"><span data-stu-id="74c8e-141">string</span></span> | <span data-ttu-id="74c8e-142">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="74c8e-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="74c8e-143">必需。</span><span class="sxs-lookup"><span data-stu-id="74c8e-143">Required.</span></span> |
| <span data-ttu-id="74c8e-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="74c8e-144">mailEnabled</span></span> | <span data-ttu-id="74c8e-145">布尔</span><span class="sxs-lookup"><span data-stu-id="74c8e-145">boolean</span></span> | <span data-ttu-id="74c8e-146">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="74c8e-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="74c8e-147">必需。</span><span class="sxs-lookup"><span data-stu-id="74c8e-147">Required.</span></span> |
| <span data-ttu-id="74c8e-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="74c8e-148">mailNickname</span></span> | <span data-ttu-id="74c8e-149">string</span><span class="sxs-lookup"><span data-stu-id="74c8e-149">string</span></span> | <span data-ttu-id="74c8e-150">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="74c8e-150">The mail alias for the group.</span></span> <span data-ttu-id="74c8e-151">必需。</span><span class="sxs-lookup"><span data-stu-id="74c8e-151">Required.</span></span> |
| <span data-ttu-id="74c8e-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="74c8e-152">securityEnabled</span></span> | <span data-ttu-id="74c8e-153">boolean</span><span class="sxs-lookup"><span data-stu-id="74c8e-153">boolean</span></span> | <span data-ttu-id="74c8e-154">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="74c8e-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="74c8e-155">必需。</span><span class="sxs-lookup"><span data-stu-id="74c8e-155">Required.</span></span> |
| <span data-ttu-id="74c8e-156">owners</span><span class="sxs-lookup"><span data-stu-id="74c8e-156">owners</span></span> | <span data-ttu-id="74c8e-157">string collection</span><span class="sxs-lookup"><span data-stu-id="74c8e-157">string collection</span></span> | <span data-ttu-id="74c8e-158">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="74c8e-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="74c8e-159">可选。</span><span class="sxs-lookup"><span data-stu-id="74c8e-159">Optional.</span></span> |
| <span data-ttu-id="74c8e-160">members</span><span class="sxs-lookup"><span data-stu-id="74c8e-160">members</span></span> | <span data-ttu-id="74c8e-161">字符串集合</span><span class="sxs-lookup"><span data-stu-id="74c8e-161">string collection</span></span> | <span data-ttu-id="74c8e-162">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="74c8e-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="74c8e-163">可选。</span><span class="sxs-lookup"><span data-stu-id="74c8e-163">Optional.</span></span> |

> <span data-ttu-id="74c8e-164">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="74c8e-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="74c8e-165">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="74c8e-166">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="74c8e-167">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="74c8e-167">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="74c8e-168">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="74c8e-168">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="74c8e-169">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="74c8e-169">groupTypes options</span></span>

<span data-ttu-id="74c8e-170">使用 **groupTypes** 属性来控制组的类型及其成员身份，如下所示：</span><span class="sxs-lookup"><span data-stu-id="74c8e-170">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="74c8e-171">组类型</span><span class="sxs-lookup"><span data-stu-id="74c8e-171">Type of group</span></span> | <span data-ttu-id="74c8e-172">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="74c8e-172">Assigned membership</span></span> | <span data-ttu-id="74c8e-173">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="74c8e-173">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="74c8e-174">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="74c8e-174">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="74c8e-175">动态</span><span class="sxs-lookup"><span data-stu-id="74c8e-175">Dynamic</span></span> | <span data-ttu-id="74c8e-176">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="74c8e-176">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="74c8e-177">响应</span><span class="sxs-lookup"><span data-stu-id="74c8e-177">Response</span></span>
<span data-ttu-id="74c8e-178">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74c8e-178">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="74c8e-179">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-179">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="74c8e-180">示例</span><span class="sxs-lookup"><span data-stu-id="74c8e-180">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="74c8e-181">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="74c8e-181">Create an Office 365 group</span></span>

<span data-ttu-id="74c8e-182">以下示例将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="74c8e-182">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="74c8e-183">请求</span><span class="sxs-lookup"><span data-stu-id="74c8e-183">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="74c8e-184">响应</span><span class="sxs-lookup"><span data-stu-id="74c8e-184">Response</span></span>

<span data-ttu-id="74c8e-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74c8e-185">The following is an example of the response.</span></span>

><span data-ttu-id="74c8e-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="74c8e-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74c8e-187">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-187">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74c8e-188">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="74c8e-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74c8e-189">C#</span><span class="sxs-lookup"><span data-stu-id="74c8e-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74c8e-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="74c8e-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74c8e-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c8e-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="74c8e-192">示例 2：创建包含所有者和成员的组</span><span class="sxs-lookup"><span data-stu-id="74c8e-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="74c8e-193">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="74c8e-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="74c8e-194">请求</span><span class="sxs-lookup"><span data-stu-id="74c8e-194">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="74c8e-195">响应</span><span class="sxs-lookup"><span data-stu-id="74c8e-195">Response</span></span>

<span data-ttu-id="74c8e-196">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="74c8e-196">The following is an example of a successful response.</span></span> <span data-ttu-id="74c8e-197">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-197">It includes only default properties.</span></span> <span data-ttu-id="74c8e-198">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="74c8e-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="74c8e-199">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="74c8e-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="74c8e-200">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="74c8e-200">All the default properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74c8e-201">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="74c8e-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74c8e-202">C#</span><span class="sxs-lookup"><span data-stu-id="74c8e-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74c8e-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="74c8e-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74c8e-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c8e-204">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
