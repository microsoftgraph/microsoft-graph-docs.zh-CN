---
title: accessPackage 资源类型
description: 访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e8603904e2a1cdb6315c1f7b5264e461cfdff09b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031786"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="aa8ac-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa8ac-103">accessPackage resource type</span></span>

<span data-ttu-id="aa8ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8ac-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="aa8ac-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="aa8ac-106">每个访问包都由一个访问包目录引用，并从该目录中的资源链接到来自定义该程序包提供的访问权限的特定于资源的角色作用域。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="aa8ac-107">访问包还链接到访问包分配策略，每个分配策略都定义了可以请求或分配访问包分配的成员。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="aa8ac-108">若要将用户分配到访问包，请 [创建一个](../api/accesspackageassignmentrequest-post.md) 引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="aa8ac-109">方法</span><span class="sxs-lookup"><span data-stu-id="aa8ac-109">Methods</span></span>

| <span data-ttu-id="aa8ac-110">方法</span><span class="sxs-lookup"><span data-stu-id="aa8ac-110">Method</span></span>       | <span data-ttu-id="aa8ac-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa8ac-111">Return Type</span></span> | <span data-ttu-id="aa8ac-112">说明</span><span class="sxs-lookup"><span data-stu-id="aa8ac-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="aa8ac-113">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="aa8ac-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="aa8ac-114">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8ac-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="aa8ac-115">检索 **accesspackage** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="aa8ac-116">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="aa8ac-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="aa8ac-118">创建新的 **accesspackage** 对象。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="aa8ac-119">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="aa8ac-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="aa8ac-121">读取 **accesspackage** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="aa8ac-122">更新 accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="aa8ac-123">无</span><span class="sxs-lookup"><span data-stu-id="aa8ac-123">None</span></span> | <span data-ttu-id="aa8ac-124">更新 **accesspackage** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="aa8ac-125">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="aa8ac-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="aa8ac-126">无</span><span class="sxs-lookup"><span data-stu-id="aa8ac-126">None</span></span> | <span data-ttu-id="aa8ac-127">删除 **accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="aa8ac-128">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="aa8ac-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="aa8ac-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8ac-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="aa8ac-130">检索此访问包的 **accessPackageResourceRoleScope** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="aa8ac-131">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="aa8ac-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="aa8ac-132">无</span><span class="sxs-lookup"><span data-stu-id="aa8ac-132">None</span></span> | <span data-ttu-id="aa8ac-133">为此访问包创建一个新的 **accessPackageResourceRoleScope** 对象。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa8ac-134">属性</span><span class="sxs-lookup"><span data-stu-id="aa8ac-134">Properties</span></span>

| <span data-ttu-id="aa8ac-135">属性</span><span class="sxs-lookup"><span data-stu-id="aa8ac-135">Property</span></span>     | <span data-ttu-id="aa8ac-136">类型</span><span class="sxs-lookup"><span data-stu-id="aa8ac-136">Type</span></span>        | <span data-ttu-id="aa8ac-137">说明</span><span class="sxs-lookup"><span data-stu-id="aa8ac-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa8ac-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="aa8ac-138">catalogId</span></span>|<span data-ttu-id="aa8ac-139">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-139">String</span></span>|<span data-ttu-id="aa8ac-140">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="aa8ac-141">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-141">Read-only.</span></span>|
|<span data-ttu-id="aa8ac-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="aa8ac-142">createdBy</span></span>|<span data-ttu-id="aa8ac-143">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-143">String</span></span>|<span data-ttu-id="aa8ac-144">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="aa8ac-145">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-145">Read-only.</span></span>|
|<span data-ttu-id="aa8ac-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa8ac-146">createdDateTime</span></span>|<span data-ttu-id="aa8ac-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8ac-147">DateTimeOffset</span></span>|<span data-ttu-id="aa8ac-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa8ac-149">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aa8ac-150">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-150">Read-only.</span></span>|
|<span data-ttu-id="aa8ac-151">说明</span><span class="sxs-lookup"><span data-stu-id="aa8ac-151">description</span></span>|<span data-ttu-id="aa8ac-152">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-152">String</span></span>|<span data-ttu-id="aa8ac-153">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-153">The description of the access package.</span></span>|
|<span data-ttu-id="aa8ac-154">displayName</span><span class="sxs-lookup"><span data-stu-id="aa8ac-154">displayName</span></span>|<span data-ttu-id="aa8ac-155">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-155">String</span></span>|<span data-ttu-id="aa8ac-156">访问包的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-156">The display name of the access package.</span></span>|
|<span data-ttu-id="aa8ac-157">id</span><span class="sxs-lookup"><span data-stu-id="aa8ac-157">id</span></span>|<span data-ttu-id="aa8ac-158">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-158">String</span></span>| <span data-ttu-id="aa8ac-159">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-159">Read-only.</span></span>|
|<span data-ttu-id="aa8ac-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="aa8ac-160">isHidden</span></span>|<span data-ttu-id="aa8ac-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa8ac-161">Boolean</span></span>|<span data-ttu-id="aa8ac-162">访问包是否在请求程序中是隐藏的。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="aa8ac-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="aa8ac-163">isRoleScopesVisible</span></span>|<span data-ttu-id="aa8ac-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa8ac-164">Boolean</span></span>|<span data-ttu-id="aa8ac-165">指示角色范围是否可见。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="aa8ac-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="aa8ac-166">modifiedBy</span></span>|<span data-ttu-id="aa8ac-167">String</span><span class="sxs-lookup"><span data-stu-id="aa8ac-167">String</span></span>|<span data-ttu-id="aa8ac-168">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="aa8ac-169">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-169">Read-only.</span></span>|
|<span data-ttu-id="aa8ac-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa8ac-170">modifiedDateTime</span></span>|<span data-ttu-id="aa8ac-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8ac-171">DateTimeOffset</span></span>|<span data-ttu-id="aa8ac-172">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa8ac-173">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-173">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aa8ac-174">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="aa8ac-175">关系</span><span class="sxs-lookup"><span data-stu-id="aa8ac-175">Relationships</span></span>

| <span data-ttu-id="aa8ac-176">关系</span><span class="sxs-lookup"><span data-stu-id="aa8ac-176">Relationship</span></span> | <span data-ttu-id="aa8ac-177">类型</span><span class="sxs-lookup"><span data-stu-id="aa8ac-177">Type</span></span>        | <span data-ttu-id="aa8ac-178">说明</span><span class="sxs-lookup"><span data-stu-id="aa8ac-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa8ac-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="aa8ac-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="aa8ac-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8ac-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="aa8ac-181">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-181">Read-only.</span></span> <span data-ttu-id="aa8ac-182">可为空。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-182">Nullable.</span></span>|
|<span data-ttu-id="aa8ac-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="aa8ac-183">accessPackageCatalog</span></span>|[<span data-ttu-id="aa8ac-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="aa8ac-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="aa8ac-185">只读。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-185">Read-only.</span></span> <span data-ttu-id="aa8ac-186">可为空。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-186">Nullable.</span></span>|
|<span data-ttu-id="aa8ac-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="aa8ac-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="aa8ac-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa8ac-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="aa8ac-189">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa8ac-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa8ac-190">JSON representation</span></span>

<span data-ttu-id="aa8ac-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa8ac-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
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


