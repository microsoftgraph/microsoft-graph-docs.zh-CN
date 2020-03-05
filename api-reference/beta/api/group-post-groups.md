---
title: 创建组
description: 创建新的 Office 365 组或安全组。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ad934ae8d97d47cef6446def3305d0a6e365597
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418790"
---
# <a name="create-group"></a><span data-ttu-id="0b6cd-103">创建组</span><span class="sxs-lookup"><span data-stu-id="0b6cd-103">Create group</span></span>

<span data-ttu-id="0b6cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b6cd-105">创建请求正文中指定的新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="0b6cd-106">你可以创建以下组之一：</span><span class="sxs-lookup"><span data-stu-id="0b6cd-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="0b6cd-107">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-107">Office 365 group (unified group)</span></span>
* <span data-ttu-id="0b6cd-108">安全组</span><span class="sxs-lookup"><span data-stu-id="0b6cd-108">Security group</span></span>

<span data-ttu-id="0b6cd-109">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="0b6cd-110">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="0b6cd-111">若要获取_非_默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="0b6cd-112">**注意**：若要创建[团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b6cd-113">权限</span><span class="sxs-lookup"><span data-stu-id="0b6cd-113">Permissions</span></span>
<span data-ttu-id="0b6cd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b6cd-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b6cd-116">Permission type</span></span>      | <span data-ttu-id="0b6cd-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b6cd-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-118">Delegated (work or school account)</span></span> | <span data-ttu-id="0b6cd-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b6cd-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="0b6cd-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b6cd-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-121">Not supported.</span></span>    |
|<span data-ttu-id="0b6cd-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b6cd-122">Application</span></span> | <span data-ttu-id="0b6cd-123">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6cd-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b6cd-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b6cd-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="0b6cd-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b6cd-125">Request headers</span></span>

| <span data-ttu-id="0b6cd-126">名称</span><span class="sxs-lookup"><span data-stu-id="0b6cd-126">Name</span></span>       | <span data-ttu-id="0b6cd-127">类型</span><span class="sxs-lookup"><span data-stu-id="0b6cd-127">Type</span></span> | <span data-ttu-id="0b6cd-128">说明</span><span class="sxs-lookup"><span data-stu-id="0b6cd-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b6cd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b6cd-129">Authorization</span></span>  | <span data-ttu-id="0b6cd-130">string</span><span class="sxs-lookup"><span data-stu-id="0b6cd-130">string</span></span>  | <span data-ttu-id="0b6cd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b6cd-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b6cd-133">Request body</span></span>

<span data-ttu-id="0b6cd-134">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="0b6cd-135">属性</span><span class="sxs-lookup"><span data-stu-id="0b6cd-135">Property</span></span> | <span data-ttu-id="0b6cd-136">类型</span><span class="sxs-lookup"><span data-stu-id="0b6cd-136">Type</span></span> | <span data-ttu-id="0b6cd-137">说明</span><span class="sxs-lookup"><span data-stu-id="0b6cd-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b6cd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0b6cd-138">displayName</span></span> | <span data-ttu-id="0b6cd-139">string</span><span class="sxs-lookup"><span data-stu-id="0b6cd-139">string</span></span> | <span data-ttu-id="0b6cd-140">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="0b6cd-141">必需。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-141">Required.</span></span> |
| <span data-ttu-id="0b6cd-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6cd-142">mailEnabled</span></span> | <span data-ttu-id="0b6cd-143">布尔</span><span class="sxs-lookup"><span data-stu-id="0b6cd-143">boolean</span></span> | <span data-ttu-id="0b6cd-144">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="0b6cd-145">必需。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-145">Required.</span></span> |
| <span data-ttu-id="0b6cd-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0b6cd-146">mailNickname</span></span> | <span data-ttu-id="0b6cd-147">string</span><span class="sxs-lookup"><span data-stu-id="0b6cd-147">string</span></span> | <span data-ttu-id="0b6cd-148">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-148">The mail alias for the group.</span></span> <span data-ttu-id="0b6cd-149">必需。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-149">Required.</span></span> |
| <span data-ttu-id="0b6cd-150">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6cd-150">securityEnabled</span></span> | <span data-ttu-id="0b6cd-151">boolean</span><span class="sxs-lookup"><span data-stu-id="0b6cd-151">boolean</span></span> | <span data-ttu-id="0b6cd-152">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-152">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="0b6cd-153">必需。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-153">Required.</span></span> |
| <span data-ttu-id="0b6cd-154">owners</span><span class="sxs-lookup"><span data-stu-id="0b6cd-154">owners</span></span> | <span data-ttu-id="0b6cd-155">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="0b6cd-155">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="0b6cd-156">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="0b6cd-157">可选。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-157">Optional.</span></span> |
| <span data-ttu-id="0b6cd-158">members</span><span class="sxs-lookup"><span data-stu-id="0b6cd-158">members</span></span> | <span data-ttu-id="0b6cd-159">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="0b6cd-159">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="0b6cd-160">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="0b6cd-161">可选。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-161">Optional.</span></span> |

> <span data-ttu-id="0b6cd-162">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-162">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="0b6cd-163">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-163">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="0b6cd-164">**注意：** 在不指定所有者的情况下使用 Group.Create 应用程序权限创建组时，将会以匿名方式创建组，并且组将不可修改。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-164">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="0b6cd-165">创建组时，可使用 `POST` 操作并为其添加所有者，以便指定可修改该组的所有者。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-165">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="0b6cd-166">以编程方式创建 Office 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-166">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="0b6cd-167">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-167">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="0b6cd-168">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-168">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="0b6cd-169">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-169">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="0b6cd-170">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="0b6cd-170">groupTypes options</span></span>

<span data-ttu-id="0b6cd-171">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-171">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="0b6cd-172">组类型</span><span class="sxs-lookup"><span data-stu-id="0b6cd-172">Type of group</span></span> | <span data-ttu-id="0b6cd-173">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="0b6cd-173">Assigned membership</span></span> | <span data-ttu-id="0b6cd-174">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="0b6cd-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="0b6cd-175">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="0b6cd-176">动态</span><span class="sxs-lookup"><span data-stu-id="0b6cd-176">Dynamic</span></span> | <span data-ttu-id="0b6cd-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="0b6cd-177">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="0b6cd-178">响应</span><span class="sxs-lookup"><span data-stu-id="0b6cd-178">Response</span></span>

<span data-ttu-id="0b6cd-179">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-179">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="0b6cd-180">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="0b6cd-181">示例</span><span class="sxs-lookup"><span data-stu-id="0b6cd-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="0b6cd-182">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="0b6cd-182">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="0b6cd-183">以下示例将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="0b6cd-184">请求</span><span class="sxs-lookup"><span data-stu-id="0b6cd-184">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b6cd-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b6cd-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b6cd-186">C#</span><span class="sxs-lookup"><span data-stu-id="0b6cd-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b6cd-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b6cd-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b6cd-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b6cd-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b6cd-189">响应</span><span class="sxs-lookup"><span data-stu-id="0b6cd-189">Response</span></span>

<span data-ttu-id="0b6cd-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-190">The following is an example of the response.</span></span>

><span data-ttu-id="0b6cd-191">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b6cd-192">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-192">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="0b6cd-193">示例 2：创建包含所有者和成员的 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="0b6cd-193">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="0b6cd-194">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-194">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="0b6cd-195">请求</span><span class="sxs-lookup"><span data-stu-id="0b6cd-195">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b6cd-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b6cd-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b6cd-197">C#</span><span class="sxs-lookup"><span data-stu-id="0b6cd-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b6cd-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b6cd-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b6cd-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b6cd-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b6cd-200">响应</span><span class="sxs-lookup"><span data-stu-id="0b6cd-200">Response</span></span> 

<span data-ttu-id="0b6cd-201">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-201">The following is an example of a successful response.</span></span> <span data-ttu-id="0b6cd-202">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-202">It includes only default properties.</span></span> <span data-ttu-id="0b6cd-203">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-203">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="0b6cd-204">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-204">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b6cd-205">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="0b6cd-205">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0b6cd-206">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0b6cd-206">See also</span></span>

- [<span data-ttu-id="0b6cd-207">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0b6cd-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0b6cd-208">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-208">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0b6cd-209">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="0b6cd-209">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->
