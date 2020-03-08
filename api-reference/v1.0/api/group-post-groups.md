---
title: 创建组
description: '创建请求正文中指定的新组。 '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 418c24dcb3779725cadb41e59c712c870d1bd74a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516989"
---
# <a name="create-group"></a><span data-ttu-id="e47cd-103">创建组</span><span class="sxs-lookup"><span data-stu-id="e47cd-103">Create group</span></span>

<span data-ttu-id="e47cd-104">命名空间：microsoft.graph 创建请求正文中指定的新组。</span><span class="sxs-lookup"><span data-stu-id="e47cd-104">Namespace: microsoft.graph Create a new group as specified in the request body.</span></span> <span data-ttu-id="e47cd-105">你可以创建以下类型的组：</span><span class="sxs-lookup"><span data-stu-id="e47cd-105">You can create the following types of groups:</span></span>

* <span data-ttu-id="e47cd-106">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="e47cd-106">Office 365 group (unified group)</span></span>
* <span data-ttu-id="e47cd-107">安全组</span><span class="sxs-lookup"><span data-stu-id="e47cd-107">Security group</span></span>

<span data-ttu-id="e47cd-108">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e47cd-109">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="e47cd-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="e47cd-110">若要获取_非_默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-110">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="e47cd-111">**注意：** 虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。</span><span class="sxs-lookup"><span data-stu-id="e47cd-111">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="e47cd-112">可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="e47cd-112">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="e47cd-113">权限</span><span class="sxs-lookup"><span data-stu-id="e47cd-113">Permissions</span></span>
<span data-ttu-id="e47cd-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e47cd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e47cd-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="e47cd-116">Permission type</span></span>      | <span data-ttu-id="e47cd-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e47cd-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e47cd-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e47cd-118">Delegated (work or school account)</span></span> | <span data-ttu-id="e47cd-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e47cd-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e47cd-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e47cd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e47cd-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="e47cd-121">Not supported.</span></span>    |
|<span data-ttu-id="e47cd-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="e47cd-122">Application</span></span> | <span data-ttu-id="e47cd-123">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47cd-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e47cd-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e47cd-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="e47cd-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e47cd-125">Request headers</span></span>
| <span data-ttu-id="e47cd-126">名称</span><span class="sxs-lookup"><span data-stu-id="e47cd-126">Name</span></span>       | <span data-ttu-id="e47cd-127">类型</span><span class="sxs-lookup"><span data-stu-id="e47cd-127">Type</span></span> | <span data-ttu-id="e47cd-128">说明</span><span class="sxs-lookup"><span data-stu-id="e47cd-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e47cd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e47cd-129">Authorization</span></span>  | <span data-ttu-id="e47cd-130">string</span><span class="sxs-lookup"><span data-stu-id="e47cd-130">string</span></span>  | <span data-ttu-id="e47cd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e47cd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e47cd-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e47cd-133">Content-Type</span></span>  | <span data-ttu-id="e47cd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="e47cd-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e47cd-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="e47cd-135">Request body</span></span>
<span data-ttu-id="e47cd-136">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="e47cd-137">属性</span><span class="sxs-lookup"><span data-stu-id="e47cd-137">Property</span></span> | <span data-ttu-id="e47cd-138">类型</span><span class="sxs-lookup"><span data-stu-id="e47cd-138">Type</span></span> | <span data-ttu-id="e47cd-139">说明</span><span class="sxs-lookup"><span data-stu-id="e47cd-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e47cd-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e47cd-140">displayName</span></span> | <span data-ttu-id="e47cd-141">string</span><span class="sxs-lookup"><span data-stu-id="e47cd-141">string</span></span> | <span data-ttu-id="e47cd-142">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="e47cd-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="e47cd-143">必需。</span><span class="sxs-lookup"><span data-stu-id="e47cd-143">Required.</span></span> |
| <span data-ttu-id="e47cd-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e47cd-144">mailEnabled</span></span> | <span data-ttu-id="e47cd-145">布尔</span><span class="sxs-lookup"><span data-stu-id="e47cd-145">boolean</span></span> | <span data-ttu-id="e47cd-146">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e47cd-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="e47cd-147">必需。</span><span class="sxs-lookup"><span data-stu-id="e47cd-147">Required.</span></span> |
| <span data-ttu-id="e47cd-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e47cd-148">mailNickname</span></span> | <span data-ttu-id="e47cd-149">string</span><span class="sxs-lookup"><span data-stu-id="e47cd-149">string</span></span> | <span data-ttu-id="e47cd-150">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="e47cd-150">The mail alias for the group.</span></span> <span data-ttu-id="e47cd-151">必需。</span><span class="sxs-lookup"><span data-stu-id="e47cd-151">Required.</span></span> |
| <span data-ttu-id="e47cd-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e47cd-152">securityEnabled</span></span> | <span data-ttu-id="e47cd-153">boolean</span><span class="sxs-lookup"><span data-stu-id="e47cd-153">boolean</span></span> | <span data-ttu-id="e47cd-154">对于启用安全机制的组（包括 Office 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e47cd-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="e47cd-155">必需。</span><span class="sxs-lookup"><span data-stu-id="e47cd-155">Required.</span></span> |
| <span data-ttu-id="e47cd-156">owners</span><span class="sxs-lookup"><span data-stu-id="e47cd-156">owners</span></span> | <span data-ttu-id="e47cd-157">string collection</span><span class="sxs-lookup"><span data-stu-id="e47cd-157">string collection</span></span> | <span data-ttu-id="e47cd-158">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="e47cd-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="e47cd-159">可选。</span><span class="sxs-lookup"><span data-stu-id="e47cd-159">Optional.</span></span> |
| <span data-ttu-id="e47cd-160">members</span><span class="sxs-lookup"><span data-stu-id="e47cd-160">members</span></span> | <span data-ttu-id="e47cd-161">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e47cd-161">string collection</span></span> | <span data-ttu-id="e47cd-162">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="e47cd-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="e47cd-163">可选。</span><span class="sxs-lookup"><span data-stu-id="e47cd-163">Optional.</span></span> |

> <span data-ttu-id="e47cd-164">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e47cd-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="e47cd-165">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="e47cd-166">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="e47cd-167">**注意：** 在不指定所有者的情况下使用 Group.Create 应用程序权限创建组时，将会以匿名方式创建组，并且组将不可修改。</span><span class="sxs-lookup"><span data-stu-id="e47cd-167">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="e47cd-168">创建组时，可使用 `POST` 操作并为其添加所有者，以便指定可修改该组的所有者。</span><span class="sxs-lookup"><span data-stu-id="e47cd-168">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="e47cd-169">以编程方式创建 Office 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="e47cd-169">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="e47cd-170">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="e47cd-170">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="e47cd-171">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="e47cd-171">groupTypes options</span></span>

<span data-ttu-id="e47cd-172">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="e47cd-172">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="e47cd-173">组类型</span><span class="sxs-lookup"><span data-stu-id="e47cd-173">Type of group</span></span> | <span data-ttu-id="e47cd-174">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="e47cd-174">Assigned membership</span></span> | <span data-ttu-id="e47cd-175">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="e47cd-175">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="e47cd-176">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="e47cd-176">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="e47cd-177">动态</span><span class="sxs-lookup"><span data-stu-id="e47cd-177">Dynamic</span></span> | <span data-ttu-id="e47cd-178">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="e47cd-178">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="e47cd-179">响应</span><span class="sxs-lookup"><span data-stu-id="e47cd-179">Response</span></span>
<span data-ttu-id="e47cd-180">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e47cd-180">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e47cd-181">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-181">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="e47cd-182">示例</span><span class="sxs-lookup"><span data-stu-id="e47cd-182">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="e47cd-183">示例 1：创建 Office 365 组</span><span class="sxs-lookup"><span data-stu-id="e47cd-183">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="e47cd-184">以下示例将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e47cd-184">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="e47cd-185">请求</span><span class="sxs-lookup"><span data-stu-id="e47cd-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e47cd-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47cd-186">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e47cd-187">C#</span><span class="sxs-lookup"><span data-stu-id="e47cd-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47cd-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47cd-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47cd-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47cd-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e47cd-190">Java</span><span class="sxs-lookup"><span data-stu-id="e47cd-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e47cd-191">响应</span><span class="sxs-lookup"><span data-stu-id="e47cd-191">Response</span></span>

<span data-ttu-id="e47cd-192">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e47cd-192">The following is an example of the response.</span></span>

><span data-ttu-id="e47cd-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e47cd-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e47cd-194">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-194">All the default properties are returned from an actual call.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="e47cd-195">示例 2：创建包含所有者和成员的组</span><span class="sxs-lookup"><span data-stu-id="e47cd-195">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="e47cd-196">以下示例将创建一个具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e47cd-196">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="e47cd-197">请求</span><span class="sxs-lookup"><span data-stu-id="e47cd-197">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e47cd-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="e47cd-198">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e47cd-199">C#</span><span class="sxs-lookup"><span data-stu-id="e47cd-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e47cd-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e47cd-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e47cd-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e47cd-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e47cd-202">Java</span><span class="sxs-lookup"><span data-stu-id="e47cd-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e47cd-203">响应</span><span class="sxs-lookup"><span data-stu-id="e47cd-203">Response</span></span>

<span data-ttu-id="e47cd-204">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="e47cd-204">The following is an example of a successful response.</span></span> <span data-ttu-id="e47cd-205">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-205">It includes only default properties.</span></span> <span data-ttu-id="e47cd-206">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="e47cd-206">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="e47cd-207">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e47cd-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e47cd-208">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="e47cd-208">All the default properties are returned from an actual call.</span></span>

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
