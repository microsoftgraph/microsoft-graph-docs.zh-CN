# <a name="create-group"></a><span data-ttu-id="6897e-101">创建组</span><span class="sxs-lookup"><span data-stu-id="6897e-101">Create group</span></span>
<span data-ttu-id="6897e-p101">使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="6897e-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="6897e-104">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="6897e-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="6897e-105">动态组</span><span class="sxs-lookup"><span data-stu-id="6897e-105">Dynamic group</span></span>
* <span data-ttu-id="6897e-106">安全组</span><span class="sxs-lookup"><span data-stu-id="6897e-106">Security group</span></span>

> <span data-ttu-id="6897e-p102">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="6897e-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="6897e-109">权限</span><span class="sxs-lookup"><span data-stu-id="6897e-109">Permissions</span></span>
<span data-ttu-id="6897e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6897e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6897e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6897e-112">Permission type</span></span>      | <span data-ttu-id="6897e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6897e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6897e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6897e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6897e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6897e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6897e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6897e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6897e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6897e-117">Not supported.</span></span>    |
|<span data-ttu-id="6897e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6897e-118">Application</span></span> | <span data-ttu-id="6897e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6897e-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6897e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6897e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="6897e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6897e-121">Request headers</span></span>
| <span data-ttu-id="6897e-122">名称</span><span class="sxs-lookup"><span data-stu-id="6897e-122">Name</span></span>       | <span data-ttu-id="6897e-123">类型</span><span class="sxs-lookup"><span data-stu-id="6897e-123">Type</span></span> | <span data-ttu-id="6897e-124">说明</span><span class="sxs-lookup"><span data-stu-id="6897e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6897e-125">授权</span><span class="sxs-lookup"><span data-stu-id="6897e-125">Authorization</span></span>  | <span data-ttu-id="6897e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="6897e-126">string</span></span>  | <span data-ttu-id="6897e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6897e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6897e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6897e-129">Request body</span></span>
<span data-ttu-id="6897e-130">下表显示了创建组时必须指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6897e-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="6897e-131">属性</span><span class="sxs-lookup"><span data-stu-id="6897e-131">Property</span></span> | <span data-ttu-id="6897e-132">类型</span><span class="sxs-lookup"><span data-stu-id="6897e-132">Type</span></span> | <span data-ttu-id="6897e-133">说明</span><span class="sxs-lookup"><span data-stu-id="6897e-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6897e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6897e-134">displayName</span></span> | <span data-ttu-id="6897e-135">字符串</span><span class="sxs-lookup"><span data-stu-id="6897e-135">string</span></span> | <span data-ttu-id="6897e-136">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="6897e-136">The name to display in the address book for the group.</span></span> <span data-ttu-id="6897e-137">必需。</span><span class="sxs-lookup"><span data-stu-id="6897e-137">Required.</span></span> |
| <span data-ttu-id="6897e-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="6897e-138">mailEnabled</span></span> | <span data-ttu-id="6897e-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="6897e-139">boolean</span></span> | <span data-ttu-id="6897e-140">对于已启用邮件的组，请设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6897e-140">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="6897e-141">如果创建的是 Office 365 组，此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6897e-141">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="6897e-142">如果创建动态或安全组，此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6897e-142">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="6897e-143">必需。</span><span class="sxs-lookup"><span data-stu-id="6897e-143">Required.</span></span> |
| <span data-ttu-id="6897e-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6897e-144">mailNickname</span></span> | <span data-ttu-id="6897e-145">字符串</span><span class="sxs-lookup"><span data-stu-id="6897e-145">string</span></span> | <span data-ttu-id="6897e-146">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="6897e-146">The mail alias for the group.</span></span> <span data-ttu-id="6897e-147">必需。</span><span class="sxs-lookup"><span data-stu-id="6897e-147">Required.</span></span> |
| <span data-ttu-id="6897e-148">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="6897e-148">securityEnabled</span></span> | <span data-ttu-id="6897e-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="6897e-149">boolean</span></span> | <span data-ttu-id="6897e-150">对于已启用安全的组设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6897e-150">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="6897e-151">如果创建动态或安全组，此设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="6897e-151">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="6897e-152">如果创建的是 Office 365 组，此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="6897e-152">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="6897e-153">必需。</span><span class="sxs-lookup"><span data-stu-id="6897e-153">Required.</span></span> |
| <span data-ttu-id="6897e-154">owners</span><span class="sxs-lookup"><span data-stu-id="6897e-154">owners</span></span> | <span data-ttu-id="6897e-155">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6897e-155">string collection</span></span> | <span data-ttu-id="6897e-156">在创建时，此属性表示所有者组。</span><span class="sxs-lookup"><span data-stu-id="6897e-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="6897e-157">可选。</span><span class="sxs-lookup"><span data-stu-id="6897e-157">Optional.</span></span> |
| <span data-ttu-id="6897e-158">members</span><span class="sxs-lookup"><span data-stu-id="6897e-158">members</span></span> | <span data-ttu-id="6897e-159">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6897e-159">string collection</span></span> | <span data-ttu-id="6897e-160">在创建时，此属性表示组的成员。</span><span class="sxs-lookup"><span data-stu-id="6897e-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="6897e-161">可选。</span><span class="sxs-lookup"><span data-stu-id="6897e-161">Optional.</span></span> |


<span data-ttu-id="6897e-162">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="6897e-162">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="6897e-163">groupTypes 选项</span><span class="sxs-lookup"><span data-stu-id="6897e-163">groupTypes options</span></span>

| <span data-ttu-id="6897e-164">组类型</span><span class="sxs-lookup"><span data-stu-id="6897e-164">Type of group</span></span> | <span data-ttu-id="6897e-165">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="6897e-165">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="6897e-166">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="6897e-166">Office 365 (aka unified group)</span></span>| <span data-ttu-id="6897e-167">"Unified"</span><span class="sxs-lookup"><span data-stu-id="6897e-167">"Unified"</span></span> |
| <span data-ttu-id="6897e-168">动态</span><span class="sxs-lookup"><span data-stu-id="6897e-168">Dynamic</span></span> | <span data-ttu-id="6897e-169">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="6897e-169">"DynamicMembership"</span></span> |
| <span data-ttu-id="6897e-170">安全</span><span class="sxs-lookup"><span data-stu-id="6897e-170">Security</span></span> | <span data-ttu-id="6897e-171">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="6897e-171">Do not set.</span></span> |


><span data-ttu-id="6897e-172">**注意：** 在没有用户上下文，也不指定所有者的情况下以编程方式创建 Office 365 组将匿名地创建组。</span><span class="sxs-lookup"><span data-stu-id="6897e-172">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="6897e-173">这样做可能会导致无法自动创建关联的 SharePoint Online 网站，直至采取进一步的手动操作。</span><span class="sxs-lookup"><span data-stu-id="6897e-173">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="6897e-p112">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6897e-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="6897e-176">响应</span><span class="sxs-lookup"><span data-stu-id="6897e-176">Response</span></span>
<span data-ttu-id="6897e-177">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6897e-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6897e-178">示例</span><span class="sxs-lookup"><span data-stu-id="6897e-178">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="6897e-179">请求 1</span><span class="sxs-lookup"><span data-stu-id="6897e-179">Request 1</span></span>
<span data-ttu-id="6897e-180">第一个示例请求创建一个 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="6897e-180">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="6897e-181">响应 1</span><span class="sxs-lookup"><span data-stu-id="6897e-181">Response 1</span></span>
<span data-ttu-id="6897e-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6897e-182">The following is an example of the response.</span></span>
><span data-ttu-id="6897e-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6897e-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="6897e-185">请求 2</span><span class="sxs-lookup"><span data-stu-id="6897e-185">Request 2</span></span>
<span data-ttu-id="6897e-186">第二个示例请求创建一个 Office 365 组，并指定所有者。</span><span class="sxs-lookup"><span data-stu-id="6897e-186">The second example request creates an Office 365 Group with owners specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="6897e-187">响应 2</span><span class="sxs-lookup"><span data-stu-id="6897e-187">Response 2</span></span>
<span data-ttu-id="6897e-188">下面展示了成功的响应示例。</span><span class="sxs-lookup"><span data-stu-id="6897e-188">The following is an example of the response.</span></span>
><span data-ttu-id="6897e-p114">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6897e-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
