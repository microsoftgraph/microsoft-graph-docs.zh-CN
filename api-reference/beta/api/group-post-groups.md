---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de304cc4faaa6e4b64992ba0d7b2af35e8b5900a
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353067"
---
# <a name="create-group"></a><span data-ttu-id="e9da3-104">创建组</span><span class="sxs-lookup"><span data-stu-id="e9da3-104">Create group</span></span>

> <span data-ttu-id="e9da3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e9da3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9da3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9da3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9da3-107">使用此 API 可以创建请求正文中指定的新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="e9da3-107">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span> <span data-ttu-id="e9da3-108">可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="e9da3-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="e9da3-109">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="e9da3-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="e9da3-110">动态组</span><span class="sxs-lookup"><span data-stu-id="e9da3-110">Dynamic group</span></span>
* <span data-ttu-id="e9da3-111">安全组</span><span class="sxs-lookup"><span data-stu-id="e9da3-111">Security group</span></span>

<span data-ttu-id="e9da3-112">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-112">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e9da3-113">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="e9da3-113">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="e9da3-114">若要获取_非_默认返回的属性，请执行 GET 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-114">To get properties that are _not_ returned by default, do a GET operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e9da3-115">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="e9da3-115">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="e9da3-116">**注意**：若要创建[团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="e9da3-116">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9da3-117">权限</span><span class="sxs-lookup"><span data-stu-id="e9da3-117">Permissions</span></span>
<span data-ttu-id="e9da3-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9da3-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9da3-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9da3-120">Permission type</span></span>      | <span data-ttu-id="e9da3-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9da3-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9da3-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9da3-122">Delegated (work or school account)</span></span> | <span data-ttu-id="e9da3-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9da3-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9da3-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9da3-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9da3-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9da3-125">Not supported.</span></span>    |
|<span data-ttu-id="e9da3-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9da3-126">Application</span></span> | <span data-ttu-id="e9da3-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9da3-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9da3-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9da3-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="e9da3-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9da3-129">Request headers</span></span>
| <span data-ttu-id="e9da3-130">名称</span><span class="sxs-lookup"><span data-stu-id="e9da3-130">Name</span></span>       | <span data-ttu-id="e9da3-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9da3-131">Type</span></span> | <span data-ttu-id="e9da3-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9da3-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9da3-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9da3-133">Authorization</span></span>  | <span data-ttu-id="e9da3-134">string</span><span class="sxs-lookup"><span data-stu-id="e9da3-134">string</span></span>  | <span data-ttu-id="e9da3-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9da3-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9da3-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9da3-137">Request body</span></span>
<span data-ttu-id="e9da3-138">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-138">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="e9da3-139">属性</span><span class="sxs-lookup"><span data-stu-id="e9da3-139">Property</span></span> | <span data-ttu-id="e9da3-140">类型</span><span class="sxs-lookup"><span data-stu-id="e9da3-140">Type</span></span> | <span data-ttu-id="e9da3-141">说明</span><span class="sxs-lookup"><span data-stu-id="e9da3-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9da3-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e9da3-142">displayName</span></span> | <span data-ttu-id="e9da3-143">string</span><span class="sxs-lookup"><span data-stu-id="e9da3-143">string</span></span> | <span data-ttu-id="e9da3-144">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="e9da3-144">The name to display in the address book for the group.</span></span> <span data-ttu-id="e9da3-145">必需。</span><span class="sxs-lookup"><span data-stu-id="e9da3-145">Required.</span></span> |
| <span data-ttu-id="e9da3-146">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e9da3-146">mailEnabled</span></span> | <span data-ttu-id="e9da3-147">布尔</span><span class="sxs-lookup"><span data-stu-id="e9da3-147">boolean</span></span> | <span data-ttu-id="e9da3-148">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-148">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="e9da3-149">如果创建 Office 365 组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-149">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="e9da3-150">如果创建动态或安全组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-150">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="e9da3-151">必需。</span><span class="sxs-lookup"><span data-stu-id="e9da3-151">Required.</span></span> |
| <span data-ttu-id="e9da3-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e9da3-152">mailNickname</span></span> | <span data-ttu-id="e9da3-153">string</span><span class="sxs-lookup"><span data-stu-id="e9da3-153">string</span></span> | <span data-ttu-id="e9da3-154">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="e9da3-154">The mail alias for the group.</span></span> <span data-ttu-id="e9da3-155">必需。</span><span class="sxs-lookup"><span data-stu-id="e9da3-155">Required.</span></span> |
| <span data-ttu-id="e9da3-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e9da3-156">securityEnabled</span></span> | <span data-ttu-id="e9da3-157">布尔</span><span class="sxs-lookup"><span data-stu-id="e9da3-157">boolean</span></span> | <span data-ttu-id="e9da3-158">对于启用安全机制的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-158">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="e9da3-159">如果创建动态或安全组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-159">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="e9da3-160">如果创建 Office 365 组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="e9da3-160">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="e9da3-161">必需。</span><span class="sxs-lookup"><span data-stu-id="e9da3-161">Required.</span></span> |
| <span data-ttu-id="e9da3-162">owners</span><span class="sxs-lookup"><span data-stu-id="e9da3-162">owners</span></span> | <span data-ttu-id="e9da3-163">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e9da3-163">string collection</span></span> | <span data-ttu-id="e9da3-164">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="e9da3-164">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="e9da3-165">可选。</span><span class="sxs-lookup"><span data-stu-id="e9da3-165">Optional.</span></span> |
| <span data-ttu-id="e9da3-166">members</span><span class="sxs-lookup"><span data-stu-id="e9da3-166">members</span></span> | <span data-ttu-id="e9da3-167">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e9da3-167">string collection</span></span> | <span data-ttu-id="e9da3-168">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="e9da3-168">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="e9da3-169">可选。</span><span class="sxs-lookup"><span data-stu-id="e9da3-169">Optional.</span></span> |

<span data-ttu-id="e9da3-170">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-170">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="e9da3-171">组类型</span><span class="sxs-lookup"><span data-stu-id="e9da3-171">Type of group</span></span> | <span data-ttu-id="e9da3-172">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="e9da3-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="e9da3-173">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="e9da3-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="e9da3-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="e9da3-174">"Unified"</span></span> |
| <span data-ttu-id="e9da3-175">Dynamic</span><span class="sxs-lookup"><span data-stu-id="e9da3-175">Dynamic</span></span> | <span data-ttu-id="e9da3-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="e9da3-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="e9da3-177">安全性</span><span class="sxs-lookup"><span data-stu-id="e9da3-177">Security</span></span> | <span data-ttu-id="e9da3-178">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="e9da3-178">Do not set.</span></span> |

<span data-ttu-id="e9da3-179">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-179">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

><span data-ttu-id="e9da3-180">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="e9da3-180">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="e9da3-181">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="e9da3-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="e9da3-p115">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="e9da3-184">响应</span><span class="sxs-lookup"><span data-stu-id="e9da3-184">Response</span></span>
<span data-ttu-id="e9da3-185">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9da3-185">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e9da3-186">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-186">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="e9da3-187">示例</span><span class="sxs-lookup"><span data-stu-id="e9da3-187">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e9da3-188">请求 1</span><span class="sxs-lookup"><span data-stu-id="e9da3-188">Request 1</span></span>
<span data-ttu-id="e9da3-189">第一个示例请求将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e9da3-189">The following is an example of a request that creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
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

#### <a name="response"></a><span data-ttu-id="e9da3-190">响应</span><span class="sxs-lookup"><span data-stu-id="e9da3-190">Response</span></span>
<span data-ttu-id="e9da3-191">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e9da3-191">The following is an example of the response.</span></span>
><span data-ttu-id="e9da3-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9da3-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e9da3-193">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-193">All the default properties are returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
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

#### <a name="request-2"></a><span data-ttu-id="e9da3-194">请求 2</span><span class="sxs-lookup"><span data-stu-id="e9da3-194">Request 2</span></span>
<span data-ttu-id="e9da3-195">第二个示例请求将创建具有指定所有者的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="e9da3-195">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a><span data-ttu-id="e9da3-196">响应 2</span><span class="sxs-lookup"><span data-stu-id="e9da3-196">Response 2</span></span>
<span data-ttu-id="e9da3-197">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="e9da3-197">The following is an example of a response to a  event.</span></span> <span data-ttu-id="e9da3-198">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-198">It includes only the default properties.</span></span> <span data-ttu-id="e9da3-199">随后可获取组的 **owners** 导航属性，来验证所有者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e9da3-199">You can subsequenty get the **owners** navigation property of the group to verify the details of the owner.</span></span> 
><span data-ttu-id="e9da3-200">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9da3-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e9da3-201">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="e9da3-201">All the default properties are returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "502df398-d59c-469d-944f-34a50e60db3f",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-27T22:17:07Z",
     "description": "Group with designated owner",
     "displayName": "Operations group",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "operations2019@contoso.com",
     "mailEnabled": true,
     "mailNickname": "operations2019",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:operations2019@contoso.com"
     ],
     "renewedDateTime": "2018-12-27T22:17:07Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="e9da3-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e9da3-202">See also</span></span>

- [<span data-ttu-id="e9da3-203">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e9da3-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e9da3-204">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="e9da3-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e9da3-205">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="e9da3-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
