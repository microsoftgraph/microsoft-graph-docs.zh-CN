---
title: accessPackage 资源类型
description: 访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d49ddfcc0db9b55701f0b84a223efcec85aa8dfe
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228063"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="94e4c-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="94e4c-103">accessPackage resource type</span></span>

<span data-ttu-id="94e4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e4c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="94e4c-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。</span><span class="sxs-lookup"><span data-stu-id="94e4c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="94e4c-106">每个访问包都由一个访问包目录引用，并从该目录中的资源链接到来自定义该程序包提供的访问权限的特定于资源的角色作用域。</span><span class="sxs-lookup"><span data-stu-id="94e4c-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="94e4c-107">访问包还链接到访问包分配策略，每个分配策略都定义了可以请求或分配访问包分配的成员。</span><span class="sxs-lookup"><span data-stu-id="94e4c-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="94e4c-108">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="94e4c-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="94e4c-109">方法</span><span class="sxs-lookup"><span data-stu-id="94e4c-109">Methods</span></span>

| <span data-ttu-id="94e4c-110">方法</span><span class="sxs-lookup"><span data-stu-id="94e4c-110">Method</span></span>       | <span data-ttu-id="94e4c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="94e4c-111">Return Type</span></span> | <span data-ttu-id="94e4c-112">说明</span><span class="sxs-lookup"><span data-stu-id="94e4c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="94e4c-113">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="94e4c-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="94e4c-114">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="94e4c-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="94e4c-115">检索**accesspackage**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="94e4c-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="94e4c-116">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="94e4c-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="94e4c-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="94e4c-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="94e4c-118">创建新的**accesspackage**对象。</span><span class="sxs-lookup"><span data-stu-id="94e4c-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="94e4c-119">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="94e4c-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="94e4c-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="94e4c-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="94e4c-121">读取**accesspackage**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94e4c-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="94e4c-122">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="94e4c-122">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="94e4c-123">无</span><span class="sxs-lookup"><span data-stu-id="94e4c-123">None</span></span> | <span data-ttu-id="94e4c-124">删除**accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="94e4c-124">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="94e4c-125">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="94e4c-125">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="94e4c-126">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="94e4c-126">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="94e4c-127">检索此访问包的**accessPackageResourceRoleScope**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="94e4c-127">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="94e4c-128">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="94e4c-128">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="94e4c-129">无</span><span class="sxs-lookup"><span data-stu-id="94e4c-129">None</span></span> | <span data-ttu-id="94e4c-130">为此访问包创建一个新的**accessPackageResourceRoleScope**对象。</span><span class="sxs-lookup"><span data-stu-id="94e4c-130">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="94e4c-131">属性</span><span class="sxs-lookup"><span data-stu-id="94e4c-131">Properties</span></span>

| <span data-ttu-id="94e4c-132">属性</span><span class="sxs-lookup"><span data-stu-id="94e4c-132">Property</span></span>     | <span data-ttu-id="94e4c-133">类型</span><span class="sxs-lookup"><span data-stu-id="94e4c-133">Type</span></span>        | <span data-ttu-id="94e4c-134">说明</span><span class="sxs-lookup"><span data-stu-id="94e4c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94e4c-135">catalogId</span><span class="sxs-lookup"><span data-stu-id="94e4c-135">catalogId</span></span>|<span data-ttu-id="94e4c-136">String</span><span class="sxs-lookup"><span data-stu-id="94e4c-136">String</span></span>|<span data-ttu-id="94e4c-137">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="94e4c-137">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="94e4c-138">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-138">Read-only.</span></span>|
|<span data-ttu-id="94e4c-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="94e4c-139">createdBy</span></span>|<span data-ttu-id="94e4c-140">String</span><span class="sxs-lookup"><span data-stu-id="94e4c-140">String</span></span>|<span data-ttu-id="94e4c-141">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="94e4c-141">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="94e4c-142">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-142">Read-only.</span></span>|
|<span data-ttu-id="94e4c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94e4c-143">createdDateTime</span></span>|<span data-ttu-id="94e4c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94e4c-144">DateTimeOffset</span></span>|<span data-ttu-id="94e4c-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="94e4c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94e4c-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="94e4c-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="94e4c-147">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-147">Read-only.</span></span>|
|<span data-ttu-id="94e4c-148">说明</span><span class="sxs-lookup"><span data-stu-id="94e4c-148">description</span></span>|<span data-ttu-id="94e4c-149">String</span><span class="sxs-lookup"><span data-stu-id="94e4c-149">String</span></span>|<span data-ttu-id="94e4c-150">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="94e4c-150">The description of the access package.</span></span>|
|<span data-ttu-id="94e4c-151">displayName</span><span class="sxs-lookup"><span data-stu-id="94e4c-151">displayName</span></span>|<span data-ttu-id="94e4c-152">String</span><span class="sxs-lookup"><span data-stu-id="94e4c-152">String</span></span>|<span data-ttu-id="94e4c-153">访问包的显示名称。</span><span class="sxs-lookup"><span data-stu-id="94e4c-153">The display name of the access package.</span></span>|
|<span data-ttu-id="94e4c-154">id</span><span class="sxs-lookup"><span data-stu-id="94e4c-154">id</span></span>|<span data-ttu-id="94e4c-155">字符串</span><span class="sxs-lookup"><span data-stu-id="94e4c-155">String</span></span>| <span data-ttu-id="94e4c-156">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-156">Read-only.</span></span>|
|<span data-ttu-id="94e4c-157">isHidden</span><span class="sxs-lookup"><span data-stu-id="94e4c-157">isHidden</span></span>|<span data-ttu-id="94e4c-158">布尔</span><span class="sxs-lookup"><span data-stu-id="94e4c-158">Boolean</span></span>|<span data-ttu-id="94e4c-159">访问包是否在请求程序中是隐藏的。</span><span class="sxs-lookup"><span data-stu-id="94e4c-159">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="94e4c-160">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="94e4c-160">isRoleScopesVisible</span></span>|<span data-ttu-id="94e4c-161">布尔</span><span class="sxs-lookup"><span data-stu-id="94e4c-161">Boolean</span></span>|<span data-ttu-id="94e4c-162">指示角色范围是否可见。</span><span class="sxs-lookup"><span data-stu-id="94e4c-162">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="94e4c-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="94e4c-163">modifiedBy</span></span>|<span data-ttu-id="94e4c-164">String</span><span class="sxs-lookup"><span data-stu-id="94e4c-164">String</span></span>|<span data-ttu-id="94e4c-165">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="94e4c-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="94e4c-166">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-166">Read-only.</span></span>|
|<span data-ttu-id="94e4c-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94e4c-167">modifiedDateTime</span></span>|<span data-ttu-id="94e4c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94e4c-168">DateTimeOffset</span></span>|<span data-ttu-id="94e4c-169">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="94e4c-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94e4c-170">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="94e4c-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="94e4c-171">只读。</span><span class="sxs-lookup"><span data-stu-id="94e4c-171">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="94e4c-172">关系</span><span class="sxs-lookup"><span data-stu-id="94e4c-172">Relationships</span></span>

| <span data-ttu-id="94e4c-173">关系</span><span class="sxs-lookup"><span data-stu-id="94e4c-173">Relationship</span></span> | <span data-ttu-id="94e4c-174">类型</span><span class="sxs-lookup"><span data-stu-id="94e4c-174">Type</span></span>        | <span data-ttu-id="94e4c-175">说明</span><span class="sxs-lookup"><span data-stu-id="94e4c-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94e4c-176">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="94e4c-176">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="94e4c-177">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="94e4c-177">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="94e4c-178">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="94e4c-178">Read-only.</span></span> <span data-ttu-id="94e4c-179">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="94e4c-179">Nullable.</span></span>|
|<span data-ttu-id="94e4c-180">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="94e4c-180">accessPackageCatalog</span></span>|[<span data-ttu-id="94e4c-181">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="94e4c-181">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="94e4c-182">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="94e4c-182">Read-only.</span></span> <span data-ttu-id="94e4c-183">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="94e4c-183">Nullable.</span></span>|
|<span data-ttu-id="94e4c-184">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="94e4c-184">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="94e4c-185">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="94e4c-185">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="94e4c-186">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="94e4c-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94e4c-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94e4c-187">JSON representation</span></span>

<span data-ttu-id="94e4c-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94e4c-188">The following is a JSON representation of the resource.</span></span>

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
