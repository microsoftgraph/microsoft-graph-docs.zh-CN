---
title: accessPackage 资源类型
description: 访问包定义资源角色的集合以及一个或多个用户如何访问这些资源的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 98e9a22137f9f6faaa39fbbb010a32b40f8f0254
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720835"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="7c3d2-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c3d2-103">accessPackage resource type</span></span>

<span data-ttu-id="7c3d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c3d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3d2-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包定义资源角色的集合以及一个或多个用户可以如何访问这些资源的策略。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="7c3d2-106">每个访问包都由单个访问包目录引用，并且具有通过定义包提供的访问的资源特定角色作用域从该目录访问资源的链接。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="7c3d2-107">访问包还链接到访问包分配策略，其中每个策略定义可以请求或分配访问包分配的人。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="7c3d2-108">若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="7c3d2-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="7c3d2-109">方法</span><span class="sxs-lookup"><span data-stu-id="7c3d2-109">Methods</span></span>

| <span data-ttu-id="7c3d2-110">方法</span><span class="sxs-lookup"><span data-stu-id="7c3d2-110">Method</span></span>       | <span data-ttu-id="7c3d2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c3d2-111">Return Type</span></span> | <span data-ttu-id="7c3d2-112">说明</span><span class="sxs-lookup"><span data-stu-id="7c3d2-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7c3d2-113">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="7c3d2-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="7c3d2-114">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c3d2-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="7c3d2-115">检索 **accesspackage 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="7c3d2-116">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="7c3d2-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="7c3d2-118">创建新的 **accesspackage** 对象。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="7c3d2-119">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="7c3d2-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="7c3d2-121">读取 **accesspackage 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="7c3d2-122">更新 accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="7c3d2-123">无</span><span class="sxs-lookup"><span data-stu-id="7c3d2-123">None</span></span> | <span data-ttu-id="7c3d2-124">更新 **accesspackage** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="7c3d2-125">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="7c3d2-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="7c3d2-126">无</span><span class="sxs-lookup"><span data-stu-id="7c3d2-126">None</span></span> | <span data-ttu-id="7c3d2-127">删除 **accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="7c3d2-128">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="7c3d2-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="7c3d2-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c3d2-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="7c3d2-130">检索此访问 **包的 accessPackageResourceRoleScope** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="7c3d2-131">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="7c3d2-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="7c3d2-132">无</span><span class="sxs-lookup"><span data-stu-id="7c3d2-132">None</span></span> | <span data-ttu-id="7c3d2-133">为此访问 **包创建新的 accessPackageResourceRoleScope** 对象。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c3d2-134">属性</span><span class="sxs-lookup"><span data-stu-id="7c3d2-134">Properties</span></span>

| <span data-ttu-id="7c3d2-135">属性</span><span class="sxs-lookup"><span data-stu-id="7c3d2-135">Property</span></span>     | <span data-ttu-id="7c3d2-136">类型</span><span class="sxs-lookup"><span data-stu-id="7c3d2-136">Type</span></span>        | <span data-ttu-id="7c3d2-137">说明</span><span class="sxs-lookup"><span data-stu-id="7c3d2-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c3d2-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="7c3d2-138">catalogId</span></span>|<span data-ttu-id="7c3d2-139">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-139">String</span></span>|<span data-ttu-id="7c3d2-140">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="7c3d2-141">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-141">Read-only.</span></span>|
|<span data-ttu-id="7c3d2-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c3d2-142">createdBy</span></span>|<span data-ttu-id="7c3d2-143">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-143">String</span></span>|<span data-ttu-id="7c3d2-144">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="7c3d2-145">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-145">Read-only.</span></span>|
|<span data-ttu-id="7c3d2-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c3d2-146">createdDateTime</span></span>|<span data-ttu-id="7c3d2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c3d2-147">DateTimeOffset</span></span>|<span data-ttu-id="7c3d2-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c3d2-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="7c3d2-150">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-150">Read-only.</span></span>|
|<span data-ttu-id="7c3d2-151">说明</span><span class="sxs-lookup"><span data-stu-id="7c3d2-151">description</span></span>|<span data-ttu-id="7c3d2-152">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-152">String</span></span>|<span data-ttu-id="7c3d2-153">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-153">The description of the access package.</span></span>|
|<span data-ttu-id="7c3d2-154">displayName</span><span class="sxs-lookup"><span data-stu-id="7c3d2-154">displayName</span></span>|<span data-ttu-id="7c3d2-155">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-155">String</span></span>|<span data-ttu-id="7c3d2-156">访问显示名称的组。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-156">The display name of the access package.</span></span>|
|<span data-ttu-id="7c3d2-157">id</span><span class="sxs-lookup"><span data-stu-id="7c3d2-157">id</span></span>|<span data-ttu-id="7c3d2-158">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-158">String</span></span>| <span data-ttu-id="7c3d2-159">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-159">Read-only.</span></span>|
|<span data-ttu-id="7c3d2-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="7c3d2-160">isHidden</span></span>|<span data-ttu-id="7c3d2-161">布尔</span><span class="sxs-lookup"><span data-stu-id="7c3d2-161">Boolean</span></span>|<span data-ttu-id="7c3d2-162">访问包是否对请求程序隐藏。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="7c3d2-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="7c3d2-163">isRoleScopesVisible</span></span>|<span data-ttu-id="7c3d2-164">布尔</span><span class="sxs-lookup"><span data-stu-id="7c3d2-164">Boolean</span></span>|<span data-ttu-id="7c3d2-165">指示角色作用域是否可见。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="7c3d2-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="7c3d2-166">modifiedBy</span></span>|<span data-ttu-id="7c3d2-167">String</span><span class="sxs-lookup"><span data-stu-id="7c3d2-167">String</span></span>|<span data-ttu-id="7c3d2-168">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="7c3d2-169">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-169">Read-only.</span></span>|
|<span data-ttu-id="7c3d2-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c3d2-170">modifiedDateTime</span></span>|<span data-ttu-id="7c3d2-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c3d2-171">DateTimeOffset</span></span>|<span data-ttu-id="7c3d2-172">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c3d2-173">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="7c3d2-174">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7c3d2-175">关系</span><span class="sxs-lookup"><span data-stu-id="7c3d2-175">Relationships</span></span>

| <span data-ttu-id="7c3d2-176">关系</span><span class="sxs-lookup"><span data-stu-id="7c3d2-176">Relationship</span></span> | <span data-ttu-id="7c3d2-177">类型</span><span class="sxs-lookup"><span data-stu-id="7c3d2-177">Type</span></span>        | <span data-ttu-id="7c3d2-178">说明</span><span class="sxs-lookup"><span data-stu-id="7c3d2-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c3d2-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="7c3d2-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="7c3d2-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c3d2-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="7c3d2-181">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-181">Read-only.</span></span> <span data-ttu-id="7c3d2-182">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-182">Nullable.</span></span>|
|<span data-ttu-id="7c3d2-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c3d2-183">accessPackageCatalog</span></span>|[<span data-ttu-id="7c3d2-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c3d2-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="7c3d2-185">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-185">Read-only.</span></span> <span data-ttu-id="7c3d2-186">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-186">Nullable.</span></span>|
|<span data-ttu-id="7c3d2-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="7c3d2-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="7c3d2-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c3d2-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="7c3d2-189">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c3d2-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c3d2-190">JSON representation</span></span>

<span data-ttu-id="7c3d2-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c3d2-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


