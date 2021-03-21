---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 44f0c10e6eb1cd1b95bdd4ba887721b65293d3f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957091"
---
# <a name="administrativeunit-resource-type"></a><span data-ttu-id="75f31-103">administrativeUnit 资源类型</span><span class="sxs-lookup"><span data-stu-id="75f31-103">administrativeUnit resource type</span></span>

<span data-ttu-id="75f31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f31-105">管理单元为用户和组目录对象提供概念容器。</span><span class="sxs-lookup"><span data-stu-id="75f31-105">An administrative unit provides a conceptual container for User and Group directory objects.</span></span> <span data-ttu-id="75f31-106">使用管理单元，公司管理员现在可以将管理职责委派给区域管理员或部门管理员，以管理管理单元中包含的用户和组或范围所包含的用户和组。</span><span class="sxs-lookup"><span data-stu-id="75f31-106">Using administrative units, a company administrator can now delegate administrative responsibilities to manage the users and groups contained within or scoped to an administrative unit to a regional or departmental administrator.</span></span>

<span data-ttu-id="75f31-107">该资源支持通过提供 [delta](../api/administrativeunit-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="75f31-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/administrativeunit-delta.md) function.</span></span>

<span data-ttu-id="75f31-108">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="75f31-108">Let's look at an example.</span></span> <span data-ttu-id="75f31-109">假设 Contoso Corp 由两个部门（一个东海岸分部和一个东海岸部门）负责。</span><span class="sxs-lookup"><span data-stu-id="75f31-109">Imagine that Contoso Corp is made up of two divisions - a West Coast Division and an East Coast Division.</span></span> <span data-ttu-id="75f31-110">Contoso 的目录角色的范围为整个租户。</span><span class="sxs-lookup"><span data-stu-id="75f31-110">Directory roles at Contoso are scoped to the entire tenant.</span></span> <span data-ttu-id="75f31-111">Contoso 公司管理员 Lee 希望委派管理责任，但将其范围划分到东海岸部门或东海岸分部。</span><span class="sxs-lookup"><span data-stu-id="75f31-111">Lee, a Contoso company administrator, wants to delegate administrative responsibilities, but scope them to the West Coast Division or the East Coast division.</span></span>  <span data-ttu-id="75f31-112">Lee 可以创建 *一个"东海岸* "管理单元，并可以将所有"东海岸"用户放入此管理单元中。</span><span class="sxs-lookup"><span data-stu-id="75f31-112">Lee can create a *West Coast admistrative unit* and place all West Coast users into this administrative unit.</span></span>  <span data-ttu-id="75f31-113">同样，Lee 可以创建一 *个"东海岸管理单元"。*</span><span class="sxs-lookup"><span data-stu-id="75f31-113">Similarly, Lee can create an *East Coast adminstrative unit*.</span></span>  <span data-ttu-id="75f31-114">现在，Lee 可以开始将管理职责委派给其他人，但作用域为自己创建的新管理单元。</span><span class="sxs-lookup"><span data-stu-id="75f31-114">Now Lee, can start delegating administrative responsibilities to others, but **scoped** to the new administrative units he's created.</span></span> <span data-ttu-id="75f31-115">Lee 将 Jennifer 设置在一个支持 *人员管理员* 角色 **中** ，该角色的作用范围为 *"东海岸"管理单元*。</span><span class="sxs-lookup"><span data-stu-id="75f31-115">Lee places Jennifer in a *helpdesk administrator* role **scoped** to the *West Coast administrative unit*.</span></span>  <span data-ttu-id="75f31-116">这允许 Jennifer 重置任何用户的密码，但只有在这些用户位于 *东海岸管理单元时。*</span><span class="sxs-lookup"><span data-stu-id="75f31-116">This allows Jennifer to reset any user's password, but only if those users are in the *West Coast administrative unit*.</span></span>  <span data-ttu-id="75f31-117">同样，Lee 将 Dave 设置在 *一个用户帐户管理员* 角色中，该角色的作用范围为"*东海岸"管理单元*。 </span><span class="sxs-lookup"><span data-stu-id="75f31-117">Similarly, Lee places Dave in a *user account administrator* role **scoped** to the *East Coast administrative unit*.</span></span>  <span data-ttu-id="75f31-118">这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但只有在这些用户位于东海岸管理 *单元中时。*</span><span class="sxs-lookup"><span data-stu-id="75f31-118">This allows Dave to update users, assign licenses and reset any user's password, but only if those users are in the *East Coast administrative unit*.</span></span> <span data-ttu-id="75f31-119">有关视频概述，请参阅 [Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。</span><span class="sxs-lookup"><span data-stu-id="75f31-119">For a video overview, please see [Introduction to Azure Active Directory Administrative Units](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).</span></span>

<span data-ttu-id="75f31-120">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="75f31-120">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="75f31-121">本主题提供 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。</span><span class="sxs-lookup"><span data-stu-id="75f31-121">This topic provides descriptions of the declared properties and navigation properties exposed by the administrativeUnit entity, as well as the operations and functions that can be called on the administrativeUnits resource.</span></span>


## <a name="methods"></a><span data-ttu-id="75f31-122">Methods</span><span class="sxs-lookup"><span data-stu-id="75f31-122">Methods</span></span>

| <span data-ttu-id="75f31-123">方法</span><span class="sxs-lookup"><span data-stu-id="75f31-123">Method</span></span>   | <span data-ttu-id="75f31-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="75f31-124">Return Type</span></span> | <span data-ttu-id="75f31-125">说明</span><span class="sxs-lookup"><span data-stu-id="75f31-125">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="75f31-126">创建</span><span class="sxs-lookup"><span data-stu-id="75f31-126">Create</span></span>](../api/administrativeunit-post-administrativeunits.md) | [<span data-ttu-id="75f31-127">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75f31-127">administrativeUnit</span></span>](administrativeunit.md) | <span data-ttu-id="75f31-128">创建新的管理单元。</span><span class="sxs-lookup"><span data-stu-id="75f31-128">Create a new administrative unit.</span></span>|
|[<span data-ttu-id="75f31-129">列表</span><span class="sxs-lookup"><span data-stu-id="75f31-129">List</span></span>](../api/administrativeunit-list.md) | <span data-ttu-id="75f31-130">[administrativeUnit](administrativeunit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f31-130">[administrativeUnit](administrativeunit.md) collection</span></span> |<span data-ttu-id="75f31-131">列出所有 administrativeUnits 的属性。</span><span class="sxs-lookup"><span data-stu-id="75f31-131">List properties of all administrativeUnits.</span></span>|
|[<span data-ttu-id="75f31-132">获取</span><span class="sxs-lookup"><span data-stu-id="75f31-132">Get</span></span>](../api/administrativeunit-get.md) | [<span data-ttu-id="75f31-133">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75f31-133">administrativeUnit</span></span>](administrativeunit.md) |<span data-ttu-id="75f31-134">读取特定 administrativeUnit 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75f31-134">Read properties and relationships of a specific administrativeUnit object.</span></span>|
|[<span data-ttu-id="75f31-135">更新</span><span class="sxs-lookup"><span data-stu-id="75f31-135">Update</span></span>](../api/administrativeunit-update.md) | [<span data-ttu-id="75f31-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75f31-136">administrativeUnit</span></span>](administrativeunit.md)    |<span data-ttu-id="75f31-137">更新 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="75f31-137">Update administrativeUnit object.</span></span> |
|[<span data-ttu-id="75f31-138">删除</span><span class="sxs-lookup"><span data-stu-id="75f31-138">Delete</span></span>](../api/administrativeunit-delete.md) | <span data-ttu-id="75f31-139">无</span><span class="sxs-lookup"><span data-stu-id="75f31-139">None</span></span> |<span data-ttu-id="75f31-140">删除 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="75f31-140">Delete administrativeUnit object.</span></span> |
|[<span data-ttu-id="75f31-141">获取增量</span><span class="sxs-lookup"><span data-stu-id="75f31-141">Get delta</span></span>](../api/administrativeunit-delta.md)|[<span data-ttu-id="75f31-142">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75f31-142">administrativeUnit</span></span>](administrativeunit.md)|<span data-ttu-id="75f31-143">获取新创建、更新或删除 **的管理单元** ，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="75f31-143">Get newly created, updated, or deleted **administrativeUnits** without having to perform a full read of the entire resource collection.</span></span>|
|[<span data-ttu-id="75f31-144">添加成员</span><span class="sxs-lookup"><span data-stu-id="75f31-144">Add a member</span></span>](../api/administrativeunit-post-members.md) |[<span data-ttu-id="75f31-145">directoryObject</span><span class="sxs-lookup"><span data-stu-id="75f31-145">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="75f31-146">向用户 (组添加成员) 。</span><span class="sxs-lookup"><span data-stu-id="75f31-146">Add a member (user or group).</span></span>|
|[<span data-ttu-id="75f31-147">List members</span><span class="sxs-lookup"><span data-stu-id="75f31-147">List members</span></span>](../api/administrativeunit-list-members.md) |<span data-ttu-id="75f31-148">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f31-148">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="75f31-149">获取用户和 (组) 列表。</span><span class="sxs-lookup"><span data-stu-id="75f31-149">Get the list of (user and group) members.</span></span>|
|[<span data-ttu-id="75f31-150">获取成员</span><span class="sxs-lookup"><span data-stu-id="75f31-150">Get a member</span></span>](../api/administrativeunit-get-members.md) |[<span data-ttu-id="75f31-151">directoryObject</span><span class="sxs-lookup"><span data-stu-id="75f31-151">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="75f31-152">获取特定成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-152">Get a specific member.</span></span>|
|[<span data-ttu-id="75f31-153">删除成员</span><span class="sxs-lookup"><span data-stu-id="75f31-153">Remove a member</span></span>](../api/administrativeunit-delete-members.md) |[<span data-ttu-id="75f31-154">directoryObject</span><span class="sxs-lookup"><span data-stu-id="75f31-154">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="75f31-155">删除成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-155">Remove a member.</span></span>|
|[<span data-ttu-id="75f31-156">添加作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="75f31-156">Add scoped-role member</span></span>](../api/administrativeunit-post-scopedrolemembers.md) |[<span data-ttu-id="75f31-157">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="75f31-157">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="75f31-158">添加作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-158">Add a scoped-role member.</span></span>|
|[<span data-ttu-id="75f31-159">列出作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="75f31-159">List scoped-role members</span></span>](../api/administrativeunit-list-scopedrolemembers.md) |<span data-ttu-id="75f31-160">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f31-160">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="75f31-161">获取作用域角色管理员列表。</span><span class="sxs-lookup"><span data-stu-id="75f31-161">Get the list of scoped-role administrators.</span></span>|
|[<span data-ttu-id="75f31-162">获取作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="75f31-162">Get a scoped-role member</span></span>](../api/administrativeunit-get-scopedrolemembers.md) |[<span data-ttu-id="75f31-163">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="75f31-163">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="75f31-164">获取特定作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-164">Get a specific scoped-role member.</span></span>|
|[<span data-ttu-id="75f31-165">删除作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="75f31-165">Remove a scoped-role member</span></span>](../api/administrativeunit-delete-scopedrolemembers.md) |[<span data-ttu-id="75f31-166">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="75f31-166">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="75f31-167">删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-167">Remove a scoped-role member.</span></span>|
|<span data-ttu-id="75f31-168">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="75f31-168">**Open extensions**</span></span>| | |
|[<span data-ttu-id="75f31-169">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="75f31-169">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="75f31-170">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75f31-170">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="75f31-171">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="75f31-171">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="75f31-172">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="75f31-172">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="75f31-173">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f31-173">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="75f31-174">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="75f31-174">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="75f31-175">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="75f31-175">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="75f31-176">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="75f31-176">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="75f31-177">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="75f31-177">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="75f31-178">属性</span><span class="sxs-lookup"><span data-stu-id="75f31-178">Properties</span></span>
| <span data-ttu-id="75f31-179">属性</span><span class="sxs-lookup"><span data-stu-id="75f31-179">Property</span></span>     | <span data-ttu-id="75f31-180">类型</span><span class="sxs-lookup"><span data-stu-id="75f31-180">Type</span></span>   |<span data-ttu-id="75f31-181">说明</span><span class="sxs-lookup"><span data-stu-id="75f31-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75f31-182">说明</span><span class="sxs-lookup"><span data-stu-id="75f31-182">description</span></span>|<span data-ttu-id="75f31-183">string</span><span class="sxs-lookup"><span data-stu-id="75f31-183">string</span></span>|<span data-ttu-id="75f31-184">管理单元的可选说明。</span><span class="sxs-lookup"><span data-stu-id="75f31-184">An optional description for the administrative unit.</span></span>|
|<span data-ttu-id="75f31-185">displayName</span><span class="sxs-lookup"><span data-stu-id="75f31-185">displayName</span></span>|<span data-ttu-id="75f31-186">string</span><span class="sxs-lookup"><span data-stu-id="75f31-186">string</span></span>|<span data-ttu-id="75f31-187">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="75f31-187">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="75f31-188">id</span><span class="sxs-lookup"><span data-stu-id="75f31-188">id</span></span>|<span data-ttu-id="75f31-189">string</span><span class="sxs-lookup"><span data-stu-id="75f31-189">string</span></span>|<span data-ttu-id="75f31-190">管理单元的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75f31-190">Unique identifier for the administrative unit.</span></span> <span data-ttu-id="75f31-191">只读。</span><span class="sxs-lookup"><span data-stu-id="75f31-191">Read-only.</span></span>|
|<span data-ttu-id="75f31-192">visibility</span><span class="sxs-lookup"><span data-stu-id="75f31-192">visibility</span></span>|<span data-ttu-id="75f31-193">string</span><span class="sxs-lookup"><span data-stu-id="75f31-193">string</span></span>|<span data-ttu-id="75f31-194">控制管理单元及其成员是隐藏的还是公开的。</span><span class="sxs-lookup"><span data-stu-id="75f31-194">Controls whether the administrative unit and its members are hidden or public.</span></span> <span data-ttu-id="75f31-195">可以设置为 `HiddenMembership` 或 `Public` 。</span><span class="sxs-lookup"><span data-stu-id="75f31-195">Can be set to `HiddenMembership` or `Public`.</span></span> <span data-ttu-id="75f31-196">如果未设置，默认行为为 `Public` 。</span><span class="sxs-lookup"><span data-stu-id="75f31-196">If not set, default behavior is `Public`.</span></span> <span data-ttu-id="75f31-197">设置为 `HiddenMembership` 时，只有管理单元的成员可以列出该管理单元的其他成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-197">When set to `HiddenMembership`, only members of the administrative unit can list other members of the administrative unit.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75f31-198">关系</span><span class="sxs-lookup"><span data-stu-id="75f31-198">Relationships</span></span>
| <span data-ttu-id="75f31-199">关系</span><span class="sxs-lookup"><span data-stu-id="75f31-199">Relationship</span></span> | <span data-ttu-id="75f31-200">类型</span><span class="sxs-lookup"><span data-stu-id="75f31-200">Type</span></span>   |<span data-ttu-id="75f31-201">说明</span><span class="sxs-lookup"><span data-stu-id="75f31-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75f31-202">extensions</span><span class="sxs-lookup"><span data-stu-id="75f31-202">extensions</span></span>|<span data-ttu-id="75f31-203">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="75f31-203">[extension](extension.md) collection</span></span>|<span data-ttu-id="75f31-204">为此管理单元定义的开放扩展集合。</span><span class="sxs-lookup"><span data-stu-id="75f31-204">The collection of open extensions defined for this Administrative Unit.</span></span> <span data-ttu-id="75f31-205">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="75f31-205">Nullable.</span></span>|
|<span data-ttu-id="75f31-206">members</span><span class="sxs-lookup"><span data-stu-id="75f31-206">members</span></span>|<span data-ttu-id="75f31-207">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="75f31-207">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="75f31-208">是此管理单元的成员的用户和组。</span><span class="sxs-lookup"><span data-stu-id="75f31-208">Users and groups that are members of this Adminsitrative Unit.</span></span> <span data-ttu-id="75f31-209">HTTP 方法：GET (list members) 、POST (add members) 、DELETE (remove members) 。</span><span class="sxs-lookup"><span data-stu-id="75f31-209">HTTP Methods: GET (list members), POST (add members), DELETE (remove members).</span></span>|
|<span data-ttu-id="75f31-210">scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="75f31-210">scopedRoleMembers</span></span>|<span data-ttu-id="75f31-211">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75f31-211">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="75f31-212">此管理单元的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="75f31-212">Scoped-role members of this Administrative Unit.</span></span>  <span data-ttu-id="75f31-213">HTTP 方法：GET (list scopedRoleMemberships) ，POST (add scopedRoleMembership) ， DELETE (remove scopedRoleMembership) 。</span><span class="sxs-lookup"><span data-stu-id="75f31-213">HTTP Methods: GET (list scopedRoleMemberships), POST (add scopedRoleMembership), DELETE (remove scopedRoleMembership).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75f31-214">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75f31-214">JSON representation</span></span>

<span data-ttu-id="75f31-215">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75f31-215">Here is a JSON representation of the resource.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="75f31-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="75f31-216">See also</span></span>

- [<span data-ttu-id="75f31-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="75f31-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="75f31-218">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="75f31-218">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="75f31-219">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="75f31-219">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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


