---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574864"
---
# <a name="create-group"></a><span data-ttu-id="231f8-104">创建组</span><span class="sxs-lookup"><span data-stu-id="231f8-104">Create group</span></span>
<span data-ttu-id="231f8-p102">使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="231f8-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="231f8-107">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="231f8-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="231f8-108">动态组</span><span class="sxs-lookup"><span data-stu-id="231f8-108">Dynamic group</span></span>
* <span data-ttu-id="231f8-109">安全组</span><span class="sxs-lookup"><span data-stu-id="231f8-109">Security group</span></span>

<span data-ttu-id="231f8-110">此操作在默认情况下仅返回每个组的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="231f8-111">这些默认属性将记录在[属性](../resources/group.md#properties)部分中。</span><span class="sxs-lookup"><span data-stu-id="231f8-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="231f8-112">若要获取_非_默认返回的属性，请执行 GET 操作，并在 `$select` OData 查询选项中指定属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="231f8-113">请参阅[示例](group-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="231f8-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="231f8-p105">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="231f8-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="231f8-116">权限</span><span class="sxs-lookup"><span data-stu-id="231f8-116">Permissions</span></span>
<span data-ttu-id="231f8-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="231f8-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="231f8-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="231f8-119">Permission type</span></span>      | <span data-ttu-id="231f8-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="231f8-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="231f8-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="231f8-121">Delegated (work or school account)</span></span> | <span data-ttu-id="231f8-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="231f8-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="231f8-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="231f8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="231f8-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="231f8-124">Not supported.</span></span>    |
|<span data-ttu-id="231f8-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="231f8-125">Application</span></span> | <span data-ttu-id="231f8-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="231f8-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="231f8-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="231f8-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="231f8-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="231f8-128">Request headers</span></span>
| <span data-ttu-id="231f8-129">名称</span><span class="sxs-lookup"><span data-stu-id="231f8-129">Name</span></span>       | <span data-ttu-id="231f8-130">类型</span><span class="sxs-lookup"><span data-stu-id="231f8-130">Type</span></span> | <span data-ttu-id="231f8-131">说明</span><span class="sxs-lookup"><span data-stu-id="231f8-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="231f8-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="231f8-132">Authorization</span></span>  | <span data-ttu-id="231f8-133">string</span><span class="sxs-lookup"><span data-stu-id="231f8-133">string</span></span>  | <span data-ttu-id="231f8-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="231f8-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="231f8-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="231f8-136">Content-Type</span></span>  | <span data-ttu-id="231f8-137">application/json</span><span class="sxs-lookup"><span data-stu-id="231f8-137">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="231f8-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="231f8-138">Request body</span></span>
<span data-ttu-id="231f8-139">下表显示了创建组时要指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-139">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="231f8-140">属性</span><span class="sxs-lookup"><span data-stu-id="231f8-140">Property</span></span> | <span data-ttu-id="231f8-141">类型</span><span class="sxs-lookup"><span data-stu-id="231f8-141">Type</span></span> | <span data-ttu-id="231f8-142">说明</span><span class="sxs-lookup"><span data-stu-id="231f8-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="231f8-143">displayName</span><span class="sxs-lookup"><span data-stu-id="231f8-143">displayName</span></span> | <span data-ttu-id="231f8-144">string</span><span class="sxs-lookup"><span data-stu-id="231f8-144">string</span></span> | <span data-ttu-id="231f8-145">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="231f8-145">The name to display in the address book for the group.</span></span> <span data-ttu-id="231f8-146">必需。</span><span class="sxs-lookup"><span data-stu-id="231f8-146">Required.</span></span> |
| <span data-ttu-id="231f8-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="231f8-147">mailEnabled</span></span> | <span data-ttu-id="231f8-148">布尔</span><span class="sxs-lookup"><span data-stu-id="231f8-148">boolean</span></span> | <span data-ttu-id="231f8-149">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="231f8-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="231f8-150">如果创建 Office 365 组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="231f8-150">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="231f8-151">如果创建动态或安全组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="231f8-151">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="231f8-152">必需。</span><span class="sxs-lookup"><span data-stu-id="231f8-152">Required.</span></span> |
| <span data-ttu-id="231f8-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="231f8-153">mailNickname</span></span> | <span data-ttu-id="231f8-154">string</span><span class="sxs-lookup"><span data-stu-id="231f8-154">string</span></span> | <span data-ttu-id="231f8-155">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="231f8-155">The mail alias for the group.</span></span> <span data-ttu-id="231f8-156">必需。</span><span class="sxs-lookup"><span data-stu-id="231f8-156">Required.</span></span> |
| <span data-ttu-id="231f8-157">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="231f8-157">securityEnabled</span></span> | <span data-ttu-id="231f8-158">布尔</span><span class="sxs-lookup"><span data-stu-id="231f8-158">boolean</span></span> | <span data-ttu-id="231f8-159">对于启用安全机制的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="231f8-159">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="231f8-160">如果创建动态或安全组，则将此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="231f8-160">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="231f8-161">如果创建 Office 365 组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="231f8-161">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="231f8-162">必需。</span><span class="sxs-lookup"><span data-stu-id="231f8-162">Required.</span></span> |
| <span data-ttu-id="231f8-163">owners</span><span class="sxs-lookup"><span data-stu-id="231f8-163">owners</span></span> | <span data-ttu-id="231f8-164">string collection</span><span class="sxs-lookup"><span data-stu-id="231f8-164">string collection</span></span> | <span data-ttu-id="231f8-165">此属性表示创建时指定的组所有者。</span><span class="sxs-lookup"><span data-stu-id="231f8-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="231f8-166">可选。</span><span class="sxs-lookup"><span data-stu-id="231f8-166">Optional.</span></span> |
| <span data-ttu-id="231f8-167">members</span><span class="sxs-lookup"><span data-stu-id="231f8-167">members</span></span> | <span data-ttu-id="231f8-168">字符串集合</span><span class="sxs-lookup"><span data-stu-id="231f8-168">string collection</span></span> | <span data-ttu-id="231f8-169">此属性表示创建时指定的组成员。</span><span class="sxs-lookup"><span data-stu-id="231f8-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="231f8-170">可选。</span><span class="sxs-lookup"><span data-stu-id="231f8-170">Optional.</span></span> |


<span data-ttu-id="231f8-171">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-171">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="231f8-172">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="231f8-172">groupTypes options</span></span>

| <span data-ttu-id="231f8-173">组类型</span><span class="sxs-lookup"><span data-stu-id="231f8-173">Type of group</span></span> | <span data-ttu-id="231f8-174">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="231f8-174">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="231f8-175">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="231f8-175">Office 365 (aka unified group)</span></span>| <span data-ttu-id="231f8-176">"Unified"</span><span class="sxs-lookup"><span data-stu-id="231f8-176">"Unified"</span></span> |
| <span data-ttu-id="231f8-177">Dynamic</span><span class="sxs-lookup"><span data-stu-id="231f8-177">Dynamic</span></span> | <span data-ttu-id="231f8-178">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="231f8-178">"DynamicMembership"</span></span> |
| <span data-ttu-id="231f8-179">安全性</span><span class="sxs-lookup"><span data-stu-id="231f8-179">Security</span></span> | <span data-ttu-id="231f8-180">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="231f8-180">Do not set.</span></span> |


><span data-ttu-id="231f8-181">**注意：** 以编程方式创建 Office 365 组时，若未提供用户上下文且未指定所有者，则将以匿名方式创建组。</span><span class="sxs-lookup"><span data-stu-id="231f8-181">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="231f8-182">这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="231f8-182">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="231f8-p115">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="231f8-185">响应</span><span class="sxs-lookup"><span data-stu-id="231f8-185">Response</span></span>
<span data-ttu-id="231f8-186">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="231f8-186">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="231f8-187">该响应仅包括组的默认属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-187">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="231f8-188">示例</span><span class="sxs-lookup"><span data-stu-id="231f8-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="231f8-189">请求 1</span><span class="sxs-lookup"><span data-stu-id="231f8-189">Request 1</span></span>
<span data-ttu-id="231f8-190">第一个示例请求将创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="231f8-190">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
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

#### <a name="response-1"></a><span data-ttu-id="231f8-191">响应 1</span><span class="sxs-lookup"><span data-stu-id="231f8-191">Response 1</span></span>
<span data-ttu-id="231f8-192">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="231f8-192">The following is an example of the response.</span></span>
><span data-ttu-id="231f8-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="231f8-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="231f8-194">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-194">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="231f8-195">请求 2</span><span class="sxs-lookup"><span data-stu-id="231f8-195">Request 2</span></span>
<span data-ttu-id="231f8-196">第二个示例请求将创建具有指定所有者和成员的 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="231f8-196">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
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

#### <a name="response-2"></a><span data-ttu-id="231f8-197">响应 2</span><span class="sxs-lookup"><span data-stu-id="231f8-197">Response 2</span></span>
<span data-ttu-id="231f8-198">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="231f8-198">The following is an example of a successful response.</span></span> <span data-ttu-id="231f8-199">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-199">It includes only default properties.</span></span> <span data-ttu-id="231f8-200">随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。</span><span class="sxs-lookup"><span data-stu-id="231f8-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="231f8-201">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="231f8-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="231f8-202">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="231f8-202">All the default properties are returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
