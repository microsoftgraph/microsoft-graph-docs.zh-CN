---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作*管理员角色*。 有关这些目录（管理员）角色的详细信息，请参阅“在 Azure AD 中分配管理员角色”。 使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下，仅激活公司管理员目录角色。 若要激活其他可用的目录角色，请发送具有此目录角色所基于的 directoryRoleTemplate ID 的 POST 请求。 继承自 directoryObject。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b3379bbbecd86612043dcc3cb8455f5c43ba9cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584045"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="be197-110">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="be197-110">directoryRole resource type</span></span>

<span data-ttu-id="be197-111">表示 Azure AD Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="be197-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="be197-112">Azure AD 目录角色也称作*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="be197-112">Activate directory roles in an Azure AD tenant and manage user memberships in directory roles. Directory roles are also known as administrator roles.</span></span> <span data-ttu-id="be197-113">有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)</span><span class="sxs-lookup"><span data-stu-id="be197-113">For more information about administrator roles, see [Assigning administrator roles in Azure Active Directory](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="be197-114">使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="be197-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="be197-115">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="be197-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="be197-116">默认情况下，仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="be197-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="be197-117">若要激活其他可用的目录角色，请发送具有此目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) ID 的 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="be197-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="be197-118">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="be197-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="be197-119">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="be197-119">This resource supports:</span></span>

- <span data-ttu-id="be197-120">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="be197-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="be197-121">方法</span><span class="sxs-lookup"><span data-stu-id="be197-121">Methods</span></span>

| <span data-ttu-id="be197-122">方法</span><span class="sxs-lookup"><span data-stu-id="be197-122">Method</span></span>       | <span data-ttu-id="be197-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="be197-123">Return Type</span></span>  |<span data-ttu-id="be197-124">说明</span><span class="sxs-lookup"><span data-stu-id="be197-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be197-125">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="be197-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="be197-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="be197-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="be197-127">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be197-127">Read properties and relationships of directoryRole object.</span></span> |
|<span data-ttu-id="be197-128">[列出 directoryRoles](../api/directoryrole-list.md)</span><span class="sxs-lookup"><span data-stu-id="be197-128">[](../api/directoryrole-list.md)List directoryRoles</span></span> | <span data-ttu-id="be197-129">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be197-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="be197-130">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="be197-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="be197-131">添加成员</span><span class="sxs-lookup"><span data-stu-id="be197-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="be197-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="be197-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="be197-133">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="be197-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="be197-134">列出成员</span><span class="sxs-lookup"><span data-stu-id="be197-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="be197-135">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be197-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="be197-136">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="be197-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="be197-137">删除成员</span><span class="sxs-lookup"><span data-stu-id="be197-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="be197-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="be197-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="be197-139">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="be197-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="be197-140">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="be197-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="be197-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="be197-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="be197-142">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="be197-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="be197-143">delta</span><span class="sxs-lookup"><span data-stu-id="be197-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="be197-144">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="be197-144">directoryRole collection</span></span>| <span data-ttu-id="be197-145">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="be197-145">Get incremental changes for directory objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="be197-146">属性</span><span class="sxs-lookup"><span data-stu-id="be197-146">Properties</span></span>
| <span data-ttu-id="be197-147">属性</span><span class="sxs-lookup"><span data-stu-id="be197-147">Property</span></span>   | <span data-ttu-id="be197-148">类型</span><span class="sxs-lookup"><span data-stu-id="be197-148">Type</span></span> | <span data-ttu-id="be197-149">说明</span><span class="sxs-lookup"><span data-stu-id="be197-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="be197-150">说明</span><span class="sxs-lookup"><span data-stu-id="be197-150">description</span></span>|<span data-ttu-id="be197-151">String</span><span class="sxs-lookup"><span data-stu-id="be197-151">String</span></span>|<span data-ttu-id="be197-p103">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="be197-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="be197-154">displayName</span><span class="sxs-lookup"><span data-stu-id="be197-154">displayName</span></span>|<span data-ttu-id="be197-155">String</span><span class="sxs-lookup"><span data-stu-id="be197-155">String</span></span>|<span data-ttu-id="be197-p104">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="be197-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="be197-158">id</span><span class="sxs-lookup"><span data-stu-id="be197-158">id</span></span>|<span data-ttu-id="be197-159">String</span><span class="sxs-lookup"><span data-stu-id="be197-159">String</span></span>|<span data-ttu-id="be197-p105">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="be197-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="be197-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="be197-163">roleTemplateId</span></span>|<span data-ttu-id="be197-164">String</span><span class="sxs-lookup"><span data-stu-id="be197-164">String</span></span>| <span data-ttu-id="be197-p106">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="be197-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="be197-168">关系</span><span class="sxs-lookup"><span data-stu-id="be197-168">Relationships</span></span>
| <span data-ttu-id="be197-169">关系</span><span class="sxs-lookup"><span data-stu-id="be197-169">Relationship</span></span> | <span data-ttu-id="be197-170">类型</span><span class="sxs-lookup"><span data-stu-id="be197-170">Type</span></span> |<span data-ttu-id="be197-171">说明</span><span class="sxs-lookup"><span data-stu-id="be197-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be197-172">成员</span><span class="sxs-lookup"><span data-stu-id="be197-172">members</span></span>|<span data-ttu-id="be197-173">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be197-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="be197-p107">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="be197-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be197-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be197-178">JSON representation</span></span>

<span data-ttu-id="be197-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be197-179">Here is a JSON representation of the resource</span></span>

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
