---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供了一个概念性容器。 通过使用管理单元，公司管理员现在可以将管理责任委派给区域或部门管理员，以管理包含在管理单元或范围内的用户和组。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d279bcfd605df8d53331cc217d7b5fdb76510659
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508392"
---
# <a name="administrativeunit-resource-type"></a><span data-ttu-id="2e93b-104">administrativeUnit 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e93b-104">administrativeUnit resource type</span></span>

<span data-ttu-id="2e93b-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2e93b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e93b-106">管理单元为用户和组目录对象提供了一个概念性容器。</span><span class="sxs-lookup"><span data-stu-id="2e93b-106">An administrative unit provides a conceptual container for User and Group directory objects.</span></span> <span data-ttu-id="2e93b-107">通过使用管理单元，公司管理员现在可以将管理责任委派给区域或部门管理员，以管理包含在管理单元或范围内的用户和组。</span><span class="sxs-lookup"><span data-stu-id="2e93b-107">Using administrative units, a company administrator can now delegate administrative responsibilities to manage the users and groups contained within or scoped to an administrative unit to a regional or departmental administrator.</span></span>

<span data-ttu-id="2e93b-108">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="2e93b-108">Let's look at an example.</span></span> <span data-ttu-id="2e93b-109">假设 Contoso Corp 由两个部门组成-一个 West 海岸部门和一个东海岸部门。</span><span class="sxs-lookup"><span data-stu-id="2e93b-109">Imagine that Contoso Corp is made up of two divisions - a West Coast Division and an East Coast Division.</span></span> <span data-ttu-id="2e93b-110">Contoso 的目录角色的作用范围限定为整个租户。</span><span class="sxs-lookup"><span data-stu-id="2e93b-110">Directory roles at Contoso are scoped to the entire tenant.</span></span> <span data-ttu-id="2e93b-111">先生，Contoso company administrator，想要委派管理责任，但将这些职责范围限定为 West 海岸部门或东海岸部门。</span><span class="sxs-lookup"><span data-stu-id="2e93b-111">Lee, a Contoso company administrator, wants to delegate administrative responsibilities, but scope them to the West Coast Division or the East Coast division.</span></span>  <span data-ttu-id="2e93b-112">用户可以创建*西海岸 admistrative 单元*，并将所有 West 海岸用户放入此管理单元。</span><span class="sxs-lookup"><span data-stu-id="2e93b-112">Lee can create a *West Coast admistrative unit* and place all West Coast users into this administrative unit.</span></span>  <span data-ttu-id="2e93b-113">同样，他可以创建一个*东海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="2e93b-113">Similarly, Lee can create an *East Coast adminstrative unit*.</span></span>  <span data-ttu-id="2e93b-114">现在，可以开始将管理责任委派给其他人，但**范围限定**为创建的新管理单元。</span><span class="sxs-lookup"><span data-stu-id="2e93b-114">Now Lee, can start delegating administrative responsibilities to others, but **scoped** to the new administrative units he's created.</span></span> <span data-ttu-id="2e93b-115">先生将 Jennifer 放在*帮助台管理员*角色中，**作用域**为*西海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="2e93b-115">Lee places Jennifer in a *helpdesk administrator* role **scoped** to the *West Coast administrative unit*.</span></span>  <span data-ttu-id="2e93b-116">这允许 Jennifer 重置任何用户的密码，但前提是这些用户位于*西海岸管理单元*中。</span><span class="sxs-lookup"><span data-stu-id="2e93b-116">This allows Jennifer to reset any user's password, but only if those users are in the *West Coast administrative unit*.</span></span>  <span data-ttu-id="2e93b-117">同样，工作先生将 Dave 放在*用户帐户管理员*角色中，该角色的**作用域**为*东海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="2e93b-117">Similarly, Lee places Dave in a *user account administrator* role **scoped** to the *East Coast administrative unit*.</span></span>  <span data-ttu-id="2e93b-118">这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但前提是这些用户位于 "*东海岸" 管理单元*中。</span><span class="sxs-lookup"><span data-stu-id="2e93b-118">This allows Dave to update users, assign licenses and reset any user's password, but only if those users are in the *East Coast administrative unit*.</span></span> <span data-ttu-id="2e93b-119">有关视频概述，请参阅[Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。</span><span class="sxs-lookup"><span data-stu-id="2e93b-119">For a video overview, please see [Introduction to Azure Active Directory Administrative Units](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).</span></span>

<span data-ttu-id="2e93b-120">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="2e93b-120">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="2e93b-121">本主题提供由 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。</span><span class="sxs-lookup"><span data-stu-id="2e93b-121">This topic provides descriptions of the declared properties and navigation properties exposed by the administrativeUnit entity, as well as the operations and functions that can be called on the administrativeUnits resource.</span></span>


## <a name="methods"></a><span data-ttu-id="2e93b-122">方法</span><span class="sxs-lookup"><span data-stu-id="2e93b-122">Methods</span></span>

| <span data-ttu-id="2e93b-123">方法</span><span class="sxs-lookup"><span data-stu-id="2e93b-123">Method</span></span>   | <span data-ttu-id="2e93b-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="2e93b-124">Return Type</span></span> | <span data-ttu-id="2e93b-125">说明</span><span class="sxs-lookup"><span data-stu-id="2e93b-125">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e93b-126">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-126">Create administrativeUnit</span></span>](../api/administrativeunit-post-administrativeunits.md) | [<span data-ttu-id="2e93b-127">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-127">administrativeUnit</span></span>](administrativeunit.md) | <span data-ttu-id="2e93b-128">创建新的管理单元。</span><span class="sxs-lookup"><span data-stu-id="2e93b-128">Create a new administrative unit.</span></span>|
|[<span data-ttu-id="2e93b-129">列出 administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="2e93b-129">List administrativeUnits</span></span>](../api/administrativeunit-list.md) | <span data-ttu-id="2e93b-130">[administrativeUnit](administrativeunit.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-130">[administrativeUnit](administrativeunit.md) collection</span></span> |<span data-ttu-id="2e93b-131">列出所有 administrativeUnits 的属性。</span><span class="sxs-lookup"><span data-stu-id="2e93b-131">List properties of all administrativeUnits.</span></span>|
|[<span data-ttu-id="2e93b-132">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-132">Get administrativeUnit</span></span>](../api/administrativeunit-get.md) | [<span data-ttu-id="2e93b-133">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-133">administrativeUnit</span></span>](administrativeunit.md) |<span data-ttu-id="2e93b-134">读取特定 administrativeUnit 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2e93b-134">Read properties and relationships of a specific administrativeUnit object.</span></span>|
|[<span data-ttu-id="2e93b-135">更新 adminstrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-135">Update adminstrativeUnit</span></span>](../api/administrativeunit-update.md) | [<span data-ttu-id="2e93b-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-136">administrativeUnit</span></span>](administrativeunit.md)  |<span data-ttu-id="2e93b-137">更新 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="2e93b-137">Update administrativeUnit object.</span></span> |
|[<span data-ttu-id="2e93b-138">删除 adminstrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2e93b-138">Delete adminstrativeUnit</span></span>](../api/administrativeunit-delete.md) | <span data-ttu-id="2e93b-139">无</span><span class="sxs-lookup"><span data-stu-id="2e93b-139">None</span></span> |<span data-ttu-id="2e93b-140">删除 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="2e93b-140">Delete administrativeUnit object.</span></span> |
|[<span data-ttu-id="2e93b-141">添加成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-141">Add a member</span></span>](../api/administrativeunit-post-members.md) |[<span data-ttu-id="2e93b-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2e93b-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="2e93b-143">添加成员（用户或组）。</span><span class="sxs-lookup"><span data-stu-id="2e93b-143">Add a member (user or group).</span></span>|
|[<span data-ttu-id="2e93b-144">列出成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-144">List members</span></span>](../api/administrativeunit-list-members.md) |<span data-ttu-id="2e93b-145">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2e93b-146">获取（用户和组）成员的列表。</span><span class="sxs-lookup"><span data-stu-id="2e93b-146">Get the list of (user and group) members.</span></span>|
|[<span data-ttu-id="2e93b-147">获取成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-147">Get a member</span></span>](../api/administrativeunit-get-members.md) |[<span data-ttu-id="2e93b-148">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2e93b-148">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="2e93b-149">获取特定成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-149">Get a specific member.</span></span>|
|[<span data-ttu-id="2e93b-150">删除成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-150">Remove a member</span></span>](../api/administrativeunit-delete-members.md) |[<span data-ttu-id="2e93b-151">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2e93b-151">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="2e93b-152">删除成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-152">Remove a member.</span></span>|
|[<span data-ttu-id="2e93b-153">添加作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-153">Add scoped-role member</span></span>](../api/administrativeunit-post-scopedrolemembers.md) |[<span data-ttu-id="2e93b-154">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="2e93b-154">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="2e93b-155">添加作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-155">Add a scoped-role member.</span></span>|
|[<span data-ttu-id="2e93b-156">列出作用域内的角色成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-156">List scoped-role members</span></span>](../api/administrativeunit-list-scopedrolemembers.md) |<span data-ttu-id="2e93b-157">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-157">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="2e93b-158">获取作用域角色管理员的列表。</span><span class="sxs-lookup"><span data-stu-id="2e93b-158">Get the list of scoped-role administrators.</span></span>|
|[<span data-ttu-id="2e93b-159">获取作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-159">Get a scoped-role member</span></span>](../api/administrativeunit-get-scopedrolemembers.md) |[<span data-ttu-id="2e93b-160">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="2e93b-160">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="2e93b-161">获取特定的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-161">Get a specific scoped-role member.</span></span>|
|[<span data-ttu-id="2e93b-162">删除作用域范围的角色成员</span><span class="sxs-lookup"><span data-stu-id="2e93b-162">Remove a scoped-role member</span></span>](../api/administrativeunit-delete-scopedrolemembers.md) |[<span data-ttu-id="2e93b-163">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="2e93b-163">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="2e93b-164">删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-164">Remove a scoped-role member.</span></span>|
|<span data-ttu-id="2e93b-165">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="2e93b-165">**Open extensions**</span></span>| | |
|[<span data-ttu-id="2e93b-166">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="2e93b-166">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="2e93b-167">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="2e93b-167">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="2e93b-168">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="2e93b-168">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="2e93b-169">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="2e93b-169">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="2e93b-170">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-170">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="2e93b-171">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="2e93b-171">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="2e93b-172">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="2e93b-172">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="2e93b-173">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="2e93b-173">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="2e93b-174">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="2e93b-174">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e93b-175">属性</span><span class="sxs-lookup"><span data-stu-id="2e93b-175">Properties</span></span>
| <span data-ttu-id="2e93b-176">属性</span><span class="sxs-lookup"><span data-stu-id="2e93b-176">Property</span></span>     | <span data-ttu-id="2e93b-177">类型</span><span class="sxs-lookup"><span data-stu-id="2e93b-177">Type</span></span>   |<span data-ttu-id="2e93b-178">说明</span><span class="sxs-lookup"><span data-stu-id="2e93b-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e93b-179">说明</span><span class="sxs-lookup"><span data-stu-id="2e93b-179">description</span></span>|<span data-ttu-id="2e93b-180">string</span><span class="sxs-lookup"><span data-stu-id="2e93b-180">string</span></span>|<span data-ttu-id="2e93b-181">管理单元的可选说明。</span><span class="sxs-lookup"><span data-stu-id="2e93b-181">An optional description for the administrative unit.</span></span>|
|<span data-ttu-id="2e93b-182">displayName</span><span class="sxs-lookup"><span data-stu-id="2e93b-182">displayName</span></span>|<span data-ttu-id="2e93b-183">string</span><span class="sxs-lookup"><span data-stu-id="2e93b-183">string</span></span>|<span data-ttu-id="2e93b-184">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2e93b-184">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="2e93b-185">id</span><span class="sxs-lookup"><span data-stu-id="2e93b-185">id</span></span>|<span data-ttu-id="2e93b-186">string</span><span class="sxs-lookup"><span data-stu-id="2e93b-186">string</span></span>|<span data-ttu-id="2e93b-187">管理单元的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2e93b-187">Unique identifier for the administrative unit.</span></span> <span data-ttu-id="2e93b-188">只读。</span><span class="sxs-lookup"><span data-stu-id="2e93b-188">Read-only.</span></span>|
|<span data-ttu-id="2e93b-189">visibility</span><span class="sxs-lookup"><span data-stu-id="2e93b-189">visibility</span></span>|<span data-ttu-id="2e93b-190">string</span><span class="sxs-lookup"><span data-stu-id="2e93b-190">string</span></span>|<span data-ttu-id="2e93b-191">控制管理单元及其成员是否为隐藏或公共的。</span><span class="sxs-lookup"><span data-stu-id="2e93b-191">Controls whether the adminstrative unit and its members are hidden or public.</span></span> <span data-ttu-id="2e93b-192">可以设置为 HiddenMembership 或 Public。</span><span class="sxs-lookup"><span data-stu-id="2e93b-192">Can be set to HiddenMembership or Public.</span></span> <span data-ttu-id="2e93b-193">如果未设置，则默认行为是公共行为。</span><span class="sxs-lookup"><span data-stu-id="2e93b-193">If not set, default behavior is Public.</span></span> <span data-ttu-id="2e93b-194">如果设置为 HiddenMembership，则只有管理单元的成员可以列出管理单位的其他成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-194">When set to HiddenMembership, only members of the administrative unit can list other members of the adminstrative unit.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e93b-195">关系</span><span class="sxs-lookup"><span data-stu-id="2e93b-195">Relationships</span></span>
| <span data-ttu-id="2e93b-196">关系</span><span class="sxs-lookup"><span data-stu-id="2e93b-196">Relationship</span></span> | <span data-ttu-id="2e93b-197">类型</span><span class="sxs-lookup"><span data-stu-id="2e93b-197">Type</span></span>   |<span data-ttu-id="2e93b-198">说明</span><span class="sxs-lookup"><span data-stu-id="2e93b-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e93b-199">extensions</span><span class="sxs-lookup"><span data-stu-id="2e93b-199">extensions</span></span>|<span data-ttu-id="2e93b-200">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-200">[extension](extension.md) collection</span></span>|<span data-ttu-id="2e93b-201">为此管理单元定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="2e93b-201">The collection of open extensions defined for this Administrative Unit.</span></span> <span data-ttu-id="2e93b-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2e93b-202">Nullable.</span></span>|
|<span data-ttu-id="2e93b-203">members</span><span class="sxs-lookup"><span data-stu-id="2e93b-203">members</span></span>|<span data-ttu-id="2e93b-204">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-204">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="2e93b-205">作为此 Adminsitrative 单位的成员的用户和组。</span><span class="sxs-lookup"><span data-stu-id="2e93b-205">Users and groups that are members of this Adminsitrative Unit.</span></span> <span data-ttu-id="2e93b-206">HTTP 方法： GET （list members）、POST （添加成员）、删除（移除成员）。</span><span class="sxs-lookup"><span data-stu-id="2e93b-206">HTTP Methods: GET (list members), POST (add members), DELETE (remove members).</span></span>|
|<span data-ttu-id="2e93b-207">scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="2e93b-207">scopedRoleMembers</span></span>|<span data-ttu-id="2e93b-208">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e93b-208">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="2e93b-209">此管理单元的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="2e93b-209">Scoped-role members of this Administrative Unit.</span></span>  <span data-ttu-id="2e93b-210">HTTP 方法： GET （list scopedRoleMemberships）、POST （add scopedRoleMembership）、DELETE （remove scopedRoleMembership）。</span><span class="sxs-lookup"><span data-stu-id="2e93b-210">HTTP Methods: GET (list scopedRoleMemberships), POST (add scopedRoleMembership), DELETE (remove scopedRoleMembership).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e93b-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e93b-211">JSON representation</span></span>

<span data-ttu-id="2e93b-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e93b-212">Here is a JSON representation of the resource.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="2e93b-213">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e93b-213">See also</span></span>

- [<span data-ttu-id="2e93b-214">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e93b-214">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2e93b-215">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e93b-215">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2e93b-216">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e93b-216">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
