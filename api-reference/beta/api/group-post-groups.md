---
title: 创建组
description: 创建新的 Microsoft 365 组或安全组。
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 871d990342807a9742ce9125c62e730fec39cd10
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507943"
---
# <a name="create-group"></a><span data-ttu-id="67ca6-103">创建组</span><span class="sxs-lookup"><span data-stu-id="67ca6-103">Create group</span></span>

<span data-ttu-id="67ca6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ca6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ca6-105">创建请求正文中指定的新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="67ca6-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="67ca6-106">你可以创建以下组之一：</span><span class="sxs-lookup"><span data-stu-id="67ca6-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="67ca6-107">Microsoft 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="67ca6-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="67ca6-108">安全组</span><span class="sxs-lookup"><span data-stu-id="67ca6-108">Security group</span></span>

<span data-ttu-id="67ca6-109">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="67ca6-110">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="67ca6-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="67ca6-111">若要获取 _非_ 默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="67ca6-112">**注意**：若要创建 [团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅 [创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="67ca6-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67ca6-113">权限</span><span class="sxs-lookup"><span data-stu-id="67ca6-113">Permissions</span></span>
<span data-ttu-id="67ca6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67ca6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ca6-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="67ca6-116">Permission type</span></span>      | <span data-ttu-id="67ca6-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67ca6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67ca6-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67ca6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="67ca6-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67ca6-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="67ca6-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67ca6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ca6-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="67ca6-121">Not supported.</span></span>    |
|<span data-ttu-id="67ca6-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="67ca6-122">Application</span></span> | <span data-ttu-id="67ca6-123">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ca6-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67ca6-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67ca6-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="67ca6-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="67ca6-125">Request headers</span></span>

| <span data-ttu-id="67ca6-126">名称</span><span class="sxs-lookup"><span data-stu-id="67ca6-126">Name</span></span>       | <span data-ttu-id="67ca6-127">类型</span><span class="sxs-lookup"><span data-stu-id="67ca6-127">Type</span></span> | <span data-ttu-id="67ca6-128">说明</span><span class="sxs-lookup"><span data-stu-id="67ca6-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67ca6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="67ca6-129">Authorization</span></span>  | <span data-ttu-id="67ca6-130">string</span><span class="sxs-lookup"><span data-stu-id="67ca6-130">string</span></span>  | <span data-ttu-id="67ca6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67ca6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67ca6-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="67ca6-133">Request body</span></span>

<span data-ttu-id="67ca6-134">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="67ca6-135">属性</span><span class="sxs-lookup"><span data-stu-id="67ca6-135">Property</span></span> | <span data-ttu-id="67ca6-136">类型</span><span class="sxs-lookup"><span data-stu-id="67ca6-136">Type</span></span> | <span data-ttu-id="67ca6-137">说明</span><span class="sxs-lookup"><span data-stu-id="67ca6-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67ca6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="67ca6-138">displayName</span></span> | <span data-ttu-id="67ca6-139">string</span><span class="sxs-lookup"><span data-stu-id="67ca6-139">string</span></span> | <span data-ttu-id="67ca6-140">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="67ca6-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="67ca6-141">必需。</span><span class="sxs-lookup"><span data-stu-id="67ca6-141">Required.</span></span> |
| <span data-ttu-id="67ca6-142">description</span><span class="sxs-lookup"><span data-stu-id="67ca6-142">description</span></span> | <span data-ttu-id="67ca6-143">string</span><span class="sxs-lookup"><span data-stu-id="67ca6-143">string</span></span> | <span data-ttu-id="67ca6-144">组说明。</span><span class="sxs-lookup"><span data-stu-id="67ca6-144">A description for the group.</span></span> <span data-ttu-id="67ca6-145">可选。</span><span class="sxs-lookup"><span data-stu-id="67ca6-145">Optional.</span></span> |
| <span data-ttu-id="67ca6-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="67ca6-146">isAssignableToRole</span></span> | <span data-ttu-id="67ca6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="67ca6-147">Boolean</span></span> | <span data-ttu-id="67ca6-148">设置为 **true** 可以将组分配给 Azure AD 角色。</span><span class="sxs-lookup"><span data-stu-id="67ca6-148">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="67ca6-149">只有特权角色管理员和全局管理员才能设置此属性的值。</span><span class="sxs-lookup"><span data-stu-id="67ca6-149">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="67ca6-150">可选。</span><span class="sxs-lookup"><span data-stu-id="67ca6-150">Optional.</span></span> |
| <span data-ttu-id="67ca6-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="67ca6-151">mailEnabled</span></span> | <span data-ttu-id="67ca6-152">布尔</span><span class="sxs-lookup"><span data-stu-id="67ca6-152">boolean</span></span> | <span data-ttu-id="67ca6-153">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="67ca6-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="67ca6-154">必需。</span><span class="sxs-lookup"><span data-stu-id="67ca6-154">Required.</span></span> |
| <span data-ttu-id="67ca6-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="67ca6-155">mailNickname</span></span> | <span data-ttu-id="67ca6-156">string</span><span class="sxs-lookup"><span data-stu-id="67ca6-156">string</span></span> | <span data-ttu-id="67ca6-157">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="67ca6-157">The mail alias for the group.</span></span> <span data-ttu-id="67ca6-158">无法在 mailNickName 中使用这些字符：`@()\[]";:.<>,SPACE`。</span><span class="sxs-lookup"><span data-stu-id="67ca6-158">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="67ca6-159">必填。</span><span class="sxs-lookup"><span data-stu-id="67ca6-159">Required.</span></span> |
| <span data-ttu-id="67ca6-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="67ca6-160">securityEnabled</span></span> | <span data-ttu-id="67ca6-161">boolean</span><span class="sxs-lookup"><span data-stu-id="67ca6-161">boolean</span></span> | <span data-ttu-id="67ca6-162">对于启用安全机制的组（包括 Microsoft 365 组），请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="67ca6-162">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="67ca6-163">必填。</span><span class="sxs-lookup"><span data-stu-id="67ca6-163">Required.</span></span> |
| <span data-ttu-id="67ca6-164">owners</span><span class="sxs-lookup"><span data-stu-id="67ca6-164">owners</span></span> | <span data-ttu-id="67ca6-165">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="67ca6-165">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="67ca6-166">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="67ca6-166">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="67ca6-167">可选。</span><span class="sxs-lookup"><span data-stu-id="67ca6-167">Optional.</span></span> |
| <span data-ttu-id="67ca6-168">members</span><span class="sxs-lookup"><span data-stu-id="67ca6-168">members</span></span> | <span data-ttu-id="67ca6-169">[directoryObject](../resources/directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="67ca6-169">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="67ca6-170">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="67ca6-170">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="67ca6-171">可选。</span><span class="sxs-lookup"><span data-stu-id="67ca6-171">Optional.</span></span> |
|<span data-ttu-id="67ca6-172">visibility</span><span class="sxs-lookup"><span data-stu-id="67ca6-172">visibility</span></span>|<span data-ttu-id="67ca6-173">字符串</span><span class="sxs-lookup"><span data-stu-id="67ca6-173">String</span></span>|<span data-ttu-id="67ca6-174">指定 Microsoft 365 组的可见性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-174">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="67ca6-175">可能的值是：`Private`、`Public`、`HiddenMembership` 或空（解释为 `Public`）。</span><span class="sxs-lookup"><span data-stu-id="67ca6-175">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="67ca6-176">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="67ca6-176">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="67ca6-177">由于 **组** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-177">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="67ca6-178">**注意：** 在不指定所有者的情况下使用 Group.Create 应用程序权限创建组时，将会以匿名方式创建组，并且组将不可修改。</span><span class="sxs-lookup"><span data-stu-id="67ca6-178">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="67ca6-179">创建组时，可使用 `POST` 操作并为其添加所有者，以便指定可修改该组的所有者。</span><span class="sxs-lookup"><span data-stu-id="67ca6-179">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="67ca6-180">以编程方式创建 Microsoft 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="67ca6-180">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="67ca6-181">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="67ca6-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="67ca6-182">根据需要为你的组指定其他可写属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-182">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="67ca6-183">有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-183">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="67ca6-184">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="67ca6-184">groupTypes options</span></span>

<span data-ttu-id="67ca6-185">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="67ca6-185">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="67ca6-186">组类型</span><span class="sxs-lookup"><span data-stu-id="67ca6-186">Type of group</span></span> | <span data-ttu-id="67ca6-187">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="67ca6-187">Assigned membership</span></span> | <span data-ttu-id="67ca6-188">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="67ca6-188">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="67ca6-189">Microsoft 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="67ca6-189">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="67ca6-190">动态</span><span class="sxs-lookup"><span data-stu-id="67ca6-190">Dynamic</span></span> | <span data-ttu-id="67ca6-191">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="67ca6-191">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="67ca6-192">响应</span><span class="sxs-lookup"><span data-stu-id="67ca6-192">Response</span></span>

<span data-ttu-id="67ca6-193">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67ca6-193">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="67ca6-194">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-194">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="67ca6-195">示例</span><span class="sxs-lookup"><span data-stu-id="67ca6-195">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="67ca6-196">示例 1：创建 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="67ca6-196">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="67ca6-197">以下示例将创建 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="67ca6-197">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="67ca6-198">请求</span><span class="sxs-lookup"><span data-stu-id="67ca6-198">Request</span></span>

<span data-ttu-id="67ca6-199">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67ca6-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67ca6-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ca6-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67ca6-201">C#</span><span class="sxs-lookup"><span data-stu-id="67ca6-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ca6-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ca6-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ca6-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ca6-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67ca6-204">Java</span><span class="sxs-lookup"><span data-stu-id="67ca6-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67ca6-205">响应</span><span class="sxs-lookup"><span data-stu-id="67ca6-205">Response</span></span>

<span data-ttu-id="67ca6-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67ca6-206">The following is an example of the response.</span></span>

><span data-ttu-id="67ca6-207">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="67ca6-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67ca6-208">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-208">All the default properties are returned from an actual call.</span></span>

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
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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
   "isAssignableToRole": null,
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
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-security-group-with-an-owner-and-members"></a><span data-ttu-id="67ca6-209">示例 2：创建包含所有者和成员的安全组</span><span class="sxs-lookup"><span data-stu-id="67ca6-209">Example 2: Create a security group with an owner and members</span></span>

<span data-ttu-id="67ca6-210">以下示例将创建一个具有指定所有者和成员的 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="67ca6-210">The following example creates a security group with an owner and members specified.</span></span> <span data-ttu-id="67ca6-211">请注意，最多可以在组创建中添加 20 个关系，如所有者和成员。</span><span class="sxs-lookup"><span data-stu-id="67ca6-211">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="67ca6-212">随后，可以通过使用[添加成员](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API 或 JSON 批处理来添加更多成员。</span><span class="sxs-lookup"><span data-stu-id="67ca6-212">You can subsequently add more members by using the [add member](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="67ca6-213">请求</span><span class="sxs-lookup"><span data-stu-id="67ca6-213">Request</span></span>

<span data-ttu-id="67ca6-214">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67ca6-214">The following is an example of the request.</span></span>

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
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="67ca6-215">响应</span><span class="sxs-lookup"><span data-stu-id="67ca6-215">Response</span></span> 

<span data-ttu-id="67ca6-216">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="67ca6-216">The following is an example of a successful response.</span></span> <span data-ttu-id="67ca6-217">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-217">It includes only default properties.</span></span> <span data-ttu-id="67ca6-218">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="67ca6-218">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="67ca6-219">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="67ca6-219">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67ca6-220">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-220">All the default properties are returned from an actual call.</span></span>

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
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": null,
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
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
    "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
    "theme": null,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="67ca6-221">示例 3：创建可以分配给 Azure AD 角色的组</span><span class="sxs-lookup"><span data-stu-id="67ca6-221">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="67ca6-222">请求</span><span class="sxs-lookup"><span data-stu-id="67ca6-222">Request</span></span>

<span data-ttu-id="67ca6-223">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67ca6-223">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67ca6-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ca6-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mailEnabled": true,
  "securityEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "visibility" : "Private"
}
```
# <a name="c"></a>[<span data-ttu-id="67ca6-225">C#</span><span class="sxs-lookup"><span data-stu-id="67ca6-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ca6-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ca6-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ca6-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ca6-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67ca6-228">Java</span><span class="sxs-lookup"><span data-stu-id="67ca6-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="67ca6-229">**注意：** 创建属性不需要 **可见性** 和 **groupTypes** 属性，但会使用这些值自动填充。</span><span class="sxs-lookup"><span data-stu-id="67ca6-229">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="67ca6-230">将 **isAssignableToRole** 属性设置为 `true` 的组不能具有动态成员资格类型。</span><span class="sxs-lookup"><span data-stu-id="67ca6-230">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="67ca6-231">有关更多信息，请参见[使用组来管理 Azure AD 角色分配](https://go.microsoft.com/fwlink/?linkid=2103037)。</span><span class="sxs-lookup"><span data-stu-id="67ca6-231">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="67ca6-232">响应</span><span class="sxs-lookup"><span data-stu-id="67ca6-232">Response</span></span>

<span data-ttu-id="67ca6-233">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="67ca6-233">The following is an example of the response.</span></span> <span data-ttu-id="67ca6-234">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="67ca6-234">It includes only default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
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
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "expirationDateTime": null,
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mail": "operations2019@contoso.com",
  "mailEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
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
  "securityEnabled": true,
  "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
  "theme": null,
  "visibility": "Private",
  "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="67ca6-235">另请参阅</span><span class="sxs-lookup"><span data-stu-id="67ca6-235">See also</span></span>

- [<span data-ttu-id="67ca6-236">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="67ca6-236">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="67ca6-237">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="67ca6-237">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="67ca6-238">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="67ca6-238">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


