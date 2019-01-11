---
title: directoryRole 资源类型
description: 表示 Azure AD 目录角色。 Azure AD 目录角色也称为是*管理员角色*。 有关目录 （管理员） 角色的详细信息，请参阅 Azure AD 中分配管理员角色。 使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下已激活公司管理员的目录角色。 若要激活发送一个 POST 请求 id 为基于目录角色 directoryRoleTemplate 其他可用的目录角色。 继承自 directoryObject。
localization_priority: Priority
ms.openlocfilehash: 05d897d6426b2feab7c08adaa125788590675f66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820865"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="529f7-110">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="529f7-110">directoryRole resource type</span></span>

<span data-ttu-id="529f7-111">表示 Azure AD 目录角色。</span><span class="sxs-lookup"><span data-stu-id="529f7-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="529f7-112">Azure AD 目录角色也称为是*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="529f7-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="529f7-113">有关目录 （管理员） 角色的详细信息，请参阅[Azure AD 中的分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。</span><span class="sxs-lookup"><span data-stu-id="529f7-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="529f7-114">使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="529f7-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="529f7-115">若要读取目录角色或更新其成员，它必须首先激活在租户中。</span><span class="sxs-lookup"><span data-stu-id="529f7-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="529f7-116">默认情况下已激活公司管理员的目录角色。</span><span class="sxs-lookup"><span data-stu-id="529f7-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="529f7-117">若要激活其他可用的目录角色将发送一个 POST 请求[directoryRoleTemplate](directoryroletemplate.md)目录角色所基于的 id。</span><span class="sxs-lookup"><span data-stu-id="529f7-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="529f7-118">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="529f7-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="529f7-119">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="529f7-119">This resource supports:</span></span>

- <span data-ttu-id="529f7-120">通过提供 [delta](../api/directoryrole-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="529f7-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="529f7-121">方法</span><span class="sxs-lookup"><span data-stu-id="529f7-121">Methods</span></span>

| <span data-ttu-id="529f7-122">方法</span><span class="sxs-lookup"><span data-stu-id="529f7-122">Method</span></span>       | <span data-ttu-id="529f7-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="529f7-123">Return Type</span></span>  |<span data-ttu-id="529f7-124">说明</span><span class="sxs-lookup"><span data-stu-id="529f7-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="529f7-125">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="529f7-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="529f7-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="529f7-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="529f7-127">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="529f7-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="529f7-128">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="529f7-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="529f7-129">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="529f7-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="529f7-130">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="529f7-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="529f7-131">添加成员</span><span class="sxs-lookup"><span data-stu-id="529f7-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="529f7-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="529f7-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="529f7-133">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="529f7-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="529f7-134">列出成员</span><span class="sxs-lookup"><span data-stu-id="529f7-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="529f7-135">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="529f7-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="529f7-136">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="529f7-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="529f7-137">删除成员</span><span class="sxs-lookup"><span data-stu-id="529f7-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="529f7-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="529f7-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="529f7-139">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="529f7-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="529f7-140">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="529f7-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="529f7-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="529f7-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="529f7-142">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="529f7-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="529f7-143">delta</span><span class="sxs-lookup"><span data-stu-id="529f7-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="529f7-144">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="529f7-144">directoryRole collection</span></span>| <span data-ttu-id="529f7-145">获得目录角色增量更改。</span><span class="sxs-lookup"><span data-stu-id="529f7-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="529f7-146">属性</span><span class="sxs-lookup"><span data-stu-id="529f7-146">Properties</span></span>
| <span data-ttu-id="529f7-147">属性</span><span class="sxs-lookup"><span data-stu-id="529f7-147">Property</span></span>   | <span data-ttu-id="529f7-148">类型</span><span class="sxs-lookup"><span data-stu-id="529f7-148">Type</span></span> | <span data-ttu-id="529f7-149">说明</span><span class="sxs-lookup"><span data-stu-id="529f7-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="529f7-150">说明</span><span class="sxs-lookup"><span data-stu-id="529f7-150">description</span></span>|<span data-ttu-id="529f7-151">String</span><span class="sxs-lookup"><span data-stu-id="529f7-151">String</span></span>|<span data-ttu-id="529f7-p103">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="529f7-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="529f7-154">displayName</span><span class="sxs-lookup"><span data-stu-id="529f7-154">displayName</span></span>|<span data-ttu-id="529f7-155">String</span><span class="sxs-lookup"><span data-stu-id="529f7-155">String</span></span>|<span data-ttu-id="529f7-p104">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="529f7-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="529f7-158">id</span><span class="sxs-lookup"><span data-stu-id="529f7-158">id</span></span>|<span data-ttu-id="529f7-159">String</span><span class="sxs-lookup"><span data-stu-id="529f7-159">String</span></span>|<span data-ttu-id="529f7-p105">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="529f7-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="529f7-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="529f7-163">roleTemplateId</span></span>|<span data-ttu-id="529f7-164">String</span><span class="sxs-lookup"><span data-stu-id="529f7-164">String</span></span>| <span data-ttu-id="529f7-p106">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="529f7-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="529f7-168">关系</span><span class="sxs-lookup"><span data-stu-id="529f7-168">Relationships</span></span>
| <span data-ttu-id="529f7-169">关系</span><span class="sxs-lookup"><span data-stu-id="529f7-169">Relationship</span></span> | <span data-ttu-id="529f7-170">类型</span><span class="sxs-lookup"><span data-stu-id="529f7-170">Type</span></span> |<span data-ttu-id="529f7-171">说明</span><span class="sxs-lookup"><span data-stu-id="529f7-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="529f7-172">members</span><span class="sxs-lookup"><span data-stu-id="529f7-172">members</span></span>|<span data-ttu-id="529f7-173">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="529f7-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="529f7-p107">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="529f7-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="529f7-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="529f7-178">JSON representation</span></span>

<span data-ttu-id="529f7-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="529f7-179">Here is a JSON representation of the resource</span></span>

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
