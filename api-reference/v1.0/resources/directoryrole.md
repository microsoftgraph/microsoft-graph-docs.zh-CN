---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作 *管理员角色*。
localization_priority: Priority
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4ed98c9fef582d2299fb9ed63f2474b0a3903611
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118677"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="14388-104">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="14388-104">directoryRole resource type</span></span>

<span data-ttu-id="14388-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14388-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14388-p102">表示 Azure AD Directory 角色。Azure AD Directory 角色也称作 *管理员角色*。有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用的目录角色，请发送具有此目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) ID 的 POST 请求。[列出目录角色模板](../api/directoryroletemplate-list.md) 以获得所有其他可用的目录角色。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="14388-p102">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. [List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="14388-115">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="14388-115">This resource supports:</span></span>

- <span data-ttu-id="14388-116">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="14388-116">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="14388-117">方法</span><span class="sxs-lookup"><span data-stu-id="14388-117">Methods</span></span>

| <span data-ttu-id="14388-118">方法</span><span class="sxs-lookup"><span data-stu-id="14388-118">Method</span></span>       | <span data-ttu-id="14388-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="14388-119">Return Type</span></span>  |<span data-ttu-id="14388-120">说明</span><span class="sxs-lookup"><span data-stu-id="14388-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14388-121">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="14388-121">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="14388-122">directoryRole</span><span class="sxs-lookup"><span data-stu-id="14388-122">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="14388-123">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14388-123">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="14388-124">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="14388-124">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="14388-125">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14388-125">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="14388-126">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="14388-126">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="14388-127">添加成员</span><span class="sxs-lookup"><span data-stu-id="14388-127">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="14388-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="14388-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="14388-129">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="14388-129">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="14388-130">列出成员</span><span class="sxs-lookup"><span data-stu-id="14388-130">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="14388-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14388-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="14388-132">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="14388-132">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="14388-133">删除成员</span><span class="sxs-lookup"><span data-stu-id="14388-133">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="14388-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="14388-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="14388-135">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="14388-135">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="14388-136">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="14388-136">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="14388-137">directoryRole</span><span class="sxs-lookup"><span data-stu-id="14388-137">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="14388-138">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="14388-138">Activate a directory role.</span></span>|
|[<span data-ttu-id="14388-139">列出 scopedMembers</span><span class="sxs-lookup"><span data-stu-id="14388-139">List scopedMembers</span></span>](../api/directoryrole-list-scopedmembers.md) |<span data-ttu-id="14388-140">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14388-140">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="14388-141">通过 scopedRoleMembership 资源集合列出其作用域为 [管理单元](administrativeunit.md) 的此目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="14388-141">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="14388-142">delta</span><span class="sxs-lookup"><span data-stu-id="14388-142">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="14388-143">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="14388-143">directoryRole collection</span></span>| <span data-ttu-id="14388-144">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="14388-144">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="14388-145">属性</span><span class="sxs-lookup"><span data-stu-id="14388-145">Properties</span></span>
| <span data-ttu-id="14388-146">属性</span><span class="sxs-lookup"><span data-stu-id="14388-146">Property</span></span>   | <span data-ttu-id="14388-147">类型</span><span class="sxs-lookup"><span data-stu-id="14388-147">Type</span></span> | <span data-ttu-id="14388-148">说明</span><span class="sxs-lookup"><span data-stu-id="14388-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="14388-149">说明</span><span class="sxs-lookup"><span data-stu-id="14388-149">description</span></span>|<span data-ttu-id="14388-150">String</span><span class="sxs-lookup"><span data-stu-id="14388-150">String</span></span>|<span data-ttu-id="14388-p103">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="14388-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="14388-153">displayName</span><span class="sxs-lookup"><span data-stu-id="14388-153">displayName</span></span>|<span data-ttu-id="14388-154">String</span><span class="sxs-lookup"><span data-stu-id="14388-154">String</span></span>|<span data-ttu-id="14388-p104">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="14388-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="14388-157">id</span><span class="sxs-lookup"><span data-stu-id="14388-157">id</span></span>|<span data-ttu-id="14388-158">String</span><span class="sxs-lookup"><span data-stu-id="14388-158">String</span></span>|<span data-ttu-id="14388-p105">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="14388-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="14388-162">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="14388-162">roleTemplateId</span></span>|<span data-ttu-id="14388-163">String</span><span class="sxs-lookup"><span data-stu-id="14388-163">String</span></span>| <span data-ttu-id="14388-p106">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="14388-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="14388-167">关系</span><span class="sxs-lookup"><span data-stu-id="14388-167">Relationships</span></span>
| <span data-ttu-id="14388-168">关系</span><span class="sxs-lookup"><span data-stu-id="14388-168">Relationship</span></span> | <span data-ttu-id="14388-169">类型</span><span class="sxs-lookup"><span data-stu-id="14388-169">Type</span></span> |<span data-ttu-id="14388-170">说明</span><span class="sxs-lookup"><span data-stu-id="14388-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14388-171">成员</span><span class="sxs-lookup"><span data-stu-id="14388-171">members</span></span>|<span data-ttu-id="14388-172">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14388-172">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="14388-p107">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="14388-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="14388-177">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="14388-177">scopedMembers</span></span>|<span data-ttu-id="14388-178">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14388-178">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="14388-179">此目录角色的成员，其作用域为 [管理单元](administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="14388-179">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="14388-180">只读。</span><span class="sxs-lookup"><span data-stu-id="14388-180">Read-only.</span></span> <span data-ttu-id="14388-181">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="14388-181">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14388-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14388-182">JSON representation</span></span>

<span data-ttu-id="14388-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14388-183">Here is a JSON representation of the resource</span></span>

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
