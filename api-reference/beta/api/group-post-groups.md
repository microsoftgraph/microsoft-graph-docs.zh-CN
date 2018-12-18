---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
ms.openlocfilehash: 1c77b3a33b19e9f0254642ef89e3d7fddc224b9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320767"
---
# <a name="create-group"></a><span data-ttu-id="5d7dc-104">创建组</span><span class="sxs-lookup"><span data-stu-id="5d7dc-104">Create group</span></span>

> <span data-ttu-id="5d7dc-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d7dc-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5d7dc-107">使用此 API 创建在请求正文中指定一个新[组](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-107">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="5d7dc-108">您可以创建一个三种类型的组：</span><span class="sxs-lookup"><span data-stu-id="5d7dc-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="5d7dc-109">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="5d7dc-110">动态组</span><span class="sxs-lookup"><span data-stu-id="5d7dc-110">Dynamic group</span></span>
* <span data-ttu-id="5d7dc-111">安全组</span><span class="sxs-lookup"><span data-stu-id="5d7dc-111">Security group</span></span>

> <span data-ttu-id="5d7dc-112">**注意**： 若要创建[团队](../resources/team.md)，首先创建一个组，然后向其添加一个团队，请参阅[创建团队](../api/team-put-teams.md)。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d7dc-113">权限</span><span class="sxs-lookup"><span data-stu-id="5d7dc-113">Permissions</span></span>
<span data-ttu-id="5d7dc-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d7dc-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d7dc-116">Permission type</span></span>      | <span data-ttu-id="5d7dc-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d7dc-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5d7dc-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d7dc-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d7dc-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7dc-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-121">Not supported.</span></span>    |
|<span data-ttu-id="5d7dc-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d7dc-122">Application</span></span> | <span data-ttu-id="5d7dc-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d7dc-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d7dc-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d7dc-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="5d7dc-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d7dc-125">Request headers</span></span>
| <span data-ttu-id="5d7dc-126">Name</span><span class="sxs-lookup"><span data-stu-id="5d7dc-126">Name</span></span>       | <span data-ttu-id="5d7dc-127">类型</span><span class="sxs-lookup"><span data-stu-id="5d7dc-127">Type</span></span> | <span data-ttu-id="5d7dc-128">说明</span><span class="sxs-lookup"><span data-stu-id="5d7dc-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d7dc-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d7dc-129">Authorization</span></span>  | <span data-ttu-id="5d7dc-130">string</span><span class="sxs-lookup"><span data-stu-id="5d7dc-130">string</span></span>  | <span data-ttu-id="5d7dc-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d7dc-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d7dc-133">Request body</span></span>
<span data-ttu-id="5d7dc-134">下表显示[组](../resources/group.md)资源时创建一组指定的属性。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="5d7dc-135">属性</span><span class="sxs-lookup"><span data-stu-id="5d7dc-135">Property</span></span> | <span data-ttu-id="5d7dc-136">类型</span><span class="sxs-lookup"><span data-stu-id="5d7dc-136">Type</span></span> | <span data-ttu-id="5d7dc-137">说明</span><span class="sxs-lookup"><span data-stu-id="5d7dc-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d7dc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5d7dc-138">displayName</span></span> | <span data-ttu-id="5d7dc-139">string</span><span class="sxs-lookup"><span data-stu-id="5d7dc-139">string</span></span> | <span data-ttu-id="5d7dc-140">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="5d7dc-141">必需。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-141">Required.</span></span> |
| <span data-ttu-id="5d7dc-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="5d7dc-142">mailEnabled</span></span> | <span data-ttu-id="5d7dc-143">布尔</span><span class="sxs-lookup"><span data-stu-id="5d7dc-143">boolean</span></span> | <span data-ttu-id="5d7dc-144">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="5d7dc-145">此设置为**true**如果创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-145">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="5d7dc-146">此设置为**false**如果创建动态或安全组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-146">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="5d7dc-147">必需。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-147">Required.</span></span> |
| <span data-ttu-id="5d7dc-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5d7dc-148">mailNickname</span></span> | <span data-ttu-id="5d7dc-149">string</span><span class="sxs-lookup"><span data-stu-id="5d7dc-149">string</span></span> | <span data-ttu-id="5d7dc-150">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-150">The mail alias for the group.</span></span> <span data-ttu-id="5d7dc-151">必需。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-151">Required.</span></span> |
| <span data-ttu-id="5d7dc-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="5d7dc-152">securityEnabled</span></span> | <span data-ttu-id="5d7dc-153">boolean</span><span class="sxs-lookup"><span data-stu-id="5d7dc-153">boolean</span></span> | <span data-ttu-id="5d7dc-154">设置为**true**已启用安全的组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-154">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="5d7dc-155">此设置为**true**如果创建动态或安全组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-155">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="5d7dc-156">此设置为**false**如果创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-156">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="5d7dc-157">必需。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-157">Required.</span></span> |
| <span data-ttu-id="5d7dc-158">owners</span><span class="sxs-lookup"><span data-stu-id="5d7dc-158">owners</span></span> | <span data-ttu-id="5d7dc-159">string collection</span><span class="sxs-lookup"><span data-stu-id="5d7dc-159">string collection</span></span> | <span data-ttu-id="5d7dc-160">在创建时，此属性表示所有者组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-160">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="5d7dc-161">可选。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-161">Optional.</span></span> |
| <span data-ttu-id="5d7dc-162">members</span><span class="sxs-lookup"><span data-stu-id="5d7dc-162">members</span></span> | <span data-ttu-id="5d7dc-163">string collection</span><span class="sxs-lookup"><span data-stu-id="5d7dc-163">string collection</span></span> | <span data-ttu-id="5d7dc-164">在创建时，此属性表示组的成员。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-164">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="5d7dc-165">可选。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-165">Optional.</span></span> |

<span data-ttu-id="5d7dc-166">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-166">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="5d7dc-167">组类型</span><span class="sxs-lookup"><span data-stu-id="5d7dc-167">Type of group</span></span> | <span data-ttu-id="5d7dc-168">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="5d7dc-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="5d7dc-169">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="5d7dc-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="5d7dc-170">"Unified"</span></span> |
| <span data-ttu-id="5d7dc-171">Dynamic</span><span class="sxs-lookup"><span data-stu-id="5d7dc-171">Dynamic</span></span> | <span data-ttu-id="5d7dc-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="5d7dc-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="5d7dc-173">安全性</span><span class="sxs-lookup"><span data-stu-id="5d7dc-173">Security</span></span> | <span data-ttu-id="5d7dc-174">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-174">Do not set.</span></span> |

<span data-ttu-id="5d7dc-175">由于**group**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作和创建它时与您自己的数据的自定义属性添加到组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-175">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="5d7dc-176">**注意：** 创建 Office 365 组以编程方式不用户上下文，也不指定所有者将匿名创建组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-176">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="5d7dc-177">这样做可能会导致正在才可以创建自动采取进一步的手动操作关联的 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="5d7dc-p113">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="5d7dc-180">响应</span><span class="sxs-lookup"><span data-stu-id="5d7dc-180">Response</span></span>
<span data-ttu-id="5d7dc-181">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-181">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d7dc-182">示例</span><span class="sxs-lookup"><span data-stu-id="5d7dc-182">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="5d7dc-183">请求 1</span><span class="sxs-lookup"><span data-stu-id="5d7dc-183">Request 1</span></span>
<span data-ttu-id="5d7dc-184">第一个示例请求创建一个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-184">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a><span data-ttu-id="5d7dc-185">响应</span><span class="sxs-lookup"><span data-stu-id="5d7dc-185">Response</span></span>
<span data-ttu-id="5d7dc-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-186">The following is an example of the response.</span></span>
><span data-ttu-id="5d7dc-187">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d7dc-188">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-188">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="5d7dc-189">请求 2</span><span class="sxs-lookup"><span data-stu-id="5d7dc-189">Request 2</span></span>
<span data-ttu-id="5d7dc-190">第二个示例请求创建一个 Office 365 组指定的所有者。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-190">The second example request creates an Office 365 Group with owners specified.</span></span>
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

 #### <a name="response-2"></a><span data-ttu-id="5d7dc-191">响应 2</span><span class="sxs-lookup"><span data-stu-id="5d7dc-191">Response 2</span></span>
<span data-ttu-id="5d7dc-192">下面是响应的成功的示例。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-192">The following is an example of the successful response.</span></span>
><span data-ttu-id="5d7dc-p115">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5d7dc-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5d7dc-195">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5d7dc-195">See also</span></span>

- [<span data-ttu-id="5d7dc-196">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5d7dc-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5d7dc-197">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5d7dc-198">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5d7dc-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
