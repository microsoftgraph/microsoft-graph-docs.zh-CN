---
title: 创建组
description: '创建请求正文中指定的新组。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c3bd3331a9dacf3d2b2959f961a2e7f744d78898
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43061844"
---
# <a name="create-group"></a><span data-ttu-id="d40fa-103">创建组</span><span class="sxs-lookup"><span data-stu-id="d40fa-103">Create group</span></span>

<span data-ttu-id="d40fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d40fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d40fa-105">创建请求正文中指定的新组。</span><span class="sxs-lookup"><span data-stu-id="d40fa-105">Create a new group as specified in the request body.</span></span> <span data-ttu-id="d40fa-106">你可以创建以下类型的组：</span><span class="sxs-lookup"><span data-stu-id="d40fa-106">You can create the following types of groups:</span></span>

* <span data-ttu-id="d40fa-107">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="d40fa-107">Office 365 group (unified group)</span></span>
* <span data-ttu-id="d40fa-108">安全组</span><span class="sxs-lookup"><span data-stu-id="d40fa-108">Security group</span></span>

<span data-ttu-id="d40fa-109">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="d40fa-110">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="d40fa-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="d40fa-111">若要获取_非_默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="d40fa-112">**注意：** 虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。</span><span class="sxs-lookup"><span data-stu-id="d40fa-112">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="d40fa-113">可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="d40fa-113">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="d40fa-114">权限</span><span class="sxs-lookup"><span data-stu-id="d40fa-114">Permissions</span></span>
<span data-ttu-id="d40fa-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d40fa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d40fa-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="d40fa-117">Permission type</span></span>      | <span data-ttu-id="d40fa-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d40fa-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d40fa-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d40fa-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d40fa-120">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d40fa-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="d40fa-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d40fa-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d40fa-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d40fa-122">Not supported.</span></span>    |
|<span data-ttu-id="d40fa-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="d40fa-123">Application</span></span> | <span data-ttu-id="d40fa-124">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d40fa-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d40fa-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d40fa-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="d40fa-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="d40fa-126">Request headers</span></span>
| <span data-ttu-id="d40fa-127">名称</span><span class="sxs-lookup"><span data-stu-id="d40fa-127">Name</span></span>       | <span data-ttu-id="d40fa-128">类型</span><span class="sxs-lookup"><span data-stu-id="d40fa-128">Type</span></span> | <span data-ttu-id="d40fa-129">说明</span><span class="sxs-lookup"><span data-stu-id="d40fa-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d40fa-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d40fa-130">Authorization</span></span>  | <span data-ttu-id="d40fa-131">string</span><span class="sxs-lookup"><span data-stu-id="d40fa-131">string</span></span>  | <span data-ttu-id="d40fa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d40fa-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d40fa-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d40fa-134">Content-Type</span></span>  | <span data-ttu-id="d40fa-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d40fa-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d40fa-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="d40fa-136">Request body</span></span>
<span data-ttu-id="d40fa-137">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="d40fa-138">属性</span><span class="sxs-lookup"><span data-stu-id="d40fa-138">Property</span></span> | <span data-ttu-id="d40fa-139">类型</span><span class="sxs-lookup"><span data-stu-id="d40fa-139">Type</span></span> | <span data-ttu-id="d40fa-140">说明</span><span class="sxs-lookup"><span data-stu-id="d40fa-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d40fa-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d40fa-141">displayName</span></span> | <span data-ttu-id="d40fa-142">string</span><span class="sxs-lookup"><span data-stu-id="d40fa-142">string</span></span> | <span data-ttu-id="d40fa-143">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d40fa-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="d40fa-144">必需。</span><span class="sxs-lookup"><span data-stu-id="d40fa-144">Required.</span></span> |
| <span data-ttu-id="d40fa-145">description</span><span class="sxs-lookup"><span data-stu-id="d40fa-145">description</span></span> | <span data-ttu-id="d40fa-146">string</span><span class="sxs-lookup"><span data-stu-id="d40fa-146">string</span></span> | <span data-ttu-id="d40fa-147">组说明。</span><span class="sxs-lookup"><span data-stu-id="d40fa-147">A description for the group.</span></span> <span data-ttu-id="d40fa-148">最大</span><span class="sxs-lookup"><span data-stu-id="d40fa-148">Max.</span></span> <span data-ttu-id="d40fa-149">长度：1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="d40fa-149">length: 1024 characters.</span></span> <span data-ttu-id="d40fa-150">可选。</span><span class="sxs-lookup"><span data-stu-id="d40fa-150">Optional.</span></span> |
| <span data-ttu-id="d40fa-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d40fa-151">mailEnabled</span></span> | <span data-ttu-id="d40fa-152">布尔</span><span class="sxs-lookup"><span data-stu-id="d40fa-152">boolean</span></span> | <span data-ttu-id="d40fa-153">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d40fa-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="d40fa-154">必需。</span><span class="sxs-lookup"><span data-stu-id="d40fa-154">Required.</span></span> |
| <span data-ttu-id="d40fa-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d40fa-155">mailNickname</span></span> | <span data-ttu-id="d40fa-156">string</span><span class="sxs-lookup"><span data-stu-id="d40fa-156">string</span></span> | <span data-ttu-id="d40fa-157">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="d40fa-157">The mail alias for the group.</span></span> <span data-ttu-id="d40fa-158">必需。</span><span class="sxs-lookup"><span data-stu-id="d40fa-158">Required.</span></span> |
| <span data-ttu-id="d40fa-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d40fa-159">securityEnabled</span></span> | <span data-ttu-id="d40fa-160">boolean</span><span class="sxs-lookup"><span data-stu-id="d40fa-160">boolean</span></span> | <span data-ttu-id="d40fa-161">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d40fa-161">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="d40fa-162">必需。</span><span class="sxs-lookup"><span data-stu-id="d40fa-162">Required.</span></span> |
| <span data-ttu-id="d40fa-163">owners</span><span class="sxs-lookup"><span data-stu-id="d40fa-163">owners</span></span> | <span data-ttu-id="d40fa-164">string collection</span><span class="sxs-lookup"><span data-stu-id="d40fa-164">string collection</span></span> | <span data-ttu-id="d40fa-165">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="d40fa-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="d40fa-166">可选。</span><span class="sxs-lookup"><span data-stu-id="d40fa-166">Optional.</span></span> |
| <span data-ttu-id="d40fa-167">members</span><span class="sxs-lookup"><span data-stu-id="d40fa-167">members</span></span> | <span data-ttu-id="d40fa-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d40fa-168">string collection</span></span> | <span data-ttu-id="d40fa-169">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="d40fa-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="d40fa-170">可选。</span><span class="sxs-lookup"><span data-stu-id="d40fa-170">Optional.</span></span> |

> <span data-ttu-id="d40fa-171">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d40fa-171">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="d40fa-172">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-172">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="d40fa-173">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-173">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="d40fa-174">**注意：** 在不指定所有者的情况下使用 Group.Create 应用程序权限创建组时，将会以匿名方式创建组，并且组将不可修改。</span><span class="sxs-lookup"><span data-stu-id="d40fa-174">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="d40fa-175">创建组时，可使用 `POST` 操作并为其添加所有者，以便指定可修改该组的所有者。</span><span class="sxs-lookup"><span data-stu-id="d40fa-175">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="d40fa-176">以编程方式创建 Office 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="d40fa-176">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="d40fa-177">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="d40fa-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="d40fa-178">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="d40fa-178">groupTypes options</span></span>

<span data-ttu-id="d40fa-179">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="d40fa-179">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="d40fa-180">组类型</span><span class="sxs-lookup"><span data-stu-id="d40fa-180">Type of group</span></span> | <span data-ttu-id="d40fa-181">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="d40fa-181">Assigned membership</span></span> | <span data-ttu-id="d40fa-182">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="d40fa-182">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="d40fa-183">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="d40fa-183">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="d40fa-184">动态</span><span class="sxs-lookup"><span data-stu-id="d40fa-184">Dynamic</span></span> | <span data-ttu-id="d40fa-185">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="d40fa-185">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="d40fa-186">响应</span><span class="sxs-lookup"><span data-stu-id="d40fa-186">Response</span></span>
<span data-ttu-id="d40fa-187">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d40fa-187">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="d40fa-188">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-188">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="d40fa-189">示例</span><span class="sxs-lookup"><span data-stu-id="d40fa-189">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="d40fa-190">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="d40fa-190">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="d40fa-191">以下示例将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d40fa-191">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="d40fa-192">请求</span><span class="sxs-lookup"><span data-stu-id="d40fa-192">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d40fa-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="d40fa-193">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d40fa-194">C#</span><span class="sxs-lookup"><span data-stu-id="d40fa-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d40fa-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d40fa-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d40fa-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d40fa-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d40fa-197">Java</span><span class="sxs-lookup"><span data-stu-id="d40fa-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d40fa-198">响应</span><span class="sxs-lookup"><span data-stu-id="d40fa-198">Response</span></span>

<span data-ttu-id="d40fa-199">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d40fa-199">The following is an example of the response.</span></span>

><span data-ttu-id="d40fa-200">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d40fa-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d40fa-201">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-201">All the default properties are returned from an actual call.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="d40fa-202">示例 2：创建包含所有者和成员的组</span><span class="sxs-lookup"><span data-stu-id="d40fa-202">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="d40fa-203">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d40fa-203">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="d40fa-204">请求</span><span class="sxs-lookup"><span data-stu-id="d40fa-204">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d40fa-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="d40fa-205">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d40fa-206">C#</span><span class="sxs-lookup"><span data-stu-id="d40fa-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d40fa-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d40fa-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d40fa-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d40fa-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d40fa-209">Java</span><span class="sxs-lookup"><span data-stu-id="d40fa-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d40fa-210">响应</span><span class="sxs-lookup"><span data-stu-id="d40fa-210">Response</span></span>

<span data-ttu-id="d40fa-211">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="d40fa-211">The following is an example of a successful response.</span></span> <span data-ttu-id="d40fa-212">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-212">It includes only default properties.</span></span> <span data-ttu-id="d40fa-213">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="d40fa-213">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="d40fa-214">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d40fa-214">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d40fa-215">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="d40fa-215">All the default properties are returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
