---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 87494b309dd731c519f0d999396f283c5a2fa583
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515907"
---
# <a name="create-group"></a><span data-ttu-id="d23ea-104">创建组</span><span class="sxs-lookup"><span data-stu-id="d23ea-104">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d23ea-p102">使用此 API 可以创建请求正文中指定的新[组](../resources/group.md)。可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="d23ea-p102">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="d23ea-107">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="d23ea-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="d23ea-108">动态组</span><span class="sxs-lookup"><span data-stu-id="d23ea-108">Dynamic group</span></span>
* <span data-ttu-id="d23ea-109">安全组</span><span class="sxs-lookup"><span data-stu-id="d23ea-109">Security group</span></span>

<span data-ttu-id="d23ea-110">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="d23ea-111">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="d23ea-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="d23ea-112">若要获取_非_默认返回的属性，请执行 GET 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="d23ea-113">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="d23ea-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="d23ea-114">**注意**：若要创建[团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="d23ea-114">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d23ea-115">权限</span><span class="sxs-lookup"><span data-stu-id="d23ea-115">Permissions</span></span>
<span data-ttu-id="d23ea-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d23ea-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d23ea-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="d23ea-118">Permission type</span></span>      | <span data-ttu-id="d23ea-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d23ea-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d23ea-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d23ea-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d23ea-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23ea-121">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d23ea-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d23ea-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d23ea-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d23ea-123">Not supported.</span></span>    |
|<span data-ttu-id="d23ea-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="d23ea-124">Application</span></span> | <span data-ttu-id="d23ea-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23ea-125">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d23ea-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d23ea-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="d23ea-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="d23ea-127">Request headers</span></span>
| <span data-ttu-id="d23ea-128">名称</span><span class="sxs-lookup"><span data-stu-id="d23ea-128">Name</span></span>       | <span data-ttu-id="d23ea-129">类型</span><span class="sxs-lookup"><span data-stu-id="d23ea-129">Type</span></span> | <span data-ttu-id="d23ea-130">说明</span><span class="sxs-lookup"><span data-stu-id="d23ea-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d23ea-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d23ea-131">Authorization</span></span>  | <span data-ttu-id="d23ea-132">string</span><span class="sxs-lookup"><span data-stu-id="d23ea-132">string</span></span>  | <span data-ttu-id="d23ea-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d23ea-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d23ea-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="d23ea-135">Request body</span></span>
<span data-ttu-id="d23ea-136">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="d23ea-137">属性</span><span class="sxs-lookup"><span data-stu-id="d23ea-137">Property</span></span> | <span data-ttu-id="d23ea-138">类型</span><span class="sxs-lookup"><span data-stu-id="d23ea-138">Type</span></span> | <span data-ttu-id="d23ea-139">说明</span><span class="sxs-lookup"><span data-stu-id="d23ea-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d23ea-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d23ea-140">displayName</span></span> | <span data-ttu-id="d23ea-141">string</span><span class="sxs-lookup"><span data-stu-id="d23ea-141">string</span></span> | <span data-ttu-id="d23ea-142">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d23ea-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="d23ea-143">必需。</span><span class="sxs-lookup"><span data-stu-id="d23ea-143">Required.</span></span> |
| <span data-ttu-id="d23ea-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d23ea-144">mailEnabled</span></span> | <span data-ttu-id="d23ea-145">布尔</span><span class="sxs-lookup"><span data-stu-id="d23ea-145">boolean</span></span> | <span data-ttu-id="d23ea-146">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="d23ea-147">如果创建 Office 365 组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-147">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="d23ea-148">如果创建动态或安全组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-148">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="d23ea-149">必需。</span><span class="sxs-lookup"><span data-stu-id="d23ea-149">Required.</span></span> |
| <span data-ttu-id="d23ea-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d23ea-150">mailNickname</span></span> | <span data-ttu-id="d23ea-151">string</span><span class="sxs-lookup"><span data-stu-id="d23ea-151">string</span></span> | <span data-ttu-id="d23ea-152">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="d23ea-152">The mail alias for the group.</span></span> <span data-ttu-id="d23ea-153">必需。</span><span class="sxs-lookup"><span data-stu-id="d23ea-153">Required.</span></span> |
| <span data-ttu-id="d23ea-154">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d23ea-154">securityEnabled</span></span> | <span data-ttu-id="d23ea-155">布尔</span><span class="sxs-lookup"><span data-stu-id="d23ea-155">boolean</span></span> | <span data-ttu-id="d23ea-156">对于启用安全机制的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-156">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="d23ea-157">如果创建动态或安全组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-157">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="d23ea-158">如果创建 Office 365 组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="d23ea-158">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="d23ea-159">必需。</span><span class="sxs-lookup"><span data-stu-id="d23ea-159">Required.</span></span> |
| <span data-ttu-id="d23ea-160">owners</span><span class="sxs-lookup"><span data-stu-id="d23ea-160">owners</span></span> | <span data-ttu-id="d23ea-161">string collection</span><span class="sxs-lookup"><span data-stu-id="d23ea-161">string collection</span></span> | <span data-ttu-id="d23ea-162">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="d23ea-162">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="d23ea-163">可选。</span><span class="sxs-lookup"><span data-stu-id="d23ea-163">Optional.</span></span> |
| <span data-ttu-id="d23ea-164">members</span><span class="sxs-lookup"><span data-stu-id="d23ea-164">members</span></span> | <span data-ttu-id="d23ea-165">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d23ea-165">string collection</span></span> | <span data-ttu-id="d23ea-166">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="d23ea-166">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="d23ea-167">可选。</span><span class="sxs-lookup"><span data-stu-id="d23ea-167">Optional.</span></span> |

<span data-ttu-id="d23ea-168">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-168">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="d23ea-169">组类型</span><span class="sxs-lookup"><span data-stu-id="d23ea-169">Type of group</span></span> | <span data-ttu-id="d23ea-170">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="d23ea-170">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="d23ea-171">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="d23ea-171">Office 365 (aka unified group)</span></span>| <span data-ttu-id="d23ea-172">"Unified"</span><span class="sxs-lookup"><span data-stu-id="d23ea-172">"Unified"</span></span> |
| <span data-ttu-id="d23ea-173">Dynamic</span><span class="sxs-lookup"><span data-stu-id="d23ea-173">Dynamic</span></span> | <span data-ttu-id="d23ea-174">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="d23ea-174">"DynamicMembership"</span></span> |
| <span data-ttu-id="d23ea-175">安全性</span><span class="sxs-lookup"><span data-stu-id="d23ea-175">Security</span></span> | <span data-ttu-id="d23ea-176">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="d23ea-176">Do not set.</span></span> |

<span data-ttu-id="d23ea-177">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `POST` 操作，并在创建组时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-177">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="d23ea-178">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="d23ea-178">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="d23ea-179">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="d23ea-179">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="d23ea-p114">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="d23ea-182">响应</span><span class="sxs-lookup"><span data-stu-id="d23ea-182">Response</span></span>
<span data-ttu-id="d23ea-183">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d23ea-183">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="d23ea-184">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-184">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="d23ea-185">示例</span><span class="sxs-lookup"><span data-stu-id="d23ea-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="d23ea-186">请求 1</span><span class="sxs-lookup"><span data-stu-id="d23ea-186">Request 1</span></span>
<span data-ttu-id="d23ea-187">第一个示例请求将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d23ea-187">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d23ea-188">响应</span><span class="sxs-lookup"><span data-stu-id="d23ea-188">Response</span></span>
<span data-ttu-id="d23ea-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d23ea-189">The following is an example of the response.</span></span>
><span data-ttu-id="d23ea-190">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d23ea-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d23ea-191">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-191">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="d23ea-192">请求 2</span><span class="sxs-lookup"><span data-stu-id="d23ea-192">Request 2</span></span>
<span data-ttu-id="d23ea-193">第二个示例请求将创建具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d23ea-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
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

#### <a name="response-2"></a><span data-ttu-id="d23ea-194">响应 2</span><span class="sxs-lookup"><span data-stu-id="d23ea-194">Response 2</span></span>
<span data-ttu-id="d23ea-195">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="d23ea-195">The following is an example of a successful response.</span></span> <span data-ttu-id="d23ea-196">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-196">It includes only default properties.</span></span> <span data-ttu-id="d23ea-197">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="d23ea-197">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="d23ea-198">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d23ea-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d23ea-199">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="d23ea-199">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
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

## <a name="see-also"></a><span data-ttu-id="d23ea-200">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d23ea-200">See also</span></span>

- [<span data-ttu-id="d23ea-201">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d23ea-201">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d23ea-202">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="d23ea-202">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d23ea-203">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="d23ea-203">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
