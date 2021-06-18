---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
localization_priority: Normal
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ed3559a0345c2ca1ca190d6ed08c1cec542837fe
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991167"
---
# <a name="administrativeunit-resource-type"></a><span data-ttu-id="65c21-103">administrativeUnit 资源类型</span><span class="sxs-lookup"><span data-stu-id="65c21-103">administrativeUnit resource type</span></span>

<span data-ttu-id="65c21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65c21-105">管理单元为用户和组目录对象提供概念容器。</span><span class="sxs-lookup"><span data-stu-id="65c21-105">An administrative unit provides a conceptual container for User and Group directory objects.</span></span> <span data-ttu-id="65c21-106">使用管理单元，公司管理员现在可以将管理职责委派给区域管理员或部门管理员，以管理管理单元中包含的用户和组或范围所包含的用户和组。</span><span class="sxs-lookup"><span data-stu-id="65c21-106">Using administrative units, a company administrator can now delegate administrative responsibilities to manage the users and groups contained within or scoped to an administrative unit to a regional or departmental administrator.</span></span>

<span data-ttu-id="65c21-107">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="65c21-107">Let's look at an example.</span></span> <span data-ttu-id="65c21-108">Imagine Contoso Corp 由两个部门（一个东海岸分部和一个东海岸部门）负责。</span><span class="sxs-lookup"><span data-stu-id="65c21-108">Imagine that Contoso Corp is made up of two divisions - a West Coast Division and an East Coast Division.</span></span> <span data-ttu-id="65c21-109">Contoso 的目录角色的范围为整个租户。</span><span class="sxs-lookup"><span data-stu-id="65c21-109">Directory roles at Contoso are scoped to the entire tenant.</span></span> <span data-ttu-id="65c21-110">Contoso 公司管理员 Lee 希望委派管理责任，但将其范围划分到东海岸部门或东海岸分部。</span><span class="sxs-lookup"><span data-stu-id="65c21-110">Lee, a Contoso company administrator, wants to delegate administrative responsibilities, but scope them to the West Coast Division or the East Coast division.</span></span>  <span data-ttu-id="65c21-111">Lee 可以创建 *一个"东海岸* "管理单元，并可以将所有"东海岸"用户放入此管理单元中。</span><span class="sxs-lookup"><span data-stu-id="65c21-111">Lee can create a *West Coast admistrative unit* and place all West Coast users into this administrative unit.</span></span>  <span data-ttu-id="65c21-112">同样，Lee 可以创建一 *个"东海岸管理单元"。*</span><span class="sxs-lookup"><span data-stu-id="65c21-112">Similarly, Lee can create an *East Coast adminstrative unit*.</span></span>  <span data-ttu-id="65c21-113">现在，Lee 可以开始将管理职责委派给其他人，但作用域为自己创建的新管理单元。</span><span class="sxs-lookup"><span data-stu-id="65c21-113">Now Lee, can start delegating administrative responsibilities to others, but **scoped** to the new administrative units he's created.</span></span> <span data-ttu-id="65c21-114">Lee 将 Jennifer 设置在一个支持 *人员管理员* 角色 **中** ，该角色的作用范围为 *"东海岸"管理单元*。</span><span class="sxs-lookup"><span data-stu-id="65c21-114">Lee places Jennifer in a *helpdesk administrator* role **scoped** to the *West Coast administrative unit*.</span></span>  <span data-ttu-id="65c21-115">这允许 Jennifer 重置任何用户的密码，但只有在这些用户位于 *东海岸管理单元时。*</span><span class="sxs-lookup"><span data-stu-id="65c21-115">This allows Jennifer to reset any user's password, but only if those users are in the *West Coast administrative unit*.</span></span>  <span data-ttu-id="65c21-116">同样，Lee 将 Dave 设置在 *一个用户帐户管理员* 角色中，该角色的作用范围为"*东海岸"管理单元*。 </span><span class="sxs-lookup"><span data-stu-id="65c21-116">Similarly, Lee places Dave in a *user account administrator* role **scoped** to the *East Coast administrative unit*.</span></span>  <span data-ttu-id="65c21-117">这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但只有在这些用户位于东海岸管理 *单元中时。*</span><span class="sxs-lookup"><span data-stu-id="65c21-117">This allows Dave to update users, assign licenses and reset any user's password, but only if those users are in the *East Coast administrative unit*.</span></span> <span data-ttu-id="65c21-118">有关视频概述，请参阅管理单元[Azure Active Directory简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。</span><span class="sxs-lookup"><span data-stu-id="65c21-118">For a video overview, please see [Introduction to Azure Active Directory Administrative Units](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).</span></span>


<span data-ttu-id="65c21-119">本主题提供 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。</span><span class="sxs-lookup"><span data-stu-id="65c21-119">This topic provides descriptions of the declared properties and navigation properties exposed by the administrativeUnit entity, as well as the operations and functions that can be called on the administrativeUnits resource.</span></span>


## <a name="methods"></a><span data-ttu-id="65c21-120">方法</span><span class="sxs-lookup"><span data-stu-id="65c21-120">Methods</span></span>

| <span data-ttu-id="65c21-121">方法</span><span class="sxs-lookup"><span data-stu-id="65c21-121">Method</span></span>   | <span data-ttu-id="65c21-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="65c21-122">Return Type</span></span> | <span data-ttu-id="65c21-123">说明</span><span class="sxs-lookup"><span data-stu-id="65c21-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="65c21-124">创建</span><span class="sxs-lookup"><span data-stu-id="65c21-124">Create</span></span>](../api/administrativeunit-post-administrativeunits.md) | [<span data-ttu-id="65c21-125">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="65c21-125">administrativeUnit</span></span>](administrativeunit.md) | <span data-ttu-id="65c21-126">创建新的管理单元。</span><span class="sxs-lookup"><span data-stu-id="65c21-126">Create a new administrative unit.</span></span>|
|[<span data-ttu-id="65c21-127">列表</span><span class="sxs-lookup"><span data-stu-id="65c21-127">List</span></span>](../api/administrativeunit-list.md) | <span data-ttu-id="65c21-128">[administrativeUnit](administrativeunit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c21-128">[administrativeUnit](administrativeunit.md) collection</span></span> |<span data-ttu-id="65c21-129">列出所有 administrativeUnits 的属性。</span><span class="sxs-lookup"><span data-stu-id="65c21-129">List properties of all administrativeUnits.</span></span>|
|[<span data-ttu-id="65c21-130">获取</span><span class="sxs-lookup"><span data-stu-id="65c21-130">Get</span></span>](../api/administrativeunit-get.md) | [<span data-ttu-id="65c21-131">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="65c21-131">administrativeUnit</span></span>](administrativeunit.md) |<span data-ttu-id="65c21-132">读取特定 administrativeUnit 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65c21-132">Read properties and relationships of a specific administrativeUnit object.</span></span>|
|[<span data-ttu-id="65c21-133">更新</span><span class="sxs-lookup"><span data-stu-id="65c21-133">Update</span></span>](../api/administrativeunit-update.md) | [<span data-ttu-id="65c21-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="65c21-134">administrativeUnit</span></span>](administrativeunit.md)    |<span data-ttu-id="65c21-135">更新 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="65c21-135">Update administrativeUnit object.</span></span> |
|[<span data-ttu-id="65c21-136">删除</span><span class="sxs-lookup"><span data-stu-id="65c21-136">Delete</span></span>](../api/administrativeunit-delete.md) | <span data-ttu-id="65c21-137">无</span><span class="sxs-lookup"><span data-stu-id="65c21-137">None</span></span> |<span data-ttu-id="65c21-138">删除 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="65c21-138">Delete administrativeUnit object.</span></span> |
|[<span data-ttu-id="65c21-139">添加成员</span><span class="sxs-lookup"><span data-stu-id="65c21-139">Add a member</span></span>](../api/administrativeunit-post-members.md) |[<span data-ttu-id="65c21-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="65c21-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="65c21-141">向用户 (组添加成员) 。</span><span class="sxs-lookup"><span data-stu-id="65c21-141">Add a member (user or group).</span></span>|
|[<span data-ttu-id="65c21-142">List members</span><span class="sxs-lookup"><span data-stu-id="65c21-142">List members</span></span>](../api/administrativeunit-list-members.md) |<span data-ttu-id="65c21-143">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c21-143">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="65c21-144">获取用户和 (组) 列表。</span><span class="sxs-lookup"><span data-stu-id="65c21-144">Get the list of (user and group) members.</span></span>|
|[<span data-ttu-id="65c21-145">获取成员</span><span class="sxs-lookup"><span data-stu-id="65c21-145">Get a member</span></span>](../api/administrativeunit-get-members.md) |[<span data-ttu-id="65c21-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="65c21-146">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="65c21-147">获取特定成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-147">Get a specific member.</span></span>|
|[<span data-ttu-id="65c21-148">删除成员</span><span class="sxs-lookup"><span data-stu-id="65c21-148">Remove a member</span></span>](../api/administrativeunit-delete-members.md) |[<span data-ttu-id="65c21-149">directoryObject</span><span class="sxs-lookup"><span data-stu-id="65c21-149">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="65c21-150">删除成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-150">Remove a member.</span></span>|
|[<span data-ttu-id="65c21-151">添加作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="65c21-151">Add scoped-role member</span></span>](../api/administrativeunit-post-scopedrolemembers.md) |[<span data-ttu-id="65c21-152">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="65c21-152">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="65c21-153">添加作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-153">Add a scoped-role member.</span></span>|
|[<span data-ttu-id="65c21-154">列出作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="65c21-154">List scoped-role members</span></span>](../api/administrativeunit-list-scopedrolemembers.md) |<span data-ttu-id="65c21-155">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c21-155">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="65c21-156">获取作用域角色管理员列表。</span><span class="sxs-lookup"><span data-stu-id="65c21-156">Get the list of scoped-role administrators.</span></span>|
|[<span data-ttu-id="65c21-157">获取作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="65c21-157">Get a scoped-role member</span></span>](../api/administrativeunit-get-scopedrolemembers.md) |[<span data-ttu-id="65c21-158">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="65c21-158">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="65c21-159">获取特定作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-159">Get a specific scoped-role member.</span></span>|
|[<span data-ttu-id="65c21-160">删除作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="65c21-160">Remove a scoped-role member</span></span>](../api/administrativeunit-delete-scopedrolemembers.md) |[<span data-ttu-id="65c21-161">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="65c21-161">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="65c21-162">删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-162">Remove a scoped-role member.</span></span>|

## <a name="properties"></a><span data-ttu-id="65c21-163">属性</span><span class="sxs-lookup"><span data-stu-id="65c21-163">Properties</span></span>
| <span data-ttu-id="65c21-164">属性</span><span class="sxs-lookup"><span data-stu-id="65c21-164">Property</span></span>     | <span data-ttu-id="65c21-165">类型</span><span class="sxs-lookup"><span data-stu-id="65c21-165">Type</span></span>   |<span data-ttu-id="65c21-166">说明</span><span class="sxs-lookup"><span data-stu-id="65c21-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65c21-167">说明</span><span class="sxs-lookup"><span data-stu-id="65c21-167">description</span></span>|<span data-ttu-id="65c21-168">string</span><span class="sxs-lookup"><span data-stu-id="65c21-168">string</span></span>|<span data-ttu-id="65c21-169">管理单元的可选说明。</span><span class="sxs-lookup"><span data-stu-id="65c21-169">An optional description for the administrative unit.</span></span>|
|<span data-ttu-id="65c21-170">displayName</span><span class="sxs-lookup"><span data-stu-id="65c21-170">displayName</span></span>|<span data-ttu-id="65c21-171">string</span><span class="sxs-lookup"><span data-stu-id="65c21-171">string</span></span>|<span data-ttu-id="65c21-172">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="65c21-172">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="65c21-173">id</span><span class="sxs-lookup"><span data-stu-id="65c21-173">id</span></span>|<span data-ttu-id="65c21-174">string</span><span class="sxs-lookup"><span data-stu-id="65c21-174">string</span></span>|<span data-ttu-id="65c21-175">管理单元的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="65c21-175">Unique identifier for the administrative unit.</span></span> <span data-ttu-id="65c21-176">只读。</span><span class="sxs-lookup"><span data-stu-id="65c21-176">Read-only.</span></span>|
|<span data-ttu-id="65c21-177">visibility</span><span class="sxs-lookup"><span data-stu-id="65c21-177">visibility</span></span>|<span data-ttu-id="65c21-178">string</span><span class="sxs-lookup"><span data-stu-id="65c21-178">string</span></span>|<span data-ttu-id="65c21-179">控制管理单元及其成员是隐藏的还是公开的。</span><span class="sxs-lookup"><span data-stu-id="65c21-179">Controls whether the administrative unit and its members are hidden or public.</span></span> <span data-ttu-id="65c21-180">可以设置为 `HiddenMembership` 或 `Public` 。</span><span class="sxs-lookup"><span data-stu-id="65c21-180">Can be set to `HiddenMembership` or `Public`.</span></span> <span data-ttu-id="65c21-181">如果未设置，默认行为为 `Public` 。</span><span class="sxs-lookup"><span data-stu-id="65c21-181">If not set, default behavior is `Public`.</span></span> <span data-ttu-id="65c21-182">设置为 `HiddenMembership` 时，只有管理单元的成员可以列出该管理单元的其他成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-182">When set to `HiddenMembership`, only members of the administrative unit can list other members of the administrative unit.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c21-183">关系</span><span class="sxs-lookup"><span data-stu-id="65c21-183">Relationships</span></span>
| <span data-ttu-id="65c21-184">关系</span><span class="sxs-lookup"><span data-stu-id="65c21-184">Relationship</span></span> | <span data-ttu-id="65c21-185">类型</span><span class="sxs-lookup"><span data-stu-id="65c21-185">Type</span></span>   |<span data-ttu-id="65c21-186">说明</span><span class="sxs-lookup"><span data-stu-id="65c21-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65c21-187">extensions</span><span class="sxs-lookup"><span data-stu-id="65c21-187">extensions</span></span>|<span data-ttu-id="65c21-188">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="65c21-188">[extension](extension.md) collection</span></span>|<span data-ttu-id="65c21-189">为此管理单元定义的开放扩展集合。</span><span class="sxs-lookup"><span data-stu-id="65c21-189">The collection of open extensions defined for this Administrative Unit.</span></span> <span data-ttu-id="65c21-190">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="65c21-190">Nullable.</span></span>|
|<span data-ttu-id="65c21-191">members</span><span class="sxs-lookup"><span data-stu-id="65c21-191">members</span></span>|<span data-ttu-id="65c21-192">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c21-192">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="65c21-193">是此管理单元的成员的用户和组。</span><span class="sxs-lookup"><span data-stu-id="65c21-193">Users and groups that are members of this Adminsitrative Unit.</span></span> <span data-ttu-id="65c21-194">HTTP 方法：GET (list members) 、POST (add members) 、DELETE (remove members) 。</span><span class="sxs-lookup"><span data-stu-id="65c21-194">HTTP Methods: GET (list members), POST (add members), DELETE (remove members).</span></span>|
|<span data-ttu-id="65c21-195">scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="65c21-195">scopedRoleMembers</span></span>|<span data-ttu-id="65c21-196">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c21-196">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="65c21-197">此管理单元的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="65c21-197">Scoped-role members of this Administrative Unit.</span></span>  <span data-ttu-id="65c21-198">HTTP 方法：GET (list scopedRoleMemberships) ，POST (add scopedRoleMembership) ， DELETE (remove scopedRoleMembership) 。</span><span class="sxs-lookup"><span data-stu-id="65c21-198">HTTP Methods: GET (list scopedRoleMemberships), POST (add scopedRoleMembership), DELETE (remove scopedRoleMembership).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65c21-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65c21-199">JSON representation</span></span>

<span data-ttu-id="65c21-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c21-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a><span data-ttu-id="65c21-201">另请参阅</span><span class="sxs-lookup"><span data-stu-id="65c21-201">See also</span></span>

- [<span data-ttu-id="65c21-202">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="65c21-202">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="65c21-203">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="65c21-203">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="65c21-204">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="65c21-204">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
