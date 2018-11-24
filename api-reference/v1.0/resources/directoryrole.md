# <a name="directoryrole-resource-type"></a><span data-ttu-id="6975d-101">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="6975d-101">directoryRole resource type</span></span>

<span data-ttu-id="6975d-102">表示 Azure AD 目录角色。</span><span class="sxs-lookup"><span data-stu-id="6975d-102">Represents an Azure AD directory role.</span></span> <span data-ttu-id="6975d-103">Azure AD 目录角色也称为是*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="6975d-103">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="6975d-104">有关目录 （管理员） 角色的详细信息，请参阅[Azure AD 中的分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。</span><span class="sxs-lookup"><span data-stu-id="6975d-104">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="6975d-105">使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="6975d-105">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="6975d-106">若要读取目录角色或更新其成员，它必须首先激活在租户中。</span><span class="sxs-lookup"><span data-stu-id="6975d-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="6975d-107">默认情况下已激活公司管理员的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6975d-107">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="6975d-108">若要激活其他可用的目录角色将发送一个 POST 请求[directoryRoleTemplate](directoryroletemplate.md)目录角色所基于的 id。</span><span class="sxs-lookup"><span data-stu-id="6975d-108">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="6975d-109">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="6975d-109">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="6975d-110">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="6975d-110">This resource supports:</span></span>

- <span data-ttu-id="6975d-111">通过提供 [delta](../api/directoryrole_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="6975d-111">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="6975d-112">方法</span><span class="sxs-lookup"><span data-stu-id="6975d-112">Methods</span></span>

| <span data-ttu-id="6975d-113">方法</span><span class="sxs-lookup"><span data-stu-id="6975d-113">Method</span></span>       | <span data-ttu-id="6975d-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="6975d-114">Return Type</span></span>  |<span data-ttu-id="6975d-115">说明</span><span class="sxs-lookup"><span data-stu-id="6975d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6975d-116">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="6975d-116">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="6975d-117">directoryRole</span><span class="sxs-lookup"><span data-stu-id="6975d-117">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="6975d-118">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6975d-118">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="6975d-119">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="6975d-119">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="6975d-120">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6975d-120">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="6975d-121">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6975d-121">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="6975d-122">添加成员</span><span class="sxs-lookup"><span data-stu-id="6975d-122">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="6975d-123">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6975d-123">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6975d-124">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="6975d-124">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="6975d-125">列出成员</span><span class="sxs-lookup"><span data-stu-id="6975d-125">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="6975d-126">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6975d-126">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6975d-127">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="6975d-127">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="6975d-128">删除成员</span><span class="sxs-lookup"><span data-stu-id="6975d-128">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="6975d-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6975d-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6975d-130">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="6975d-130">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="6975d-131">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="6975d-131">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="6975d-132">directoryRole</span><span class="sxs-lookup"><span data-stu-id="6975d-132">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="6975d-133">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="6975d-133">Activate a directory role.</span></span>|
|[<span data-ttu-id="6975d-134">delta</span><span class="sxs-lookup"><span data-stu-id="6975d-134">delta</span></span>](../api/directoryrole_delta.md)|<span data-ttu-id="6975d-135">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="6975d-135">directoryRole collection</span></span>| <span data-ttu-id="6975d-136">获得目录角色增量更改。</span><span class="sxs-lookup"><span data-stu-id="6975d-136">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="6975d-137">属性</span><span class="sxs-lookup"><span data-stu-id="6975d-137">Properties</span></span>
| <span data-ttu-id="6975d-138">属性</span><span class="sxs-lookup"><span data-stu-id="6975d-138">Property</span></span>   | <span data-ttu-id="6975d-139">类型</span><span class="sxs-lookup"><span data-stu-id="6975d-139">Type</span></span> | <span data-ttu-id="6975d-140">说明</span><span class="sxs-lookup"><span data-stu-id="6975d-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6975d-141">说明</span><span class="sxs-lookup"><span data-stu-id="6975d-141">description</span></span>|<span data-ttu-id="6975d-142">String</span><span class="sxs-lookup"><span data-stu-id="6975d-142">String</span></span>|<span data-ttu-id="6975d-p102">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="6975d-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6975d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6975d-145">displayName</span></span>|<span data-ttu-id="6975d-146">String</span><span class="sxs-lookup"><span data-stu-id="6975d-146">String</span></span>|<span data-ttu-id="6975d-p103">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="6975d-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6975d-149">id</span><span class="sxs-lookup"><span data-stu-id="6975d-149">id</span></span>|<span data-ttu-id="6975d-150">String</span><span class="sxs-lookup"><span data-stu-id="6975d-150">String</span></span>|<span data-ttu-id="6975d-p104">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="6975d-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="6975d-154">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6975d-154">roleTemplateId</span></span>|<span data-ttu-id="6975d-155">String</span><span class="sxs-lookup"><span data-stu-id="6975d-155">String</span></span>| <span data-ttu-id="6975d-p105">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="6975d-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6975d-159">关系</span><span class="sxs-lookup"><span data-stu-id="6975d-159">Relationships</span></span>
| <span data-ttu-id="6975d-160">关系</span><span class="sxs-lookup"><span data-stu-id="6975d-160">Relationship</span></span> | <span data-ttu-id="6975d-161">类型</span><span class="sxs-lookup"><span data-stu-id="6975d-161">Type</span></span> |<span data-ttu-id="6975d-162">说明</span><span class="sxs-lookup"><span data-stu-id="6975d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6975d-163">members</span><span class="sxs-lookup"><span data-stu-id="6975d-163">members</span></span>|<span data-ttu-id="6975d-164">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6975d-164">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="6975d-p106">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6975d-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6975d-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6975d-169">JSON representation</span></span>

<span data-ttu-id="6975d-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6975d-170">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
