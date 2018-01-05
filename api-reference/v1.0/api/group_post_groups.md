# <a name="create-group"></a><span data-ttu-id="87b4e-101">创建组</span><span class="sxs-lookup"><span data-stu-id="87b4e-101">Create group</span></span>
<span data-ttu-id="87b4e-p101">使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：</span><span class="sxs-lookup"><span data-stu-id="87b4e-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="87b4e-104">Office 365 组（统一组）</span><span class="sxs-lookup"><span data-stu-id="87b4e-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="87b4e-105">动态组</span><span class="sxs-lookup"><span data-stu-id="87b4e-105">Dynamic group</span></span>
* <span data-ttu-id="87b4e-106">安全组</span><span class="sxs-lookup"><span data-stu-id="87b4e-106">Security group</span></span>

> <span data-ttu-id="87b4e-p102">**注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="87b4e-109">权限</span><span class="sxs-lookup"><span data-stu-id="87b4e-109">Permissions</span></span>
<span data-ttu-id="87b4e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87b4e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="87b4e-112">Permission type</span></span>      | <span data-ttu-id="87b4e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87b4e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87b4e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87b4e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="87b4e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87b4e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87b4e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87b4e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87b4e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="87b4e-117">Not supported.</span></span>    |
|<span data-ttu-id="87b4e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="87b4e-118">Application</span></span> | <span data-ttu-id="87b4e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87b4e-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87b4e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87b4e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="87b4e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="87b4e-121">Request headers</span></span>
| <span data-ttu-id="87b4e-122">名称</span><span class="sxs-lookup"><span data-stu-id="87b4e-122">Name</span></span>       | <span data-ttu-id="87b4e-123">类型</span><span class="sxs-lookup"><span data-stu-id="87b4e-123">Type</span></span> | <span data-ttu-id="87b4e-124">说明</span><span class="sxs-lookup"><span data-stu-id="87b4e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87b4e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87b4e-125">Authorization</span></span>  | <span data-ttu-id="87b4e-126">string</span><span class="sxs-lookup"><span data-stu-id="87b4e-126">string</span></span>  | <span data-ttu-id="87b4e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87b4e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="87b4e-129">Request body</span></span>
<span data-ttu-id="87b4e-130">下表显示了创建组时至少必须指定的[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="87b4e-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="87b4e-131">属性</span><span class="sxs-lookup"><span data-stu-id="87b4e-131">Property</span></span> | <span data-ttu-id="87b4e-132">类型</span><span class="sxs-lookup"><span data-stu-id="87b4e-132">Type</span></span> | <span data-ttu-id="87b4e-133">说明</span><span class="sxs-lookup"><span data-stu-id="87b4e-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87b4e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="87b4e-134">displayName</span></span> | <span data-ttu-id="87b4e-135">string</span><span class="sxs-lookup"><span data-stu-id="87b4e-135">string</span></span> | <span data-ttu-id="87b4e-136">要在组的通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="87b4e-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="87b4e-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="87b4e-137">mailEnabled</span></span> | <span data-ttu-id="87b4e-138">布尔</span><span class="sxs-lookup"><span data-stu-id="87b4e-138">boolean</span></span> | <span data-ttu-id="87b4e-p105">对于已启用邮件的组，请设置为 **true**。如果创建 Office 365 组，则将此设置为 **true**。如果创建动态或安全组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="87b4e-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="87b4e-142">mailNickname</span></span> | <span data-ttu-id="87b4e-143">string</span><span class="sxs-lookup"><span data-stu-id="87b4e-143">string</span></span> | <span data-ttu-id="87b4e-144">组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="87b4e-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="87b4e-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="87b4e-145">securityEnabled</span></span> | <span data-ttu-id="87b4e-146">布尔</span><span class="sxs-lookup"><span data-stu-id="87b4e-146">boolean</span></span> | <span data-ttu-id="87b4e-p106">对于启用安全机制的组，请设置为 **true**。如果创建动态或安全组，则将此设置为 **true**。如果创建 Office 365 组，则将此设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="87b4e-150">如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。</span><span class="sxs-lookup"><span data-stu-id="87b4e-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="87b4e-151">组类型</span><span class="sxs-lookup"><span data-stu-id="87b4e-151">Type of group</span></span> | <span data-ttu-id="87b4e-152">**groupTypes** 属性</span><span class="sxs-lookup"><span data-stu-id="87b4e-152">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="87b4e-153">Office 365（也称为统一组）</span><span class="sxs-lookup"><span data-stu-id="87b4e-153">Office 365 (aka unified group)</span></span>| <span data-ttu-id="87b4e-154">"Unified"</span><span class="sxs-lookup"><span data-stu-id="87b4e-154">"Unified"</span></span> |
| <span data-ttu-id="87b4e-155">Dynamic</span><span class="sxs-lookup"><span data-stu-id="87b4e-155">Dynamic</span></span> | <span data-ttu-id="87b4e-156">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="87b4e-156">"DynamicMembership"</span></span> |
| <span data-ttu-id="87b4e-157">安全性</span><span class="sxs-lookup"><span data-stu-id="87b4e-157">Security</span></span> | <span data-ttu-id="87b4e-158">请勿设置。</span><span class="sxs-lookup"><span data-stu-id="87b4e-158">Do not set.</span></span> |

<span data-ttu-id="87b4e-p107">根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。</span><span class="sxs-lookup"><span data-stu-id="87b4e-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="87b4e-161">响应</span><span class="sxs-lookup"><span data-stu-id="87b4e-161">Response</span></span>
<span data-ttu-id="87b4e-162">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87b4e-162">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87b4e-163">示例</span><span class="sxs-lookup"><span data-stu-id="87b4e-163">Example</span></span>
#### <a name="request"></a><span data-ttu-id="87b4e-164">请求</span><span class="sxs-lookup"><span data-stu-id="87b4e-164">Request</span></span>
<span data-ttu-id="87b4e-165">下面的示例展示了如何请求创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="87b4e-165">Here is an example of a request that creates an Office 365 group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
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

#### <a name="response"></a><span data-ttu-id="87b4e-166">响应</span><span class="sxs-lookup"><span data-stu-id="87b4e-166">Response</span></span>
<span data-ttu-id="87b4e-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="87b4e-167">Here is an example of the response.</span></span>
><span data-ttu-id="87b4e-168">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="87b4e-168">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="87b4e-169">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87b4e-169">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
