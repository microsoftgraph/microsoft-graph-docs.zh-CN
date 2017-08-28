# <a name="directoryrole-resource-type"></a><span data-ttu-id="91b58-101">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="91b58-101">directoryRole resource type</span></span>

<span data-ttu-id="91b58-p101">表示 Azure AD Directory 角色。Azure AD Directory 角色也称作*管理员角色*。有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用的目录角色，请发送具有此目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) ID 的 POST 请求。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="91b58-p101">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="91b58-110">方法</span><span class="sxs-lookup"><span data-stu-id="91b58-110">Methods</span></span>

| <span data-ttu-id="91b58-111">方法</span><span class="sxs-lookup"><span data-stu-id="91b58-111">Method</span></span>       | <span data-ttu-id="91b58-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="91b58-112">Return Type</span></span>  |<span data-ttu-id="91b58-113">说明</span><span class="sxs-lookup"><span data-stu-id="91b58-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91b58-114">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="91b58-114">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="91b58-115">directoryRole</span><span class="sxs-lookup"><span data-stu-id="91b58-115">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="91b58-116">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91b58-116">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="91b58-117">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="91b58-117">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="91b58-118">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91b58-118">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="91b58-119">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="91b58-119">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="91b58-120">添加成员</span><span class="sxs-lookup"><span data-stu-id="91b58-120">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="91b58-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="91b58-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="91b58-122">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="91b58-122">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="91b58-123">列出成员</span><span class="sxs-lookup"><span data-stu-id="91b58-123">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="91b58-124">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91b58-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="91b58-125">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="91b58-125">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="91b58-126">删除成员</span><span class="sxs-lookup"><span data-stu-id="91b58-126">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="91b58-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="91b58-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="91b58-128">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="91b58-128">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="91b58-129">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="91b58-129">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="91b58-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="91b58-130">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="91b58-131">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="91b58-131">Activate a directory role.</span></span>|

## <a name="properties"></a><span data-ttu-id="91b58-132">属性</span><span class="sxs-lookup"><span data-stu-id="91b58-132">Properties</span></span>
| <span data-ttu-id="91b58-133">属性</span><span class="sxs-lookup"><span data-stu-id="91b58-133">Property</span></span>   | <span data-ttu-id="91b58-134">类型</span><span class="sxs-lookup"><span data-stu-id="91b58-134">Type</span></span> | <span data-ttu-id="91b58-135">说明</span><span class="sxs-lookup"><span data-stu-id="91b58-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="91b58-136">说明</span><span class="sxs-lookup"><span data-stu-id="91b58-136">description</span></span>|<span data-ttu-id="91b58-137">String</span><span class="sxs-lookup"><span data-stu-id="91b58-137">String</span></span>|<span data-ttu-id="91b58-p102">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="91b58-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="91b58-140">displayName</span><span class="sxs-lookup"><span data-stu-id="91b58-140">displayName</span></span>|<span data-ttu-id="91b58-141">String</span><span class="sxs-lookup"><span data-stu-id="91b58-141">String</span></span>|<span data-ttu-id="91b58-p103">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="91b58-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="91b58-144">id</span><span class="sxs-lookup"><span data-stu-id="91b58-144">id</span></span>|<span data-ttu-id="91b58-145">String</span><span class="sxs-lookup"><span data-stu-id="91b58-145">String</span></span>|<span data-ttu-id="91b58-p104">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="91b58-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="91b58-149">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="91b58-149">roleTemplateId</span></span>|<span data-ttu-id="91b58-150">String</span><span class="sxs-lookup"><span data-stu-id="91b58-150">String</span></span>| <span data-ttu-id="91b58-p105">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="91b58-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="91b58-154">关系</span><span class="sxs-lookup"><span data-stu-id="91b58-154">Relationships</span></span>
| <span data-ttu-id="91b58-155">关系</span><span class="sxs-lookup"><span data-stu-id="91b58-155">Relationship</span></span> | <span data-ttu-id="91b58-156">类型</span><span class="sxs-lookup"><span data-stu-id="91b58-156">Type</span></span> |<span data-ttu-id="91b58-157">说明</span><span class="sxs-lookup"><span data-stu-id="91b58-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91b58-158">成员</span><span class="sxs-lookup"><span data-stu-id="91b58-158">members</span></span>|<span data-ttu-id="91b58-159">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91b58-159">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="91b58-p106">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="91b58-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91b58-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91b58-164">JSON representation</span></span>

<span data-ttu-id="91b58-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91b58-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
