---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作*管理员角色*。 有关这些目录（管理员）角色的详细信息，请参阅“在 Azure AD 中分配管理员角色”。 使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下，仅激活公司管理员目录角色。 若要激活其他可用的目录角色, 请使用目录角色所基于的 directoryRoleTemplate 的 ID 发送 POST 请求。 继承自 directoryObject。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac9b08e2e39bce6a20703089d6bfe69c8b25f55f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657901"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="927da-110">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="927da-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="927da-111">表示 Azure AD Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="927da-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="927da-112">Azure AD 目录角色也称作*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="927da-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="927da-113">有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)</span><span class="sxs-lookup"><span data-stu-id="927da-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="927da-114">使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="927da-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="927da-115">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="927da-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="927da-116">默认情况下，仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="927da-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="927da-117">若要激活其他可用的目录角色, 请使用目录角色所基于的[directoryRoleTemplate](directoryroletemplate.md)的 ID 发送 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="927da-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="927da-118">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="927da-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="927da-119">默认情况下, 目录角色的作用域为 "租户范围"。</span><span class="sxs-lookup"><span data-stu-id="927da-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="927da-120">但是, 目录角色 (目前只有*用户帐户管理员*和*支持人员管理员*) 也可能作用于[管理单元](administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="927da-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="927da-121">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="927da-121">This resource supports:</span></span>

- <span data-ttu-id="927da-122">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="927da-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="927da-123">方法</span><span class="sxs-lookup"><span data-stu-id="927da-123">Methods</span></span>

| <span data-ttu-id="927da-124">方法</span><span class="sxs-lookup"><span data-stu-id="927da-124">Method</span></span>       | <span data-ttu-id="927da-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="927da-125">Return Type</span></span>  |<span data-ttu-id="927da-126">说明</span><span class="sxs-lookup"><span data-stu-id="927da-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="927da-127">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="927da-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="927da-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="927da-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="927da-129">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="927da-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="927da-130">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="927da-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="927da-131">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="927da-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="927da-132">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="927da-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="927da-133">添加成员</span><span class="sxs-lookup"><span data-stu-id="927da-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="927da-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="927da-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="927da-135">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="927da-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="927da-136">列出成员</span><span class="sxs-lookup"><span data-stu-id="927da-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="927da-137">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="927da-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="927da-138">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="927da-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="927da-139">删除成员</span><span class="sxs-lookup"><span data-stu-id="927da-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="927da-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="927da-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="927da-141">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="927da-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="927da-142">列出作用域内的角色成员</span><span class="sxs-lookup"><span data-stu-id="927da-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="927da-143">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="927da-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="927da-144">通过 scopedRoleMembership 资源集合列出此目录角色的范围限定为[管理单元](administrativeunit.md)的成员。</span><span class="sxs-lookup"><span data-stu-id="927da-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="927da-145">delta</span><span class="sxs-lookup"><span data-stu-id="927da-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="927da-146">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="927da-146">directoryRole collection</span></span>| <span data-ttu-id="927da-147">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="927da-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="927da-148">属性</span><span class="sxs-lookup"><span data-stu-id="927da-148">Properties</span></span>
| <span data-ttu-id="927da-149">属性</span><span class="sxs-lookup"><span data-stu-id="927da-149">Property</span></span>   | <span data-ttu-id="927da-150">类型</span><span class="sxs-lookup"><span data-stu-id="927da-150">Type</span></span> |<span data-ttu-id="927da-151">说明</span><span class="sxs-lookup"><span data-stu-id="927da-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="927da-152">说明</span><span class="sxs-lookup"><span data-stu-id="927da-152">description</span></span>|<span data-ttu-id="927da-153">字符串</span><span class="sxs-lookup"><span data-stu-id="927da-153">String</span></span>|<span data-ttu-id="927da-p104">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="927da-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="927da-156">displayName</span><span class="sxs-lookup"><span data-stu-id="927da-156">displayName</span></span>|<span data-ttu-id="927da-157">String</span><span class="sxs-lookup"><span data-stu-id="927da-157">String</span></span>|<span data-ttu-id="927da-p105">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="927da-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="927da-160">id</span><span class="sxs-lookup"><span data-stu-id="927da-160">id</span></span>|<span data-ttu-id="927da-161">字符串</span><span class="sxs-lookup"><span data-stu-id="927da-161">String</span></span>|<span data-ttu-id="927da-p106">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="927da-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="927da-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="927da-165">roleTemplateId</span></span>|<span data-ttu-id="927da-166">String</span><span class="sxs-lookup"><span data-stu-id="927da-166">String</span></span>| <span data-ttu-id="927da-p107">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="927da-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="927da-170">关系</span><span class="sxs-lookup"><span data-stu-id="927da-170">Relationships</span></span>
| <span data-ttu-id="927da-171">关系</span><span class="sxs-lookup"><span data-stu-id="927da-171">Relationship</span></span> | <span data-ttu-id="927da-172">类型</span><span class="sxs-lookup"><span data-stu-id="927da-172">Type</span></span> |<span data-ttu-id="927da-173">说明</span><span class="sxs-lookup"><span data-stu-id="927da-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="927da-174">成员</span><span class="sxs-lookup"><span data-stu-id="927da-174">members</span></span>|<span data-ttu-id="927da-175">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="927da-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="927da-p108">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="927da-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="927da-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="927da-180">scopedMembers</span></span>|<span data-ttu-id="927da-181">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="927da-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="927da-182">此目录角色的作用域为 "[管理单元](administrativeunit.md)" 的成员。</span><span class="sxs-lookup"><span data-stu-id="927da-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="927da-183">只读。</span><span class="sxs-lookup"><span data-stu-id="927da-183">Read-only.</span></span> <span data-ttu-id="927da-184">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="927da-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="927da-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="927da-185">JSON representation</span></span>

<span data-ttu-id="927da-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="927da-186">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
