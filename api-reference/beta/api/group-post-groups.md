---
title: 创建组
description: 创建新的 Office 365 组或安全组。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: c91c43c0156aa4edda9eef71232001fdede38887
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536195"
---
# <a name="create-group"></a><span data-ttu-id="960b1-103">创建组</span><span class="sxs-lookup"><span data-stu-id="960b1-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="960b1-104">创建请求正文中指定的新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="960b1-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="960b1-105">你可以创建以下组之一：</span><span class="sxs-lookup"><span data-stu-id="960b1-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="960b1-106">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="960b1-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="960b1-107">安全组</span><span class="sxs-lookup"><span data-stu-id="960b1-107">Security group</span></span>

<span data-ttu-id="960b1-108">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="960b1-109">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="960b1-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="960b1-110">若要获取_非_默认返回的属性，请执行 GET 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="960b1-111">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="960b1-111">See an [example](group-get.md#request-2).</span></span>

><span data-ttu-id="960b1-112">**注意**：若要创建[团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="960b1-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="960b1-113">权限</span><span class="sxs-lookup"><span data-stu-id="960b1-113">Permissions</span></span>
<span data-ttu-id="960b1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="960b1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="960b1-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="960b1-116">Permission type</span></span>      | <span data-ttu-id="960b1-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="960b1-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="960b1-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="960b1-118">Delegated (work or school account)</span></span> | <span data-ttu-id="960b1-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="960b1-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="960b1-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="960b1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="960b1-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="960b1-121">Not supported.</span></span>    |
|<span data-ttu-id="960b1-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="960b1-122">Application</span></span> | <span data-ttu-id="960b1-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="960b1-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="960b1-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="960b1-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="960b1-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="960b1-125">Request headers</span></span>

| <span data-ttu-id="960b1-126">名称</span><span class="sxs-lookup"><span data-stu-id="960b1-126">Name</span></span>       | <span data-ttu-id="960b1-127">类型</span><span class="sxs-lookup"><span data-stu-id="960b1-127">Type</span></span> | <span data-ttu-id="960b1-128">说明</span><span class="sxs-lookup"><span data-stu-id="960b1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="960b1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="960b1-129">Authorization</span></span>  | <span data-ttu-id="960b1-130">string</span><span class="sxs-lookup"><span data-stu-id="960b1-130">string</span></span>  | <span data-ttu-id="960b1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="960b1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="960b1-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="960b1-133">Request body</span></span>

<span data-ttu-id="960b1-134">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="960b1-135">属性</span><span class="sxs-lookup"><span data-stu-id="960b1-135">Property</span></span> | <span data-ttu-id="960b1-136">类型</span><span class="sxs-lookup"><span data-stu-id="960b1-136">Type</span></span> | <span data-ttu-id="960b1-137">说明</span><span class="sxs-lookup"><span data-stu-id="960b1-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="960b1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="960b1-138">displayName</span></span> | <span data-ttu-id="960b1-139">string</span><span class="sxs-lookup"><span data-stu-id="960b1-139">string</span></span> | <span data-ttu-id="960b1-140">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="960b1-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="960b1-141">必需。</span><span class="sxs-lookup"><span data-stu-id="960b1-141">Required.</span></span> |
| <span data-ttu-id="960b1-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="960b1-142">mailEnabled</span></span> | <span data-ttu-id="960b1-143">布尔</span><span class="sxs-lookup"><span data-stu-id="960b1-143">boolean</span></span> | <span data-ttu-id="960b1-144">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="960b1-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="960b1-145">必需。</span><span class="sxs-lookup"><span data-stu-id="960b1-145">Required.</span></span> |
| <span data-ttu-id="960b1-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="960b1-146">mailNickname</span></span> | <span data-ttu-id="960b1-147">string</span><span class="sxs-lookup"><span data-stu-id="960b1-147">string</span></span> | <span data-ttu-id="960b1-148">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="960b1-148">The mail alias for the group.</span></span> <span data-ttu-id="960b1-149">必需。</span><span class="sxs-lookup"><span data-stu-id="960b1-149">Required.</span></span> |
| <span data-ttu-id="960b1-150">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="960b1-150">securityEnabled</span></span> | <span data-ttu-id="960b1-151">boolean</span><span class="sxs-lookup"><span data-stu-id="960b1-151">boolean</span></span> | <span data-ttu-id="960b1-152">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="960b1-152">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="960b1-153">必需。</span><span class="sxs-lookup"><span data-stu-id="960b1-153">Required.</span></span> |
| <span data-ttu-id="960b1-154">owners</span><span class="sxs-lookup"><span data-stu-id="960b1-154">owners</span></span> | <span data-ttu-id="960b1-155">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="960b1-155">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="960b1-156">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="960b1-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="960b1-157">可选。</span><span class="sxs-lookup"><span data-stu-id="960b1-157">Optional.</span></span> |
| <span data-ttu-id="960b1-158">members</span><span class="sxs-lookup"><span data-stu-id="960b1-158">members</span></span> | <span data-ttu-id="960b1-159">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="960b1-159">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="960b1-160">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="960b1-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="960b1-161">可选。</span><span class="sxs-lookup"><span data-stu-id="960b1-161">Optional.</span></span> |

> <span data-ttu-id="960b1-162">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="960b1-162">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="960b1-163">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-163">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="960b1-164">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="960b1-164">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="960b1-165">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="960b1-165">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="960b1-p113">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="960b1-168">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="960b1-168">groupTypes options</span></span>

<span data-ttu-id="960b1-169">使用 **groupTypes** 属性来控制组的类型及其成员身份，如下所示：</span><span class="sxs-lookup"><span data-stu-id="960b1-169">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="960b1-170">组类型</span><span class="sxs-lookup"><span data-stu-id="960b1-170">Type of group</span></span> | <span data-ttu-id="960b1-171">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="960b1-171">Assigned membership</span></span> | <span data-ttu-id="960b1-172">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="960b1-172">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="960b1-173">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="960b1-173">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="960b1-174">动态</span><span class="sxs-lookup"><span data-stu-id="960b1-174">Dynamic</span></span> | <span data-ttu-id="960b1-175">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="960b1-175">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="960b1-176">响应</span><span class="sxs-lookup"><span data-stu-id="960b1-176">Response</span></span>

<span data-ttu-id="960b1-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="960b1-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="960b1-178">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-178">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="960b1-179">示例</span><span class="sxs-lookup"><span data-stu-id="960b1-179">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="960b1-180">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="960b1-180">Create an Office 365 group</span></span>

<span data-ttu-id="960b1-181">以下示例将创建一个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="960b1-181">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="960b1-182">请求</span><span class="sxs-lookup"><span data-stu-id="960b1-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="960b1-183">响应</span><span class="sxs-lookup"><span data-stu-id="960b1-183">Response</span></span>

<span data-ttu-id="960b1-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="960b1-184">The following is an example of the response.</span></span>

><span data-ttu-id="960b1-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="960b1-185">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="960b1-186">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-186">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="960b1-187">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="960b1-187">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="960b1-188">C#</span><span class="sxs-lookup"><span data-stu-id="960b1-188">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="960b1-189">Javascript</span><span class="sxs-lookup"><span data-stu-id="960b1-189">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="960b1-190">示例 2：创建包含所有者和成员的 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="960b1-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="960b1-191">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="960b1-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="960b1-192">请求</span><span class="sxs-lookup"><span data-stu-id="960b1-192">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="960b1-193">响应</span><span class="sxs-lookup"><span data-stu-id="960b1-193">Response</span></span> 

<span data-ttu-id="960b1-194">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="960b1-194">The following is an example of a successful response.</span></span> <span data-ttu-id="960b1-195">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-195">It includes only default properties.</span></span> <span data-ttu-id="960b1-196">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="960b1-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="960b1-197">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="960b1-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="960b1-198">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="960b1-198">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="960b1-199">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="960b1-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="960b1-200">C#</span><span class="sxs-lookup"><span data-stu-id="960b1-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="960b1-201">Javascript</span><span class="sxs-lookup"><span data-stu-id="960b1-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="960b1-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="960b1-202">See also</span></span>

- [<span data-ttu-id="960b1-203">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="960b1-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="960b1-204">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="960b1-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="960b1-205">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="960b1-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
