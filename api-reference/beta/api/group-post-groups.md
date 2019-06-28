---
title: 创建组
description: 创建新的 Office 365 组或安全组。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 918e1b40ff45b92b44d3e18970f232cd318a2865
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262942"
---
# <a name="create-group"></a><span data-ttu-id="ed5b3-103">创建组</span><span class="sxs-lookup"><span data-stu-id="ed5b3-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed5b3-104">创建请求正文中指定的新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="ed5b3-105">你可以创建以下组之一：</span><span class="sxs-lookup"><span data-stu-id="ed5b3-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="ed5b3-106">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="ed5b3-107">安全组</span><span class="sxs-lookup"><span data-stu-id="ed5b3-107">Security group</span></span>

<span data-ttu-id="ed5b3-108">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="ed5b3-109">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="ed5b3-110">若要获取_非_默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="ed5b3-111">**注意**：若要创建[团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed5b3-112">权限</span><span class="sxs-lookup"><span data-stu-id="ed5b3-112">Permissions</span></span>
<span data-ttu-id="ed5b3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5b3-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed5b3-115">Permission type</span></span>      | <span data-ttu-id="ed5b3-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed5b3-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ed5b3-118">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed5b3-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="ed5b3-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed5b3-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-120">Not supported.</span></span>    |
|<span data-ttu-id="ed5b3-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed5b3-121">Application</span></span> | <span data-ttu-id="ed5b3-122">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed5b3-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed5b3-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed5b3-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="ed5b3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed5b3-124">Request headers</span></span>

| <span data-ttu-id="ed5b3-125">名称</span><span class="sxs-lookup"><span data-stu-id="ed5b3-125">Name</span></span>       | <span data-ttu-id="ed5b3-126">类型</span><span class="sxs-lookup"><span data-stu-id="ed5b3-126">Type</span></span> | <span data-ttu-id="ed5b3-127">说明</span><span class="sxs-lookup"><span data-stu-id="ed5b3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed5b3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed5b3-128">Authorization</span></span>  | <span data-ttu-id="ed5b3-129">string</span><span class="sxs-lookup"><span data-stu-id="ed5b3-129">string</span></span>  | <span data-ttu-id="ed5b3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed5b3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed5b3-132">Request body</span></span>

<span data-ttu-id="ed5b3-133">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="ed5b3-134">属性</span><span class="sxs-lookup"><span data-stu-id="ed5b3-134">Property</span></span> | <span data-ttu-id="ed5b3-135">类型</span><span class="sxs-lookup"><span data-stu-id="ed5b3-135">Type</span></span> | <span data-ttu-id="ed5b3-136">说明</span><span class="sxs-lookup"><span data-stu-id="ed5b3-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed5b3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ed5b3-137">displayName</span></span> | <span data-ttu-id="ed5b3-138">string</span><span class="sxs-lookup"><span data-stu-id="ed5b3-138">string</span></span> | <span data-ttu-id="ed5b3-139">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="ed5b3-140">必需。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-140">Required.</span></span> |
| <span data-ttu-id="ed5b3-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ed5b3-141">mailEnabled</span></span> | <span data-ttu-id="ed5b3-142">布尔</span><span class="sxs-lookup"><span data-stu-id="ed5b3-142">boolean</span></span> | <span data-ttu-id="ed5b3-143">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="ed5b3-144">必需。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-144">Required.</span></span> |
| <span data-ttu-id="ed5b3-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ed5b3-145">mailNickname</span></span> | <span data-ttu-id="ed5b3-146">string</span><span class="sxs-lookup"><span data-stu-id="ed5b3-146">string</span></span> | <span data-ttu-id="ed5b3-147">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-147">The mail alias for the group.</span></span> <span data-ttu-id="ed5b3-148">必需。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-148">Required.</span></span> |
| <span data-ttu-id="ed5b3-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ed5b3-149">securityEnabled</span></span> | <span data-ttu-id="ed5b3-150">boolean</span><span class="sxs-lookup"><span data-stu-id="ed5b3-150">boolean</span></span> | <span data-ttu-id="ed5b3-151">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="ed5b3-152">必需。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-152">Required.</span></span> |
| <span data-ttu-id="ed5b3-153">owners</span><span class="sxs-lookup"><span data-stu-id="ed5b3-153">owners</span></span> | <span data-ttu-id="ed5b3-154">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="ed5b3-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="ed5b3-155">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="ed5b3-156">可选。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-156">Optional.</span></span> |
| <span data-ttu-id="ed5b3-157">members</span><span class="sxs-lookup"><span data-stu-id="ed5b3-157">members</span></span> | <span data-ttu-id="ed5b3-158">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="ed5b3-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="ed5b3-159">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="ed5b3-160">可选。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-160">Optional.</span></span> |

> <span data-ttu-id="ed5b3-161">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="ed5b3-162">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="ed5b3-163">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="ed5b3-164">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="ed5b3-p112">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="ed5b3-167">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="ed5b3-167">groupTypes options</span></span>

<span data-ttu-id="ed5b3-168">使用 **groupTypes** 属性来控制组的类型及其成员身份，如下所示：</span><span class="sxs-lookup"><span data-stu-id="ed5b3-168">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="ed5b3-169">组类型</span><span class="sxs-lookup"><span data-stu-id="ed5b3-169">Type of group</span></span> | <span data-ttu-id="ed5b3-170">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="ed5b3-170">Assigned membership</span></span> | <span data-ttu-id="ed5b3-171">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="ed5b3-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="ed5b3-172">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="ed5b3-173">动态</span><span class="sxs-lookup"><span data-stu-id="ed5b3-173">Dynamic</span></span> | <span data-ttu-id="ed5b3-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="ed5b3-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="ed5b3-175">响应</span><span class="sxs-lookup"><span data-stu-id="ed5b3-175">Response</span></span>

<span data-ttu-id="ed5b3-176">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-176">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="ed5b3-177">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="ed5b3-178">示例</span><span class="sxs-lookup"><span data-stu-id="ed5b3-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="ed5b3-179">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="ed5b3-179">Create an Office 365 group</span></span>

<span data-ttu-id="ed5b3-180">以下示例将创建一个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-180">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="ed5b3-181">请求</span><span class="sxs-lookup"><span data-stu-id="ed5b3-181">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="ed5b3-182">响应</span><span class="sxs-lookup"><span data-stu-id="ed5b3-182">Response</span></span>

<span data-ttu-id="ed5b3-183">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-183">The following is an example of the response.</span></span>

><span data-ttu-id="ed5b3-184">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-184">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ed5b3-185">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-185">All the default properties are returned from an actual call.</span></span>

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
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed5b3-186">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ed5b3-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed5b3-187">C#</span><span class="sxs-lookup"><span data-stu-id="ed5b3-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed5b3-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed5b3-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ed5b3-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed5b3-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="ed5b3-190">示例 2：创建包含所有者和成员的 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="ed5b3-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="ed5b3-191">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="ed5b3-192">请求</span><span class="sxs-lookup"><span data-stu-id="ed5b3-192">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
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
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="ed5b3-193">响应</span><span class="sxs-lookup"><span data-stu-id="ed5b3-193">Response</span></span> 

<span data-ttu-id="ed5b3-194">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-194">The following is an example of a successful response.</span></span> <span data-ttu-id="ed5b3-195">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-195">It includes only default properties.</span></span> <span data-ttu-id="ed5b3-196">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="ed5b3-197">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ed5b3-198">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="ed5b3-198">All the default properties are returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed5b3-199">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ed5b3-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed5b3-200">C#</span><span class="sxs-lookup"><span data-stu-id="ed5b3-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed5b3-201">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed5b3-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ed5b3-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed5b3-202">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="ed5b3-203">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ed5b3-203">See also</span></span>

- [<span data-ttu-id="ed5b3-204">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ed5b3-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ed5b3-205">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-205">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ed5b3-206">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ed5b3-206">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
