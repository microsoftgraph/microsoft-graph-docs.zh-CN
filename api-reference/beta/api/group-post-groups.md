---
title: 创建组
description: 创建新的 Microsoft 365 组或安全组。
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 570b3a138e593586d55016f6640c68ddeeb188ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953817"
---
# <a name="create-group"></a><span data-ttu-id="7613e-103">创建组</span><span class="sxs-lookup"><span data-stu-id="7613e-103">Create group</span></span>

<span data-ttu-id="7613e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7613e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7613e-p101">创建请求正文中指定的新[组](../resources/group.md)。可以创建以下其中一个组：</span><span class="sxs-lookup"><span data-stu-id="7613e-p101">Create a new [group](../resources/group.md) as specified in the request body. You can create one of the following groups:</span></span>

* <span data-ttu-id="7613e-107">Microsoft 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="7613e-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="7613e-108">安全组</span><span class="sxs-lookup"><span data-stu-id="7613e-108">Security group</span></span>

<span data-ttu-id="7613e-p102">默认情况下，此操作仅返回每个组的属性子集。这些默认属性在 [属性](../resources/group.md#properties)部分进行了说明。要获取默认情况下 _未_ 返回的属性，请执行 [GET 操作](group-get.md)并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-p102">This operation returns by default only a subset of the properties for each group. These default properties are noted in the [Properties](../resources/group.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="7613e-112">**注意** ：若要创建 [团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅 [创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="7613e-112">**Note** : To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7613e-113">权限</span><span class="sxs-lookup"><span data-stu-id="7613e-113">Permissions</span></span>
<span data-ttu-id="7613e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7613e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7613e-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="7613e-116">Permission type</span></span>      | <span data-ttu-id="7613e-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7613e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7613e-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7613e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7613e-119">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7613e-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7613e-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7613e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7613e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="7613e-121">Not supported.</span></span>    |
|<span data-ttu-id="7613e-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="7613e-122">Application</span></span> | <span data-ttu-id="7613e-123">Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7613e-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7613e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7613e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7613e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7613e-125">Request headers</span></span>

| <span data-ttu-id="7613e-126">名称</span><span class="sxs-lookup"><span data-stu-id="7613e-126">Name</span></span>       | <span data-ttu-id="7613e-127">类型</span><span class="sxs-lookup"><span data-stu-id="7613e-127">Type</span></span> | <span data-ttu-id="7613e-128">说明</span><span class="sxs-lookup"><span data-stu-id="7613e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7613e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7613e-129">Authorization</span></span>  | <span data-ttu-id="7613e-130">string</span><span class="sxs-lookup"><span data-stu-id="7613e-130">string</span></span>  | <span data-ttu-id="7613e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7613e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7613e-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="7613e-133">Request body</span></span>

<span data-ttu-id="7613e-134">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7613e-135">属性</span><span class="sxs-lookup"><span data-stu-id="7613e-135">Property</span></span> | <span data-ttu-id="7613e-136">类型</span><span class="sxs-lookup"><span data-stu-id="7613e-136">Type</span></span> | <span data-ttu-id="7613e-137">说明</span><span class="sxs-lookup"><span data-stu-id="7613e-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7613e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7613e-138">displayName</span></span> | <span data-ttu-id="7613e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="7613e-139">string</span></span> | <span data-ttu-id="7613e-p105">将在组的通讯簿中显示的名称。必填。</span><span class="sxs-lookup"><span data-stu-id="7613e-p105">The name to display in the address book for the group. Required.</span></span> |
| <span data-ttu-id="7613e-142">description</span><span class="sxs-lookup"><span data-stu-id="7613e-142">description</span></span> | <span data-ttu-id="7613e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="7613e-143">string</span></span> | <span data-ttu-id="7613e-p106">对组的说明。可选。</span><span class="sxs-lookup"><span data-stu-id="7613e-p106">A description for the group. Optional.</span></span> |
| <span data-ttu-id="7613e-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="7613e-146">isAssignableToRole</span></span> | <span data-ttu-id="7613e-147">布尔值</span><span class="sxs-lookup"><span data-stu-id="7613e-147">Boolean</span></span> | <span data-ttu-id="7613e-p107">设置为 **true** 可以将组分配给 Azure AD 角色。只有特权角色管理员和全局管理员才能设置此属性的值。可选。</span><span class="sxs-lookup"><span data-stu-id="7613e-p107">Set to **true** to enable the group to be assigned to an Azure AD role. Only Privileged Role Administrator and Global Administrator can set the value of this property. Optional.</span></span> |
| <span data-ttu-id="7613e-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7613e-151">mailEnabled</span></span> | <span data-ttu-id="7613e-152">布尔值</span><span class="sxs-lookup"><span data-stu-id="7613e-152">boolean</span></span> | <span data-ttu-id="7613e-p108">对于已启用邮件的组，请设置为 **true** 。必填。</span><span class="sxs-lookup"><span data-stu-id="7613e-p108">Set to **true** for mail-enabled groups. Required.</span></span> |
| <span data-ttu-id="7613e-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7613e-155">mailNickname</span></span> | <span data-ttu-id="7613e-156">字符串</span><span class="sxs-lookup"><span data-stu-id="7613e-156">string</span></span> | <span data-ttu-id="7613e-p109">组的邮件别名。无法在 mailNickName: `@()\[]";:.<>,SPACE` 中使用这些字符。必填。</span><span class="sxs-lookup"><span data-stu-id="7613e-p109">The mail alias for the group. These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`. Required.</span></span> |
| <span data-ttu-id="7613e-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7613e-160">securityEnabled</span></span> | <span data-ttu-id="7613e-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="7613e-161">boolean</span></span> | <span data-ttu-id="7613e-p110">对于已启用安全机制的组（包括 Microsoft 365 组），请设置为 **true** 。必填。</span><span class="sxs-lookup"><span data-stu-id="7613e-p110">Set to **true** for security-enabled groups, including Microsoft 365 groups. Required.</span></span> |
| <span data-ttu-id="7613e-164">owners</span><span class="sxs-lookup"><span data-stu-id="7613e-164">owners</span></span> | <span data-ttu-id="7613e-165">[directoryObject](../resources/directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7613e-165">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="7613e-p111">此属性表示创建时指定的组所有者。可选。</span><span class="sxs-lookup"><span data-stu-id="7613e-p111">This property represents the owners for the group at creation time. Optional.</span></span> |
| <span data-ttu-id="7613e-168">members</span><span class="sxs-lookup"><span data-stu-id="7613e-168">members</span></span> | <span data-ttu-id="7613e-169">[directoryObject](../resources/directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7613e-169">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="7613e-p112">此属性表示创建时指定的组成员。可选。</span><span class="sxs-lookup"><span data-stu-id="7613e-p112">This property represents the members for the group at creation time. Optional.</span></span> |
|<span data-ttu-id="7613e-172">visibility</span><span class="sxs-lookup"><span data-stu-id="7613e-172">visibility</span></span>|<span data-ttu-id="7613e-173">字符串</span><span class="sxs-lookup"><span data-stu-id="7613e-173">String</span></span>|<span data-ttu-id="7613e-p113">指定 Microsoft 365 组的可见性。可能的值是：`Private`、`Public`、`HiddenMembership` 或空（解释为 `Public`）。</span><span class="sxs-lookup"><span data-stu-id="7613e-p113">Specifies the visibility of a Microsoft 365 group. Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="7613e-176">**注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。</span><span class="sxs-lookup"><span data-stu-id="7613e-176">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="7613e-177">由于 **组** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-177">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7613e-p114">**注意：** 使用“组”创建组。创建应用程序权限而不指定所有者将匿名创建组，并且该组不可修改。可以使用 `POST` 操作并在创建组时将所有者添加到组中，以指定可以修改组的所有者。</span><span class="sxs-lookup"><span data-stu-id="7613e-p114">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable. You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="7613e-p115">通过仅应用上下文以编程方式创建 Microsoft 365 组而不指定所有者将匿名创建组。这样做可能导致在执行进一步的手动操作之前，不会自动创建关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="7613e-p115">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously. Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7613e-p116">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-p116">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="7613e-184">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="7613e-184">groupTypes options</span></span>

<span data-ttu-id="7613e-185">使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。</span><span class="sxs-lookup"><span data-stu-id="7613e-185">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="7613e-186">组类型</span><span class="sxs-lookup"><span data-stu-id="7613e-186">Type of group</span></span> | <span data-ttu-id="7613e-187">已分配成员身份</span><span class="sxs-lookup"><span data-stu-id="7613e-187">Assigned membership</span></span> | <span data-ttu-id="7613e-188">动态成员身份</span><span class="sxs-lookup"><span data-stu-id="7613e-188">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="7613e-189">Microsoft 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="7613e-189">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="7613e-190">动态</span><span class="sxs-lookup"><span data-stu-id="7613e-190">Dynamic</span></span> | <span data-ttu-id="7613e-191">`[]` ( _null_ )</span><span class="sxs-lookup"><span data-stu-id="7613e-191">`[]` ( _null_ )</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="7613e-192">响应</span><span class="sxs-lookup"><span data-stu-id="7613e-192">Response</span></span>

<span data-ttu-id="7613e-p117">如果成功，此方法将在响应正文中返回一个 `201 Created` 响应代码和一个[组](../resources/group.md)对象。该响应仅包含该组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-p117">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body. The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="7613e-195">示例</span><span class="sxs-lookup"><span data-stu-id="7613e-195">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="7613e-196">示例 1：创建 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="7613e-196">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="7613e-197">以下示例将创建 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="7613e-197">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="7613e-198">请求</span><span class="sxs-lookup"><span data-stu-id="7613e-198">Request</span></span>

<span data-ttu-id="7613e-199">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7613e-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7613e-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="7613e-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7613e-201">C#</span><span class="sxs-lookup"><span data-stu-id="7613e-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7613e-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7613e-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7613e-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7613e-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7613e-204">Java</span><span class="sxs-lookup"><span data-stu-id="7613e-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7613e-205">响应</span><span class="sxs-lookup"><span data-stu-id="7613e-205">Response</span></span>

<span data-ttu-id="7613e-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7613e-206">The following is an example of the response.</span></span>

><span data-ttu-id="7613e-207">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7613e-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7613e-208">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-208">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-a-microsoft-365-group-with-an-owner-and-members"></a><span data-ttu-id="7613e-209">示例 2：创建包含所有者和成员的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="7613e-209">Example 2: Create a Microsoft 365 group with an owner and members</span></span>

<span data-ttu-id="7613e-210">以下示例将创建一个具有指定所有者和成员的 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="7613e-210">The following example creates a Microsoft 365 group with an owner and members specified.</span></span> <span data-ttu-id="7613e-211">请注意，最多可以在组创建中添加 20 个关系，如所有者和成员。</span><span class="sxs-lookup"><span data-stu-id="7613e-211">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="7613e-212">随后，可以通过使用[添加成员](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API 或 JSON 批处理来添加更多成员。</span><span class="sxs-lookup"><span data-stu-id="7613e-212">You can subsequently add more members by using the [add member](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="7613e-213">请求</span><span class="sxs-lookup"><span data-stu-id="7613e-213">Request</span></span>

<span data-ttu-id="7613e-214">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7613e-214">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
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

#### <a name="response"></a><span data-ttu-id="7613e-215">响应</span><span class="sxs-lookup"><span data-stu-id="7613e-215">Response</span></span> 

<span data-ttu-id="7613e-216">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="7613e-216">The following is an example of a successful response.</span></span> <span data-ttu-id="7613e-217">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-217">It includes only default properties.</span></span> <span data-ttu-id="7613e-218">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="7613e-218">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="7613e-219">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7613e-219">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7613e-220">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-220">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="7613e-221">示例 3：创建可以分配给 Azure AD 角色的组</span><span class="sxs-lookup"><span data-stu-id="7613e-221">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="7613e-222">请求</span><span class="sxs-lookup"><span data-stu-id="7613e-222">Request</span></span>

<span data-ttu-id="7613e-223">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7613e-223">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7613e-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="7613e-224">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7613e-225">C#</span><span class="sxs-lookup"><span data-stu-id="7613e-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7613e-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7613e-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7613e-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7613e-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7613e-228">Java</span><span class="sxs-lookup"><span data-stu-id="7613e-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="7613e-229">**注意：** 创建属性不需要 **visibility** 和 **groupTypes** 属性，但会使用这些值自动填充。</span><span class="sxs-lookup"><span data-stu-id="7613e-229">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="7613e-230">将 **isAssignableToRole** 属性设置为 `true` 的组不能具有动态成员资格类型。</span><span class="sxs-lookup"><span data-stu-id="7613e-230">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="7613e-231">有关更多信息，请参见[使用组来管理 Azure AD 角色分配](https://go.microsoft.com/fwlink/?linkid=2103037)。</span><span class="sxs-lookup"><span data-stu-id="7613e-231">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="7613e-232">响应</span><span class="sxs-lookup"><span data-stu-id="7613e-232">Response</span></span>

<span data-ttu-id="7613e-233">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7613e-233">The following is an example of the response.</span></span> <span data-ttu-id="7613e-234">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="7613e-234">It includes only default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7613e-235">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7613e-235">See also</span></span>

- [<span data-ttu-id="7613e-236">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7613e-236">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7613e-237">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7613e-237">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7613e-238">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7613e-238">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


