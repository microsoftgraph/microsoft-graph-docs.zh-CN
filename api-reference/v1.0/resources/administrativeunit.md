---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供了一个概念性容器。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e97ca2eba834931e311c3f10b85991697d66360b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059533"
---
# <a name="administrativeunit-resource-type"></a><span data-ttu-id="757f1-103">administrativeUnit 资源类型</span><span class="sxs-lookup"><span data-stu-id="757f1-103">administrativeUnit resource type</span></span>

<span data-ttu-id="757f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="757f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="757f1-105">管理单元为用户和组目录对象提供了一个概念性容器。</span><span class="sxs-lookup"><span data-stu-id="757f1-105">An administrative unit provides a conceptual container for User and Group directory objects.</span></span> <span data-ttu-id="757f1-106">通过使用管理单元，公司管理员现在可以将管理责任委派给区域或部门管理员，以管理包含在管理单元或范围内的用户和组。</span><span class="sxs-lookup"><span data-stu-id="757f1-106">Using administrative units, a company administrator can now delegate administrative responsibilities to manage the users and groups contained within or scoped to an administrative unit to a regional or departmental administrator.</span></span>

<span data-ttu-id="757f1-107">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="757f1-107">Let's look at an example.</span></span> <span data-ttu-id="757f1-108">假设 Contoso Corp 由两个部门组成-一个 West 海岸部门和一个东海岸部门。</span><span class="sxs-lookup"><span data-stu-id="757f1-108">Imagine that Contoso Corp is made up of two divisions - a West Coast Division and an East Coast Division.</span></span> <span data-ttu-id="757f1-109">Contoso 的目录角色的作用范围限定为整个租户。</span><span class="sxs-lookup"><span data-stu-id="757f1-109">Directory roles at Contoso are scoped to the entire tenant.</span></span> <span data-ttu-id="757f1-110">先生，Contoso company administrator，想要委派管理责任，但将这些职责范围限定为 West 海岸部门或东海岸部门。</span><span class="sxs-lookup"><span data-stu-id="757f1-110">Lee, a Contoso company administrator, wants to delegate administrative responsibilities, but scope them to the West Coast Division or the East Coast division.</span></span>  <span data-ttu-id="757f1-111">用户可以创建 *西海岸 admistrative 单元* ，并将所有 West 海岸用户放入此管理单元。</span><span class="sxs-lookup"><span data-stu-id="757f1-111">Lee can create a *West Coast admistrative unit* and place all West Coast users into this administrative unit.</span></span>  <span data-ttu-id="757f1-112">同样，他可以创建一个 *东海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="757f1-112">Similarly, Lee can create an *East Coast adminstrative unit*.</span></span>  <span data-ttu-id="757f1-113">现在，可以开始将管理责任委派给其他人，但 **范围限定** 为创建的新管理单元。</span><span class="sxs-lookup"><span data-stu-id="757f1-113">Now Lee, can start delegating administrative responsibilities to others, but **scoped** to the new administrative units he's created.</span></span> <span data-ttu-id="757f1-114">先生将 Jennifer 放在 *帮助台管理员* 角色中， **作用域** 为 *西海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="757f1-114">Lee places Jennifer in a *helpdesk administrator* role **scoped** to the *West Coast administrative unit*.</span></span>  <span data-ttu-id="757f1-115">这允许 Jennifer 重置任何用户的密码，但前提是这些用户位于 *西海岸管理单元*中。</span><span class="sxs-lookup"><span data-stu-id="757f1-115">This allows Jennifer to reset any user's password, but only if those users are in the *West Coast administrative unit*.</span></span>  <span data-ttu-id="757f1-116">同样，工作先生将 Dave 放在 *用户帐户管理员* 角色中，该角色的 **作用域** 为 *东海岸管理单元*。</span><span class="sxs-lookup"><span data-stu-id="757f1-116">Similarly, Lee places Dave in a *user account administrator* role **scoped** to the *East Coast administrative unit*.</span></span>  <span data-ttu-id="757f1-117">这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但前提是这些用户位于 " *东海岸" 管理单元*中。</span><span class="sxs-lookup"><span data-stu-id="757f1-117">This allows Dave to update users, assign licenses and reset any user's password, but only if those users are in the *East Coast administrative unit*.</span></span> <span data-ttu-id="757f1-118">有关视频概述，请参阅 [Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。</span><span class="sxs-lookup"><span data-stu-id="757f1-118">For a video overview, please see [Introduction to Azure Active Directory Administrative Units](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).</span></span>


<span data-ttu-id="757f1-119">本主题提供由 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。</span><span class="sxs-lookup"><span data-stu-id="757f1-119">This topic provides descriptions of the declared properties and navigation properties exposed by the administrativeUnit entity, as well as the operations and functions that can be called on the administrativeUnits resource.</span></span>


## <a name="methods"></a><span data-ttu-id="757f1-120">方法</span><span class="sxs-lookup"><span data-stu-id="757f1-120">Methods</span></span>

| <span data-ttu-id="757f1-121">方法</span><span class="sxs-lookup"><span data-stu-id="757f1-121">Method</span></span>   | <span data-ttu-id="757f1-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="757f1-122">Return Type</span></span> | <span data-ttu-id="757f1-123">说明</span><span class="sxs-lookup"><span data-stu-id="757f1-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="757f1-124">创建</span><span class="sxs-lookup"><span data-stu-id="757f1-124">Create</span></span>](../api/administrativeunit-post-administrativeunits.md) | [<span data-ttu-id="757f1-125">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="757f1-125">administrativeUnit</span></span>](administrativeunit.md) | <span data-ttu-id="757f1-126">创建新的管理单元。</span><span class="sxs-lookup"><span data-stu-id="757f1-126">Create a new administrative unit.</span></span>|
|[<span data-ttu-id="757f1-127">List</span><span class="sxs-lookup"><span data-stu-id="757f1-127">List</span></span>](../api/administrativeunit-list.md) | <span data-ttu-id="757f1-128">[administrativeUnit](administrativeunit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="757f1-128">[administrativeUnit](administrativeunit.md) collection</span></span> |<span data-ttu-id="757f1-129">列出所有 administrativeUnits 的属性。</span><span class="sxs-lookup"><span data-stu-id="757f1-129">List properties of all administrativeUnits.</span></span>|
|[<span data-ttu-id="757f1-130">获取</span><span class="sxs-lookup"><span data-stu-id="757f1-130">Get</span></span>](../api/administrativeunit-get.md) | [<span data-ttu-id="757f1-131">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="757f1-131">administrativeUnit</span></span>](administrativeunit.md) |<span data-ttu-id="757f1-132">读取特定 administrativeUnit 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="757f1-132">Read properties and relationships of a specific administrativeUnit object.</span></span>|
|[<span data-ttu-id="757f1-133">更新</span><span class="sxs-lookup"><span data-stu-id="757f1-133">Update</span></span>](../api/administrativeunit-update.md) | [<span data-ttu-id="757f1-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="757f1-134">administrativeUnit</span></span>](administrativeunit.md)    |<span data-ttu-id="757f1-135">更新 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="757f1-135">Update administrativeUnit object.</span></span> |
|[<span data-ttu-id="757f1-136">删除</span><span class="sxs-lookup"><span data-stu-id="757f1-136">Delete</span></span>](../api/administrativeunit-delete.md) | <span data-ttu-id="757f1-137">无</span><span class="sxs-lookup"><span data-stu-id="757f1-137">None</span></span> |<span data-ttu-id="757f1-138">删除 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="757f1-138">Delete administrativeUnit object.</span></span> |
|[<span data-ttu-id="757f1-139">添加成员</span><span class="sxs-lookup"><span data-stu-id="757f1-139">Add a member</span></span>](../api/administrativeunit-post-members.md) |[<span data-ttu-id="757f1-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="757f1-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="757f1-141">将成员添加 (用户或组) 。</span><span class="sxs-lookup"><span data-stu-id="757f1-141">Add a member (user or group).</span></span>|
|[<span data-ttu-id="757f1-142">List members</span><span class="sxs-lookup"><span data-stu-id="757f1-142">List members</span></span>](../api/administrativeunit-list-members.md) |<span data-ttu-id="757f1-143">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="757f1-143">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="757f1-144">获取 (的用户和组) 成员的列表。</span><span class="sxs-lookup"><span data-stu-id="757f1-144">Get the list of (user and group) members.</span></span>|
|[<span data-ttu-id="757f1-145">获取成员</span><span class="sxs-lookup"><span data-stu-id="757f1-145">Get a member</span></span>](../api/administrativeunit-get-members.md) |[<span data-ttu-id="757f1-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="757f1-146">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="757f1-147">获取特定成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-147">Get a specific member.</span></span>|
|[<span data-ttu-id="757f1-148">删除成员</span><span class="sxs-lookup"><span data-stu-id="757f1-148">Remove a member</span></span>](../api/administrativeunit-delete-members.md) |[<span data-ttu-id="757f1-149">directoryObject</span><span class="sxs-lookup"><span data-stu-id="757f1-149">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="757f1-150">删除成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-150">Remove a member.</span></span>|
|[<span data-ttu-id="757f1-151">添加作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="757f1-151">Add scoped-role member</span></span>](../api/administrativeunit-post-scopedrolemembers.md) |[<span data-ttu-id="757f1-152">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="757f1-152">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="757f1-153">添加作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-153">Add a scoped-role member.</span></span>|
|[<span data-ttu-id="757f1-154">列出作用域内的角色成员</span><span class="sxs-lookup"><span data-stu-id="757f1-154">List scoped-role members</span></span>](../api/administrativeunit-list-scopedrolemembers.md) |<span data-ttu-id="757f1-155">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="757f1-155">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="757f1-156">获取作用域角色管理员的列表。</span><span class="sxs-lookup"><span data-stu-id="757f1-156">Get the list of scoped-role administrators.</span></span>|
|[<span data-ttu-id="757f1-157">获取作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="757f1-157">Get a scoped-role member</span></span>](../api/administrativeunit-get-scopedrolemembers.md) |[<span data-ttu-id="757f1-158">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="757f1-158">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="757f1-159">获取特定的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-159">Get a specific scoped-role member.</span></span>|
|[<span data-ttu-id="757f1-160">删除作用域范围的角色成员</span><span class="sxs-lookup"><span data-stu-id="757f1-160">Remove a scoped-role member</span></span>](../api/administrativeunit-delete-scopedrolemembers.md) |[<span data-ttu-id="757f1-161">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="757f1-161">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="757f1-162">删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-162">Remove a scoped-role member.</span></span>|

## <a name="properties"></a><span data-ttu-id="757f1-163">属性</span><span class="sxs-lookup"><span data-stu-id="757f1-163">Properties</span></span>
| <span data-ttu-id="757f1-164">属性</span><span class="sxs-lookup"><span data-stu-id="757f1-164">Property</span></span>     | <span data-ttu-id="757f1-165">类型</span><span class="sxs-lookup"><span data-stu-id="757f1-165">Type</span></span>   |<span data-ttu-id="757f1-166">说明</span><span class="sxs-lookup"><span data-stu-id="757f1-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="757f1-167">说明</span><span class="sxs-lookup"><span data-stu-id="757f1-167">description</span></span>|<span data-ttu-id="757f1-168">string</span><span class="sxs-lookup"><span data-stu-id="757f1-168">string</span></span>|<span data-ttu-id="757f1-169">管理单元的可选说明。</span><span class="sxs-lookup"><span data-stu-id="757f1-169">An optional description for the administrative unit.</span></span>|
|<span data-ttu-id="757f1-170">displayName</span><span class="sxs-lookup"><span data-stu-id="757f1-170">displayName</span></span>|<span data-ttu-id="757f1-171">string</span><span class="sxs-lookup"><span data-stu-id="757f1-171">string</span></span>|<span data-ttu-id="757f1-172">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="757f1-172">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="757f1-173">id</span><span class="sxs-lookup"><span data-stu-id="757f1-173">id</span></span>|<span data-ttu-id="757f1-174">string</span><span class="sxs-lookup"><span data-stu-id="757f1-174">string</span></span>|<span data-ttu-id="757f1-175">管理单元的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="757f1-175">Unique identifier for the administrative unit.</span></span> <span data-ttu-id="757f1-176">只读。</span><span class="sxs-lookup"><span data-stu-id="757f1-176">Read-only.</span></span>|
|<span data-ttu-id="757f1-177">visibility</span><span class="sxs-lookup"><span data-stu-id="757f1-177">visibility</span></span>|<span data-ttu-id="757f1-178">string</span><span class="sxs-lookup"><span data-stu-id="757f1-178">string</span></span>|<span data-ttu-id="757f1-179">控制管理单元及其成员是否为隐藏或公共的。</span><span class="sxs-lookup"><span data-stu-id="757f1-179">Controls whether the adminstrative unit and its members are hidden or public.</span></span> <span data-ttu-id="757f1-180">可以设置为 HiddenMembership 或 Public。</span><span class="sxs-lookup"><span data-stu-id="757f1-180">Can be set to HiddenMembership or Public.</span></span> <span data-ttu-id="757f1-181">如果未设置，则默认行为是公共行为。</span><span class="sxs-lookup"><span data-stu-id="757f1-181">If not set, default behavior is Public.</span></span> <span data-ttu-id="757f1-182">如果设置为 HiddenMembership，则只有管理单元的成员可以列出管理单位的其他成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-182">When set to HiddenMembership, only members of the administrative unit can list other members of the adminstrative unit.</span></span>|

## <a name="relationships"></a><span data-ttu-id="757f1-183">关系</span><span class="sxs-lookup"><span data-stu-id="757f1-183">Relationships</span></span>
| <span data-ttu-id="757f1-184">关系</span><span class="sxs-lookup"><span data-stu-id="757f1-184">Relationship</span></span> | <span data-ttu-id="757f1-185">类型</span><span class="sxs-lookup"><span data-stu-id="757f1-185">Type</span></span>   |<span data-ttu-id="757f1-186">说明</span><span class="sxs-lookup"><span data-stu-id="757f1-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="757f1-187">成员</span><span class="sxs-lookup"><span data-stu-id="757f1-187">members</span></span>|<span data-ttu-id="757f1-188">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="757f1-188">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="757f1-189">作为此 Adminsitrative 单位的成员的用户和组。</span><span class="sxs-lookup"><span data-stu-id="757f1-189">Users and groups that are members of this Adminsitrative Unit.</span></span> <span data-ttu-id="757f1-190">HTTP 方法：获取 (的列表成员) 、POST (添加成员) 、删除 (删除成员) 。</span><span class="sxs-lookup"><span data-stu-id="757f1-190">HTTP Methods: GET (list members), POST (add members), DELETE (remove members).</span></span>|
|<span data-ttu-id="757f1-191">scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="757f1-191">scopedRoleMembers</span></span>|<span data-ttu-id="757f1-192">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="757f1-192">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="757f1-193">此管理单元的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="757f1-193">Scoped-role members of this Administrative Unit.</span></span>  <span data-ttu-id="757f1-194">HTTP 方法： GET (list scopedRoleMemberships) ，POST (add scopedRoleMembership) ，DELETE (remove scopedRoleMembership) 。</span><span class="sxs-lookup"><span data-stu-id="757f1-194">HTTP Methods: GET (list scopedRoleMemberships), POST (add scopedRoleMembership), DELETE (remove scopedRoleMembership).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="757f1-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="757f1-195">JSON representation</span></span>

<span data-ttu-id="757f1-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="757f1-196">Here is a JSON representation of the resource.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="757f1-197">另请参阅</span><span class="sxs-lookup"><span data-stu-id="757f1-197">See also</span></span>

- [<span data-ttu-id="757f1-198">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="757f1-198">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="757f1-199">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="757f1-199">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="757f1-200">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="757f1-200">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
