---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
ms.openlocfilehash: 2fff86d3bc86a8e78c295b1a4553006ac416ddd1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322958"
---
# <a name="create-group"></a><span data-ttu-id="582d6-104">创建组</span><span class="sxs-lookup"><span data-stu-id="582d6-104">Create group</span></span>
<span data-ttu-id="582d6-p102">使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="582d6-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="582d6-107">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="582d6-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="582d6-108">动态组</span><span class="sxs-lookup"><span data-stu-id="582d6-108">Dynamic group</span></span>
* <span data-ttu-id="582d6-109">安全组</span><span class="sxs-lookup"><span data-stu-id="582d6-109">Security group</span></span>

> <span data-ttu-id="582d6-p103">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="582d6-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="582d6-112">权限</span><span class="sxs-lookup"><span data-stu-id="582d6-112">Permissions</span></span>
<span data-ttu-id="582d6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="582d6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="582d6-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="582d6-115">Permission type</span></span>      | <span data-ttu-id="582d6-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="582d6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="582d6-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="582d6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="582d6-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="582d6-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="582d6-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="582d6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="582d6-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="582d6-120">Not supported.</span></span>    |
|<span data-ttu-id="582d6-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="582d6-121">Application</span></span> | <span data-ttu-id="582d6-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="582d6-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="582d6-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="582d6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="582d6-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="582d6-124">Request headers</span></span>
| <span data-ttu-id="582d6-125">Name</span><span class="sxs-lookup"><span data-stu-id="582d6-125">Name</span></span>       | <span data-ttu-id="582d6-126">类型</span><span class="sxs-lookup"><span data-stu-id="582d6-126">Type</span></span> | <span data-ttu-id="582d6-127">说明</span><span class="sxs-lookup"><span data-stu-id="582d6-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="582d6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="582d6-128">Authorization</span></span>  | <span data-ttu-id="582d6-129">string</span><span class="sxs-lookup"><span data-stu-id="582d6-129">string</span></span>  | <span data-ttu-id="582d6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="582d6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="582d6-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="582d6-132">Request body</span></span>
<span data-ttu-id="582d6-133">下表显示[组](../resources/group.md)资源时创建一组指定的属性。</span><span class="sxs-lookup"><span data-stu-id="582d6-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="582d6-134">属性</span><span class="sxs-lookup"><span data-stu-id="582d6-134">Property</span></span> | <span data-ttu-id="582d6-135">类型</span><span class="sxs-lookup"><span data-stu-id="582d6-135">Type</span></span> | <span data-ttu-id="582d6-136">说明</span><span class="sxs-lookup"><span data-stu-id="582d6-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="582d6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="582d6-137">displayName</span></span> | <span data-ttu-id="582d6-138">string</span><span class="sxs-lookup"><span data-stu-id="582d6-138">string</span></span> | <span data-ttu-id="582d6-139">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="582d6-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="582d6-140">必需。</span><span class="sxs-lookup"><span data-stu-id="582d6-140">Required.</span></span> |
| <span data-ttu-id="582d6-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="582d6-141">mailEnabled</span></span> | <span data-ttu-id="582d6-142">布尔</span><span class="sxs-lookup"><span data-stu-id="582d6-142">boolean</span></span> | <span data-ttu-id="582d6-143">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="582d6-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="582d6-144">此设置为**true**如果创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="582d6-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="582d6-145">此设置为**false**如果创建动态或安全组。</span><span class="sxs-lookup"><span data-stu-id="582d6-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="582d6-146">必需。</span><span class="sxs-lookup"><span data-stu-id="582d6-146">Required.</span></span> |
| <span data-ttu-id="582d6-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="582d6-147">mailNickname</span></span> | <span data-ttu-id="582d6-148">string</span><span class="sxs-lookup"><span data-stu-id="582d6-148">string</span></span> | <span data-ttu-id="582d6-149">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="582d6-149">The mail alias for the group.</span></span> <span data-ttu-id="582d6-150">必需。</span><span class="sxs-lookup"><span data-stu-id="582d6-150">Required.</span></span> |
| <span data-ttu-id="582d6-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="582d6-151">securityEnabled</span></span> | <span data-ttu-id="582d6-152">boolean</span><span class="sxs-lookup"><span data-stu-id="582d6-152">boolean</span></span> | <span data-ttu-id="582d6-153">设置为**true**已启用安全的组。</span><span class="sxs-lookup"><span data-stu-id="582d6-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="582d6-154">此设置为**true**如果创建动态或安全组。</span><span class="sxs-lookup"><span data-stu-id="582d6-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="582d6-155">此设置为**false**如果创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="582d6-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="582d6-156">必需。</span><span class="sxs-lookup"><span data-stu-id="582d6-156">Required.</span></span> |
| <span data-ttu-id="582d6-157">owners</span><span class="sxs-lookup"><span data-stu-id="582d6-157">owners</span></span> | <span data-ttu-id="582d6-158">string collection</span><span class="sxs-lookup"><span data-stu-id="582d6-158">string collection</span></span> | <span data-ttu-id="582d6-159">在创建时，此属性表示所有者组。</span><span class="sxs-lookup"><span data-stu-id="582d6-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="582d6-160">可选。</span><span class="sxs-lookup"><span data-stu-id="582d6-160">Optional.</span></span> |
| <span data-ttu-id="582d6-161">members</span><span class="sxs-lookup"><span data-stu-id="582d6-161">members</span></span> | <span data-ttu-id="582d6-162">string collection</span><span class="sxs-lookup"><span data-stu-id="582d6-162">string collection</span></span> | <span data-ttu-id="582d6-163">在创建时，此属性表示组的成员。</span><span class="sxs-lookup"><span data-stu-id="582d6-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="582d6-164">可选。</span><span class="sxs-lookup"><span data-stu-id="582d6-164">Optional.</span></span> |


<span data-ttu-id="582d6-165">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="582d6-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="582d6-166">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="582d6-166">groupTypes options</span></span>

| <span data-ttu-id="582d6-167">组类型</span><span class="sxs-lookup"><span data-stu-id="582d6-167">Type of group</span></span> | <span data-ttu-id="582d6-168">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="582d6-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="582d6-169">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="582d6-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="582d6-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="582d6-170">"Unified"</span></span> |
| <span data-ttu-id="582d6-171">Dynamic</span><span class="sxs-lookup"><span data-stu-id="582d6-171">Dynamic</span></span> | <span data-ttu-id="582d6-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="582d6-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="582d6-173">安全性</span><span class="sxs-lookup"><span data-stu-id="582d6-173">Security</span></span> | <span data-ttu-id="582d6-174">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="582d6-174">Do not set.</span></span> |


><span data-ttu-id="582d6-175">**注意：** 创建 Office 365 组以编程方式不用户上下文，也不指定所有者将匿名创建组。</span><span class="sxs-lookup"><span data-stu-id="582d6-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="582d6-176">这样做可能会导致正在才可以创建自动采取进一步的手动操作关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="582d6-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="582d6-p113">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="582d6-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="582d6-179">响应</span><span class="sxs-lookup"><span data-stu-id="582d6-179">Response</span></span>
<span data-ttu-id="582d6-180">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="582d6-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="582d6-181">示例</span><span class="sxs-lookup"><span data-stu-id="582d6-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="582d6-182">请求 1</span><span class="sxs-lookup"><span data-stu-id="582d6-182">Request 1</span></span>
<span data-ttu-id="582d6-183">第一个示例请求创建一个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="582d6-183">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="582d6-184">响应 1</span><span class="sxs-lookup"><span data-stu-id="582d6-184">Response 1</span></span>
<span data-ttu-id="582d6-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="582d6-185">The following is an example of the response.</span></span>
><span data-ttu-id="582d6-186">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="582d6-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="582d6-187">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="582d6-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="582d6-188">请求 2</span><span class="sxs-lookup"><span data-stu-id="582d6-188">Request 2</span></span>
<span data-ttu-id="582d6-189">第二个示例请求创建一个 Office 365 组指定的所有者。</span><span class="sxs-lookup"><span data-stu-id="582d6-189">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="582d6-190">响应 2</span><span class="sxs-lookup"><span data-stu-id="582d6-190">Response 2</span></span>
<span data-ttu-id="582d6-191">下面是响应的成功的示例。</span><span class="sxs-lookup"><span data-stu-id="582d6-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="582d6-192">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="582d6-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="582d6-193">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="582d6-193">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
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
