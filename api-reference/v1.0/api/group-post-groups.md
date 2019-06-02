---
title: 创建组
description: '创建请求正文中指定的新组。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 0a525ffffe62685e863572c0e81c808b2c6e8a02
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537119"
---
# <a name="create-group"></a><span data-ttu-id="4690b-103">创建组</span><span class="sxs-lookup"><span data-stu-id="4690b-103">Create group</span></span>
<span data-ttu-id="4690b-104">创建请求正文中指定的新组。</span><span class="sxs-lookup"><span data-stu-id="4690b-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="4690b-105">你可以创建以下类型的组：</span><span class="sxs-lookup"><span data-stu-id="4690b-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="4690b-106">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="4690b-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="4690b-107">安全组</span><span class="sxs-lookup"><span data-stu-id="4690b-107">Security group</span></span>

<span data-ttu-id="4690b-108">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="4690b-109">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="4690b-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="4690b-110">若要获取_非_默认返回的属性，请执行 GET 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="4690b-111">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="4690b-111">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="4690b-p104">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="4690b-p104">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="4690b-114">权限</span><span class="sxs-lookup"><span data-stu-id="4690b-114">Permissions</span></span>
<span data-ttu-id="4690b-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4690b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4690b-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="4690b-117">Permission type</span></span>      | <span data-ttu-id="4690b-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4690b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4690b-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4690b-119">Delegated (work or school account)</span></span> | <span data-ttu-id="4690b-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4690b-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4690b-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4690b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4690b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="4690b-122">Not supported.</span></span>    |
|<span data-ttu-id="4690b-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="4690b-123">Application</span></span> | <span data-ttu-id="4690b-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4690b-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4690b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4690b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="4690b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4690b-126">Request headers</span></span>
| <span data-ttu-id="4690b-127">名称</span><span class="sxs-lookup"><span data-stu-id="4690b-127">Name</span></span>       | <span data-ttu-id="4690b-128">类型</span><span class="sxs-lookup"><span data-stu-id="4690b-128">Type</span></span> | <span data-ttu-id="4690b-129">说明</span><span class="sxs-lookup"><span data-stu-id="4690b-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4690b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4690b-130">Authorization</span></span>  | <span data-ttu-id="4690b-131">string</span><span class="sxs-lookup"><span data-stu-id="4690b-131">string</span></span>  | <span data-ttu-id="4690b-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4690b-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4690b-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4690b-134">Content-Type</span></span>  | <span data-ttu-id="4690b-135">application/json</span><span class="sxs-lookup"><span data-stu-id="4690b-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4690b-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="4690b-136">Request body</span></span>
<span data-ttu-id="4690b-137">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="4690b-138">属性</span><span class="sxs-lookup"><span data-stu-id="4690b-138">Property</span></span> | <span data-ttu-id="4690b-139">类型</span><span class="sxs-lookup"><span data-stu-id="4690b-139">Type</span></span> | <span data-ttu-id="4690b-140">说明</span><span class="sxs-lookup"><span data-stu-id="4690b-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4690b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4690b-141">displayName</span></span> | <span data-ttu-id="4690b-142">string</span><span class="sxs-lookup"><span data-stu-id="4690b-142">string</span></span> | <span data-ttu-id="4690b-143">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="4690b-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="4690b-144">必需。</span><span class="sxs-lookup"><span data-stu-id="4690b-144">Required.</span></span> |
| <span data-ttu-id="4690b-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4690b-145">mailEnabled</span></span> | <span data-ttu-id="4690b-146">布尔</span><span class="sxs-lookup"><span data-stu-id="4690b-146">boolean</span></span> | <span data-ttu-id="4690b-147">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="4690b-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="4690b-148">必需。</span><span class="sxs-lookup"><span data-stu-id="4690b-148">Required.</span></span> |
| <span data-ttu-id="4690b-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4690b-149">mailNickname</span></span> | <span data-ttu-id="4690b-150">string</span><span class="sxs-lookup"><span data-stu-id="4690b-150">string</span></span> | <span data-ttu-id="4690b-151">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="4690b-151">The mail alias for the group.</span></span> <span data-ttu-id="4690b-152">必需。</span><span class="sxs-lookup"><span data-stu-id="4690b-152">Required.</span></span> |
| <span data-ttu-id="4690b-153">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4690b-153">securityEnabled</span></span> | <span data-ttu-id="4690b-154">boolean</span><span class="sxs-lookup"><span data-stu-id="4690b-154">boolean</span></span> | <span data-ttu-id="4690b-155">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="4690b-155">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="4690b-156">必需。</span><span class="sxs-lookup"><span data-stu-id="4690b-156">Required.</span></span> |
| <span data-ttu-id="4690b-157">owners</span><span class="sxs-lookup"><span data-stu-id="4690b-157">owners</span></span> | <span data-ttu-id="4690b-158">string collection</span><span class="sxs-lookup"><span data-stu-id="4690b-158">string collection</span></span> | <span data-ttu-id="4690b-159">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="4690b-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="4690b-160">可选。</span><span class="sxs-lookup"><span data-stu-id="4690b-160">Optional.</span></span> |
| <span data-ttu-id="4690b-161">members</span><span class="sxs-lookup"><span data-stu-id="4690b-161">members</span></span> | <span data-ttu-id="4690b-162">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4690b-162">string collection</span></span> | <span data-ttu-id="4690b-163">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="4690b-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="4690b-164">可选。</span><span class="sxs-lookup"><span data-stu-id="4690b-164">Optional.</span></span> |

> <span data-ttu-id="4690b-165">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="4690b-165">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="4690b-166">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-166">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="4690b-167">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-167">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="4690b-168">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="4690b-168">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="4690b-169">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="4690b-169">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="4690b-170">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="4690b-170">groupTypes options</span></span>

<span data-ttu-id="4690b-171">使用 **groupTypes** 属性来控制组的类型及其成员身份，如下所示：</span><span class="sxs-lookup"><span data-stu-id="4690b-171">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="4690b-172">组类型</span><span class="sxs-lookup"><span data-stu-id="4690b-172">Type of group</span></span> | <span data-ttu-id="4690b-173">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="4690b-173">Assigned membership</span></span> | <span data-ttu-id="4690b-174">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="4690b-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="4690b-175">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="4690b-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="4690b-176">动态</span><span class="sxs-lookup"><span data-stu-id="4690b-176">Dynamic</span></span> | <span data-ttu-id="4690b-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="4690b-177">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="4690b-178">响应</span><span class="sxs-lookup"><span data-stu-id="4690b-178">Response</span></span>
<span data-ttu-id="4690b-179">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4690b-179">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="4690b-180">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="4690b-181">示例</span><span class="sxs-lookup"><span data-stu-id="4690b-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="4690b-182">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="4690b-182">Create an Office 365 group</span></span>

<span data-ttu-id="4690b-183">以下示例将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="4690b-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="4690b-184">请求</span><span class="sxs-lookup"><span data-stu-id="4690b-184">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4690b-185">响应</span><span class="sxs-lookup"><span data-stu-id="4690b-185">Response</span></span>

<span data-ttu-id="4690b-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4690b-186">The following is an example of the response.</span></span>

><span data-ttu-id="4690b-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4690b-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4690b-188">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-188">All the default properties are returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4690b-189">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4690b-189">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4690b-190">C#</span><span class="sxs-lookup"><span data-stu-id="4690b-190">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4690b-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="4690b-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="4690b-192">示例 2：创建包含所有者和成员的组</span><span class="sxs-lookup"><span data-stu-id="4690b-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="4690b-193">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="4690b-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="4690b-194">请求</span><span class="sxs-lookup"><span data-stu-id="4690b-194">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4690b-195">响应</span><span class="sxs-lookup"><span data-stu-id="4690b-195">Response</span></span>

<span data-ttu-id="4690b-196">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="4690b-196">The following is an example of a successful response.</span></span> <span data-ttu-id="4690b-197">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-197">It includes only default properties.</span></span> <span data-ttu-id="4690b-198">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="4690b-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="4690b-199">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4690b-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4690b-200">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="4690b-200">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4690b-201">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4690b-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4690b-202">C#</span><span class="sxs-lookup"><span data-stu-id="4690b-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4690b-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="4690b-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
