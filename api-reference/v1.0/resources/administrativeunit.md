---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5ff1e4a5915487837ab7db25d2acefa3fafb4ad5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448875"
---
# <a name="administrativeunit-resource-type"></a><span data-ttu-id="145b5-103">administrativeUnit 资源类型</span><span class="sxs-lookup"><span data-stu-id="145b5-103">administrativeUnit resource type</span></span>

<span data-ttu-id="145b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="145b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="145b5-105">管理单元为用户和组目录对象提供概念容器。</span><span class="sxs-lookup"><span data-stu-id="145b5-105">An administrative unit provides a conceptual container for User and Group directory objects.</span></span> <span data-ttu-id="145b5-106">通过使用管理单元，公司管理员可以将管理责任委派给区域管理员或部门管理员，以管理包含在管理单元内或作用域内的用户和组。</span><span class="sxs-lookup"><span data-stu-id="145b5-106">Using administrative units, a company administrator can now delegate administrative responsibilities to manage the users and groups contained within or scoped to an administrative unit to a regional or departmental administrator.</span></span>

<span data-ttu-id="145b5-107">来看一个示例。</span><span class="sxs-lookup"><span data-stu-id="145b5-107">Let's look at an example.</span></span> <span data-ttu-id="145b5-108">假设 Contoso Corp 由两个部门（一个"西陆岛"分部和一个"东部经济区"部门）所决定。</span><span class="sxs-lookup"><span data-stu-id="145b5-108">Imagine that Contoso Corp is made up of two divisions - a West Coast Division and an East Coast Division.</span></span> <span data-ttu-id="145b5-109">Contoso 的目录角色的范围为整个租户。</span><span class="sxs-lookup"><span data-stu-id="145b5-109">Directory roles at Contoso are scoped to the entire tenant.</span></span> <span data-ttu-id="145b5-110">Contoso 公司管理员 Lee 想要委派管理职责，但将其范围缩小到"西陆岛"部门或"东部经济区"部门。</span><span class="sxs-lookup"><span data-stu-id="145b5-110">Lee, a Contoso company administrator, wants to delegate administrative responsibilities, but scope them to the West Coast Division or the East Coast division.</span></span>  <span data-ttu-id="145b5-111">小王可以创建 *一个"西陆岛"管理单元* ，并可以将所有"西陆"用户放入此管理单元中。</span><span class="sxs-lookup"><span data-stu-id="145b5-111">Lee can create a *West Coast admistrative unit* and place all West Coast users into this administrative unit.</span></span>  <span data-ttu-id="145b5-112">同样，小王可以创建 *一个东部经济区管理单元*。</span><span class="sxs-lookup"><span data-stu-id="145b5-112">Similarly, Lee can create an *East Coast adminstrative unit*.</span></span>  <span data-ttu-id="145b5-113">现在，Lee 可以开始将管理职责委派给其他人，但范围是自己创建的新管理单元。</span><span class="sxs-lookup"><span data-stu-id="145b5-113">Now Lee, can start delegating administrative responsibilities to others, but **scoped** to the new administrative units he's created.</span></span> <span data-ttu-id="145b5-114">小王将 Jennifer设置在一个范围为"西陆"管理单元的支持 *人员管理员角色中*。</span><span class="sxs-lookup"><span data-stu-id="145b5-114">Lee places Jennifer in a *helpdesk administrator* role **scoped** to the *West Coast administrative unit*.</span></span>  <span data-ttu-id="145b5-115">这允许 Jennifer 重置任何用户的密码，但只有在这些用户位于"西陆岛"管理单元 *中时。*</span><span class="sxs-lookup"><span data-stu-id="145b5-115">This allows Jennifer to reset any user's password, but only if those users are in the *West Coast administrative unit*.</span></span>  <span data-ttu-id="145b5-116">同样，小王将 Dave 设置在一个用户帐户 *管理员* 角色中，该角色的作用范围是"*东部经济区"管理单元*。</span><span class="sxs-lookup"><span data-stu-id="145b5-116">Similarly, Lee places Dave in a *user account administrator* role **scoped** to the *East Coast administrative unit*.</span></span>  <span data-ttu-id="145b5-117">这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但只有在这些用户位于东部行政区管理单元 *中时。*</span><span class="sxs-lookup"><span data-stu-id="145b5-117">This allows Dave to update users, assign licenses and reset any user's password, but only if those users are in the *East Coast administrative unit*.</span></span> <span data-ttu-id="145b5-118">有关视频概述，请参阅 [Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。</span><span class="sxs-lookup"><span data-stu-id="145b5-118">For a video overview, please see [Introduction to Azure Active Directory Administrative Units](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).</span></span>


<span data-ttu-id="145b5-119">本主题提供 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。</span><span class="sxs-lookup"><span data-stu-id="145b5-119">This topic provides descriptions of the declared properties and navigation properties exposed by the administrativeUnit entity, as well as the operations and functions that can be called on the administrativeUnits resource.</span></span>


## <a name="methods"></a><span data-ttu-id="145b5-120">Methods</span><span class="sxs-lookup"><span data-stu-id="145b5-120">Methods</span></span>

| <span data-ttu-id="145b5-121">方法</span><span class="sxs-lookup"><span data-stu-id="145b5-121">Method</span></span>   | <span data-ttu-id="145b5-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="145b5-122">Return Type</span></span> | <span data-ttu-id="145b5-123">说明</span><span class="sxs-lookup"><span data-stu-id="145b5-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="145b5-124">创建</span><span class="sxs-lookup"><span data-stu-id="145b5-124">Create</span></span>](../api/administrativeunit-post-administrativeunits.md) | [<span data-ttu-id="145b5-125">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="145b5-125">administrativeUnit</span></span>](administrativeunit.md) | <span data-ttu-id="145b5-126">创建新的管理单元。</span><span class="sxs-lookup"><span data-stu-id="145b5-126">Create a new administrative unit.</span></span>|
|[<span data-ttu-id="145b5-127">List</span><span class="sxs-lookup"><span data-stu-id="145b5-127">List</span></span>](../api/administrativeunit-list.md) | <span data-ttu-id="145b5-128">[administrativeUnit](administrativeunit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="145b5-128">[administrativeUnit](administrativeunit.md) collection</span></span> |<span data-ttu-id="145b5-129">列出所有 administrativeUnits 的属性。</span><span class="sxs-lookup"><span data-stu-id="145b5-129">List properties of all administrativeUnits.</span></span>|
|[<span data-ttu-id="145b5-130">获取</span><span class="sxs-lookup"><span data-stu-id="145b5-130">Get</span></span>](../api/administrativeunit-get.md) | [<span data-ttu-id="145b5-131">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="145b5-131">administrativeUnit</span></span>](administrativeunit.md) |<span data-ttu-id="145b5-132">读取特定 administrativeUnit 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="145b5-132">Read properties and relationships of a specific administrativeUnit object.</span></span>|
|[<span data-ttu-id="145b5-133">更新</span><span class="sxs-lookup"><span data-stu-id="145b5-133">Update</span></span>](../api/administrativeunit-update.md) | [<span data-ttu-id="145b5-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="145b5-134">administrativeUnit</span></span>](administrativeunit.md)    |<span data-ttu-id="145b5-135">更新 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="145b5-135">Update administrativeUnit object.</span></span> |
|[<span data-ttu-id="145b5-136">删除</span><span class="sxs-lookup"><span data-stu-id="145b5-136">Delete</span></span>](../api/administrativeunit-delete.md) | <span data-ttu-id="145b5-137">无</span><span class="sxs-lookup"><span data-stu-id="145b5-137">None</span></span> |<span data-ttu-id="145b5-138">删除 administrativeUnit 对象。</span><span class="sxs-lookup"><span data-stu-id="145b5-138">Delete administrativeUnit object.</span></span> |
|[<span data-ttu-id="145b5-139">添加成员</span><span class="sxs-lookup"><span data-stu-id="145b5-139">Add a member</span></span>](../api/administrativeunit-post-members.md) |[<span data-ttu-id="145b5-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="145b5-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="145b5-141">在用户或 (中添加成员) 。</span><span class="sxs-lookup"><span data-stu-id="145b5-141">Add a member (user or group).</span></span>|
|[<span data-ttu-id="145b5-142">List members</span><span class="sxs-lookup"><span data-stu-id="145b5-142">List members</span></span>](../api/administrativeunit-list-members.md) |<span data-ttu-id="145b5-143">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="145b5-143">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="145b5-144">获取用户和 (组) 列表。</span><span class="sxs-lookup"><span data-stu-id="145b5-144">Get the list of (user and group) members.</span></span>|
|[<span data-ttu-id="145b5-145">获取成员</span><span class="sxs-lookup"><span data-stu-id="145b5-145">Get a member</span></span>](../api/administrativeunit-get-members.md) |[<span data-ttu-id="145b5-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="145b5-146">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="145b5-147">获取特定成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-147">Get a specific member.</span></span>|
|[<span data-ttu-id="145b5-148">删除成员</span><span class="sxs-lookup"><span data-stu-id="145b5-148">Remove a member</span></span>](../api/administrativeunit-delete-members.md) |[<span data-ttu-id="145b5-149">directoryObject</span><span class="sxs-lookup"><span data-stu-id="145b5-149">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="145b5-150">删除成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-150">Remove a member.</span></span>|
|[<span data-ttu-id="145b5-151">添加作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="145b5-151">Add scoped-role member</span></span>](../api/administrativeunit-post-scopedrolemembers.md) |[<span data-ttu-id="145b5-152">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="145b5-152">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="145b5-153">添加作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-153">Add a scoped-role member.</span></span>|
|[<span data-ttu-id="145b5-154">列出作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="145b5-154">List scoped-role members</span></span>](../api/administrativeunit-list-scopedrolemembers.md) |<span data-ttu-id="145b5-155">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="145b5-155">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="145b5-156">获取作用域角色管理员的列表。</span><span class="sxs-lookup"><span data-stu-id="145b5-156">Get the list of scoped-role administrators.</span></span>|
|[<span data-ttu-id="145b5-157">获取作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="145b5-157">Get a scoped-role member</span></span>](../api/administrativeunit-get-scopedrolemembers.md) |[<span data-ttu-id="145b5-158">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="145b5-158">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="145b5-159">获取特定作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-159">Get a specific scoped-role member.</span></span>|
|[<span data-ttu-id="145b5-160">删除作用域角色成员</span><span class="sxs-lookup"><span data-stu-id="145b5-160">Remove a scoped-role member</span></span>](../api/administrativeunit-delete-scopedrolemembers.md) |[<span data-ttu-id="145b5-161">scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="145b5-161">scopedRoleMembership</span></span>](scopedrolemembership.md)| <span data-ttu-id="145b5-162">删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-162">Remove a scoped-role member.</span></span>|

## <a name="properties"></a><span data-ttu-id="145b5-163">属性</span><span class="sxs-lookup"><span data-stu-id="145b5-163">Properties</span></span>
| <span data-ttu-id="145b5-164">属性</span><span class="sxs-lookup"><span data-stu-id="145b5-164">Property</span></span>     | <span data-ttu-id="145b5-165">类型</span><span class="sxs-lookup"><span data-stu-id="145b5-165">Type</span></span>   |<span data-ttu-id="145b5-166">说明</span><span class="sxs-lookup"><span data-stu-id="145b5-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="145b5-167">说明</span><span class="sxs-lookup"><span data-stu-id="145b5-167">description</span></span>|<span data-ttu-id="145b5-168">string</span><span class="sxs-lookup"><span data-stu-id="145b5-168">string</span></span>|<span data-ttu-id="145b5-169">管理单元的可选说明。</span><span class="sxs-lookup"><span data-stu-id="145b5-169">An optional description for the administrative unit.</span></span>|
|<span data-ttu-id="145b5-170">displayName</span><span class="sxs-lookup"><span data-stu-id="145b5-170">displayName</span></span>|<span data-ttu-id="145b5-171">string</span><span class="sxs-lookup"><span data-stu-id="145b5-171">string</span></span>|<span data-ttu-id="145b5-172">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="145b5-172">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="145b5-173">id</span><span class="sxs-lookup"><span data-stu-id="145b5-173">id</span></span>|<span data-ttu-id="145b5-174">string</span><span class="sxs-lookup"><span data-stu-id="145b5-174">string</span></span>|<span data-ttu-id="145b5-175">管理单元的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="145b5-175">Unique identifier for the administrative unit.</span></span> <span data-ttu-id="145b5-176">只读。</span><span class="sxs-lookup"><span data-stu-id="145b5-176">Read-only.</span></span>|
|<span data-ttu-id="145b5-177">visibility</span><span class="sxs-lookup"><span data-stu-id="145b5-177">visibility</span></span>|<span data-ttu-id="145b5-178">string</span><span class="sxs-lookup"><span data-stu-id="145b5-178">string</span></span>|<span data-ttu-id="145b5-179">控制管理单元及其成员是隐藏还是公开。</span><span class="sxs-lookup"><span data-stu-id="145b5-179">Controls whether the administrative unit and its members are hidden or public.</span></span> <span data-ttu-id="145b5-180">可以设置为或 `HiddenMembership` `Public` 。</span><span class="sxs-lookup"><span data-stu-id="145b5-180">Can be set to `HiddenMembership` or `Public`.</span></span> <span data-ttu-id="145b5-181">如果未设置，默认行为为 Public。</span><span class="sxs-lookup"><span data-stu-id="145b5-181">If not set, default behavior is Public.</span></span> <span data-ttu-id="145b5-182">设置为 HiddenMembership 时，只有管理单元的成员才能列出管理单元的其他成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-182">When set to HiddenMembership, only members of the administrative unit can list other members of the adminstrative unit.</span></span>|

## <a name="relationships"></a><span data-ttu-id="145b5-183">关系</span><span class="sxs-lookup"><span data-stu-id="145b5-183">Relationships</span></span>
| <span data-ttu-id="145b5-184">关系</span><span class="sxs-lookup"><span data-stu-id="145b5-184">Relationship</span></span> | <span data-ttu-id="145b5-185">类型</span><span class="sxs-lookup"><span data-stu-id="145b5-185">Type</span></span>   |<span data-ttu-id="145b5-186">说明</span><span class="sxs-lookup"><span data-stu-id="145b5-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="145b5-187">成员</span><span class="sxs-lookup"><span data-stu-id="145b5-187">members</span></span>|<span data-ttu-id="145b5-188">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="145b5-188">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="145b5-189">是此管理单元的成员的用户和组。</span><span class="sxs-lookup"><span data-stu-id="145b5-189">Users and groups that are members of this Adminsitrative Unit.</span></span> <span data-ttu-id="145b5-190">HTTP 方法：get (list members) ， POST (add members) ， DELETE (remove members) .</span><span class="sxs-lookup"><span data-stu-id="145b5-190">HTTP Methods: GET (list members), POST (add members), DELETE (remove members).</span></span>|
|<span data-ttu-id="145b5-191">scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="145b5-191">scopedRoleMembers</span></span>|<span data-ttu-id="145b5-192">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="145b5-192">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="145b5-193">此管理单元的作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="145b5-193">Scoped-role members of this Administrative Unit.</span></span>  <span data-ttu-id="145b5-194">HTTP 方法：GET (list scopedRoleMemberships) ， POST (add scopedRoleMembership) ， DELETE (remove scopedRoleMembership) 。</span><span class="sxs-lookup"><span data-stu-id="145b5-194">HTTP Methods: GET (list scopedRoleMemberships), POST (add scopedRoleMembership), DELETE (remove scopedRoleMembership).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="145b5-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="145b5-195">JSON representation</span></span>

<span data-ttu-id="145b5-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="145b5-196">Here is a JSON representation of the resource.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="145b5-197">另请参阅</span><span class="sxs-lookup"><span data-stu-id="145b5-197">See also</span></span>

- [<span data-ttu-id="145b5-198">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="145b5-198">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="145b5-199">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="145b5-199">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="145b5-200">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="145b5-200">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
