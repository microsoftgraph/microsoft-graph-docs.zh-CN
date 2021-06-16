---
title: 创建组
description: '创建请求正文中指定的新组。 '
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c2f0163a6b37a556fc6db45e2daf75a8a4052a3
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941521"
---
# <a name="create-group"></a><span data-ttu-id="a2a59-103">创建组</span><span class="sxs-lookup"><span data-stu-id="a2a59-103">Create group</span></span>

<span data-ttu-id="a2a59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a59-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2a59-p101">创建请求正文中指定的新组。可以创建下列几种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="a2a59-p101">Create a new group as specified in the request body. You can create the following types of groups:</span></span>

* <span data-ttu-id="a2a59-107">Microsoft 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="a2a59-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="a2a59-108">安全组</span><span class="sxs-lookup"><span data-stu-id="a2a59-108">Security group</span></span>

<span data-ttu-id="a2a59-109">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="a2a59-110">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="a2a59-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="a2a59-111">若要获取 _非_ 默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="a2a59-112">**注意：** 虽然 Microsoft Teams 是在 Microsoft 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。</span><span class="sxs-lookup"><span data-stu-id="a2a59-112">**Note**: Although Microsoft Teams is built on Microsoft 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="a2a59-113">可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="a2a59-113">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2a59-114">权限</span><span class="sxs-lookup"><span data-stu-id="a2a59-114">Permissions</span></span>
<span data-ttu-id="a2a59-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2a59-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2a59-117">Permission type</span></span>      | <span data-ttu-id="a2a59-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2a59-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2a59-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2a59-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a2a59-120">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2a59-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="a2a59-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2a59-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2a59-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2a59-122">Not supported.</span></span>    |
|<span data-ttu-id="a2a59-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2a59-123">Application</span></span> | <span data-ttu-id="a2a59-124">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a59-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2a59-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2a59-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="a2a59-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2a59-126">Request headers</span></span>
| <span data-ttu-id="a2a59-127">名称</span><span class="sxs-lookup"><span data-stu-id="a2a59-127">Name</span></span>       | <span data-ttu-id="a2a59-128">类型</span><span class="sxs-lookup"><span data-stu-id="a2a59-128">Type</span></span> | <span data-ttu-id="a2a59-129">说明</span><span class="sxs-lookup"><span data-stu-id="a2a59-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2a59-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2a59-130">Authorization</span></span>  | <span data-ttu-id="a2a59-131">string</span><span class="sxs-lookup"><span data-stu-id="a2a59-131">string</span></span>  | <span data-ttu-id="a2a59-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2a59-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2a59-134">Content-Type</span></span>  | <span data-ttu-id="a2a59-135">application/json</span><span class="sxs-lookup"><span data-stu-id="a2a59-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2a59-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2a59-136">Request body</span></span>
<span data-ttu-id="a2a59-137">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="a2a59-138">属性</span><span class="sxs-lookup"><span data-stu-id="a2a59-138">Property</span></span> | <span data-ttu-id="a2a59-139">类型</span><span class="sxs-lookup"><span data-stu-id="a2a59-139">Type</span></span> | <span data-ttu-id="a2a59-140">说明</span><span class="sxs-lookup"><span data-stu-id="a2a59-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2a59-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a2a59-141">displayName</span></span> | <span data-ttu-id="a2a59-142">string</span><span class="sxs-lookup"><span data-stu-id="a2a59-142">string</span></span> | <span data-ttu-id="a2a59-p106">要在组的通讯簿中显示的名称。最大长度: 256 个字符。必填。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p106">The name to display in the address book for the group. Maximum length: 256 characters. Required.</span></span> |
| <span data-ttu-id="a2a59-146">说明</span><span class="sxs-lookup"><span data-stu-id="a2a59-146">description</span></span> | <span data-ttu-id="a2a59-147">string</span><span class="sxs-lookup"><span data-stu-id="a2a59-147">string</span></span> | <span data-ttu-id="a2a59-148">组说明。</span><span class="sxs-lookup"><span data-stu-id="a2a59-148">A description for the group.</span></span> <span data-ttu-id="a2a59-149">最大</span><span class="sxs-lookup"><span data-stu-id="a2a59-149">Max.</span></span> <span data-ttu-id="a2a59-150">长度：1024 个字符。</span><span class="sxs-lookup"><span data-stu-id="a2a59-150">length: 1024 characters.</span></span> <span data-ttu-id="a2a59-151">可选。</span><span class="sxs-lookup"><span data-stu-id="a2a59-151">Optional.</span></span> |
| <span data-ttu-id="a2a59-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a2a59-152">mailEnabled</span></span> | <span data-ttu-id="a2a59-153">布尔</span><span class="sxs-lookup"><span data-stu-id="a2a59-153">boolean</span></span> | <span data-ttu-id="a2a59-154">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a2a59-154">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="a2a59-155">必需。</span><span class="sxs-lookup"><span data-stu-id="a2a59-155">Required.</span></span> |
| <span data-ttu-id="a2a59-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a2a59-156">mailNickname</span></span> | <span data-ttu-id="a2a59-157">string</span><span class="sxs-lookup"><span data-stu-id="a2a59-157">string</span></span> | <span data-ttu-id="a2a59-158">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="a2a59-158">The mail alias for the group.</span></span> <span data-ttu-id="a2a59-159">最大</span><span class="sxs-lookup"><span data-stu-id="a2a59-159">Max.</span></span> <span data-ttu-id="a2a59-160">长度：64 个字符。</span><span class="sxs-lookup"><span data-stu-id="a2a59-160">length: 64 characters.</span></span> <span data-ttu-id="a2a59-161">无法在 mailNickName 中使用这些字符：`@()\[]";:.<>,SPACE`。</span><span class="sxs-lookup"><span data-stu-id="a2a59-161">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="a2a59-162">必填。</span><span class="sxs-lookup"><span data-stu-id="a2a59-162">Required.</span></span> |
| <span data-ttu-id="a2a59-163">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a2a59-163">securityEnabled</span></span> | <span data-ttu-id="a2a59-164">boolean</span><span class="sxs-lookup"><span data-stu-id="a2a59-164">boolean</span></span> | <span data-ttu-id="a2a59-165">对于启用安全机制的组（包括 Microsoft 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a2a59-165">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="a2a59-166">必填。</span><span class="sxs-lookup"><span data-stu-id="a2a59-166">Required.</span></span> |
| <span data-ttu-id="a2a59-167">owners</span><span class="sxs-lookup"><span data-stu-id="a2a59-167">owners</span></span> | <span data-ttu-id="a2a59-168">string collection</span><span class="sxs-lookup"><span data-stu-id="a2a59-168">string collection</span></span> | <span data-ttu-id="a2a59-p111">此属性表示创建时指定的组所有者。可选。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p111">This property represents the owners for the group at creation time. Optional.</span></span> |
| <span data-ttu-id="a2a59-171">members</span><span class="sxs-lookup"><span data-stu-id="a2a59-171">members</span></span> | <span data-ttu-id="a2a59-172">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a2a59-172">string collection</span></span> | <span data-ttu-id="a2a59-p112">此属性表示创建时指定的组成员。可选。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p112">This property represents the members for the group at creation time. Optional.</span></span> |
|<span data-ttu-id="a2a59-175">visibility</span><span class="sxs-lookup"><span data-stu-id="a2a59-175">visibility</span></span>|<span data-ttu-id="a2a59-176">String</span><span class="sxs-lookup"><span data-stu-id="a2a59-176">String</span></span>|<span data-ttu-id="a2a59-177">指定 Microsoft 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-177">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="a2a59-178">可能的值是：`Private`、`Public`、`HiddenMembership` 或空（解释为 `Public`）。</span><span class="sxs-lookup"><span data-stu-id="a2a59-178">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="a2a59-179">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="a2a59-179">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="a2a59-p114">根据需要为组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="a2a59-182">**注意：** 在不指定所有者的情况下使用 Group.Create 应用程序权限创建组时，将会以匿名方式创建组，并且组将不可修改。</span><span class="sxs-lookup"><span data-stu-id="a2a59-182">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="a2a59-183">创建组时，可使用 `POST` 操作并为其添加所有者，以便指定可修改该组的所有者。</span><span class="sxs-lookup"><span data-stu-id="a2a59-183">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="a2a59-184">以编程方式创建 Microsoft 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="a2a59-184">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="a2a59-185">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="a2a59-185">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="a2a59-186">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="a2a59-186">groupTypes options</span></span>

<span data-ttu-id="a2a59-187">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="a2a59-187">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="a2a59-188">组类型</span><span class="sxs-lookup"><span data-stu-id="a2a59-188">Type of group</span></span> | <span data-ttu-id="a2a59-189">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="a2a59-189">Assigned membership</span></span> | <span data-ttu-id="a2a59-190">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="a2a59-190">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="a2a59-191">Microsoft 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="a2a59-191">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="a2a59-192">动态</span><span class="sxs-lookup"><span data-stu-id="a2a59-192">Dynamic</span></span> | <span data-ttu-id="a2a59-193">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="a2a59-193">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="a2a59-194">响应</span><span class="sxs-lookup"><span data-stu-id="a2a59-194">Response</span></span>
<span data-ttu-id="a2a59-195">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2a59-195">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="a2a59-196">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-196">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="a2a59-197">示例</span><span class="sxs-lookup"><span data-stu-id="a2a59-197">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="a2a59-198">示例 1：创建 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="a2a59-198">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="a2a59-199">以下示例将创建 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="a2a59-199">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="a2a59-200">请求</span><span class="sxs-lookup"><span data-stu-id="a2a59-200">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a2a59-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2a59-201">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2a59-202">C#</span><span class="sxs-lookup"><span data-stu-id="a2a59-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2a59-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2a59-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2a59-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2a59-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2a59-205">Java</span><span class="sxs-lookup"><span data-stu-id="a2a59-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a2a59-206">响应</span><span class="sxs-lookup"><span data-stu-id="a2a59-206">Response</span></span>

<span data-ttu-id="a2a59-207">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2a59-207">The following is an example of the response.</span></span>

><span data-ttu-id="a2a59-208">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2a59-208">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="a2a59-209">示例 2：创建包含所有者和成员的组</span><span class="sxs-lookup"><span data-stu-id="a2a59-209">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="a2a59-210">以下示例将创建一个具有指定所有者和成员的安全组。</span><span class="sxs-lookup"><span data-stu-id="a2a59-210">The following example creates a Security group with an owner and members specified.</span></span> <span data-ttu-id="a2a59-211">请注意，最多可以在组创建中添加 20 个关系，如所有者和成员。</span><span class="sxs-lookup"><span data-stu-id="a2a59-211">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="a2a59-212">随后，可以通过使用[添加成员](group-post-members.md) API 或 JSON 批处理来添加更多成员。</span><span class="sxs-lookup"><span data-stu-id="a2a59-212">You can subsequently add more members by using the [add member](group-post-members.md) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="a2a59-213">请求</span><span class="sxs-lookup"><span data-stu-id="a2a59-213">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a2a59-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2a59-214">HTTP</span></span>](#tab/http)
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
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a2a59-215">C#</span><span class="sxs-lookup"><span data-stu-id="a2a59-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2a59-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2a59-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2a59-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2a59-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2a59-218">Java</span><span class="sxs-lookup"><span data-stu-id="a2a59-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a2a59-219">响应</span><span class="sxs-lookup"><span data-stu-id="a2a59-219">Response</span></span>

<span data-ttu-id="a2a59-220">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="a2a59-220">The following is an example of a successful response.</span></span> <span data-ttu-id="a2a59-221">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="a2a59-221">It includes only default properties.</span></span> <span data-ttu-id="a2a59-222">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="a2a59-222">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="a2a59-223">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2a59-223">**Note:** The response object shown here might be shortened for readability.</span></span>

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

