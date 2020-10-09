---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作*管理员角色*。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bec9df52add7ab5a3c0440f3d7c7896d2920370a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402287"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="9f54b-104">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f54b-104">directoryRole resource type</span></span>

<span data-ttu-id="9f54b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f54b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f54b-106">表示 Azure AD Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="9f54b-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="9f54b-107">Azure AD 目录角色也称作*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="9f54b-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="9f54b-108">有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)</span><span class="sxs-lookup"><span data-stu-id="9f54b-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span> <span data-ttu-id="9f54b-109">使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="9f54b-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="9f54b-110">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="9f54b-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9f54b-111">默认情况下，仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="9f54b-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="9f54b-112">若要激活其他可用的目录角色，请使用目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 ID 发送 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="9f54b-112">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="9f54b-113">[列出目录角色模板](../api/directoryroletemplate-list.md)，以获取其他所有可用目录角色。</span><span class="sxs-lookup"><span data-stu-id="9f54b-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="9f54b-114">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="9f54b-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="9f54b-115">默认情况下，目录角色的作用域为 "租户范围"。</span><span class="sxs-lookup"><span data-stu-id="9f54b-115">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="9f54b-116">但是，当前仅 (*用户帐户管理员* 和 *支持人员管理员*) 的目录角色也可能作用域为 " [管理单元](administrativeunit.md)"。</span><span class="sxs-lookup"><span data-stu-id="9f54b-116">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="9f54b-117">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="9f54b-117">This resource supports:</span></span>

- <span data-ttu-id="9f54b-118">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="9f54b-118">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9f54b-119">方法</span><span class="sxs-lookup"><span data-stu-id="9f54b-119">Methods</span></span>

| <span data-ttu-id="9f54b-120">方法</span><span class="sxs-lookup"><span data-stu-id="9f54b-120">Method</span></span>       | <span data-ttu-id="9f54b-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f54b-121">Return Type</span></span>  |<span data-ttu-id="9f54b-122">说明</span><span class="sxs-lookup"><span data-stu-id="9f54b-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f54b-123">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="9f54b-123">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="9f54b-124">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9f54b-124">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="9f54b-125">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f54b-125">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="9f54b-126">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="9f54b-126">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="9f54b-127">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-127">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="9f54b-128">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="9f54b-128">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="9f54b-129">添加成员</span><span class="sxs-lookup"><span data-stu-id="9f54b-129">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="9f54b-130">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9f54b-130">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9f54b-131">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="9f54b-131">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9f54b-132">列出成员</span><span class="sxs-lookup"><span data-stu-id="9f54b-132">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9f54b-133">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-133">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9f54b-134">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="9f54b-134">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="9f54b-135">删除成员</span><span class="sxs-lookup"><span data-stu-id="9f54b-135">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="9f54b-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9f54b-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9f54b-137">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="9f54b-137">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="9f54b-138">列出作用域内的角色成员</span><span class="sxs-lookup"><span data-stu-id="9f54b-138">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9f54b-139">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-139">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9f54b-140">通过 scopedRoleMembership 资源集合列出此目录角色的范围限定为 [管理单元](administrativeunit.md)的成员。</span><span class="sxs-lookup"><span data-stu-id="9f54b-140">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="9f54b-141">delta</span><span class="sxs-lookup"><span data-stu-id="9f54b-141">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="9f54b-142">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-142">directoryRole collection</span></span>| <span data-ttu-id="9f54b-143">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="9f54b-143">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f54b-144">属性</span><span class="sxs-lookup"><span data-stu-id="9f54b-144">Properties</span></span>
| <span data-ttu-id="9f54b-145">属性</span><span class="sxs-lookup"><span data-stu-id="9f54b-145">Property</span></span>   | <span data-ttu-id="9f54b-146">类型</span><span class="sxs-lookup"><span data-stu-id="9f54b-146">Type</span></span> |<span data-ttu-id="9f54b-147">说明</span><span class="sxs-lookup"><span data-stu-id="9f54b-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f54b-148">说明</span><span class="sxs-lookup"><span data-stu-id="9f54b-148">description</span></span>|<span data-ttu-id="9f54b-149">String</span><span class="sxs-lookup"><span data-stu-id="9f54b-149">String</span></span>|<span data-ttu-id="9f54b-p104">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="9f54b-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9f54b-152">displayName</span><span class="sxs-lookup"><span data-stu-id="9f54b-152">displayName</span></span>|<span data-ttu-id="9f54b-153">String</span><span class="sxs-lookup"><span data-stu-id="9f54b-153">String</span></span>|<span data-ttu-id="9f54b-p105">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="9f54b-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9f54b-156">id</span><span class="sxs-lookup"><span data-stu-id="9f54b-156">id</span></span>|<span data-ttu-id="9f54b-157">String</span><span class="sxs-lookup"><span data-stu-id="9f54b-157">String</span></span>|<span data-ttu-id="9f54b-p106">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="9f54b-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9f54b-161">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9f54b-161">roleTemplateId</span></span>|<span data-ttu-id="9f54b-162">String</span><span class="sxs-lookup"><span data-stu-id="9f54b-162">String</span></span>| <span data-ttu-id="9f54b-p107">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="9f54b-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9f54b-166">关系</span><span class="sxs-lookup"><span data-stu-id="9f54b-166">Relationships</span></span>
| <span data-ttu-id="9f54b-167">关系</span><span class="sxs-lookup"><span data-stu-id="9f54b-167">Relationship</span></span> | <span data-ttu-id="9f54b-168">类型</span><span class="sxs-lookup"><span data-stu-id="9f54b-168">Type</span></span> |<span data-ttu-id="9f54b-169">说明</span><span class="sxs-lookup"><span data-stu-id="9f54b-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f54b-170">成员</span><span class="sxs-lookup"><span data-stu-id="9f54b-170">members</span></span>|<span data-ttu-id="9f54b-171">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-171">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="9f54b-p108">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9f54b-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9f54b-176">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="9f54b-176">scopedMembers</span></span>|<span data-ttu-id="9f54b-177">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f54b-177">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9f54b-178">此目录角色的作用域为 " [管理单元](administrativeunit.md)" 的成员。</span><span class="sxs-lookup"><span data-stu-id="9f54b-178">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="9f54b-179">只读。</span><span class="sxs-lookup"><span data-stu-id="9f54b-179">Read-only.</span></span> <span data-ttu-id="9f54b-180">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9f54b-180">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f54b-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f54b-181">JSON representation</span></span>

<span data-ttu-id="9f54b-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f54b-182">Here is a JSON representation of the resource</span></span>

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