---
title: accessPackage 资源类型
description: 访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a944309d59383b8c1501495c12d937acb13adbbb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870979"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="f0178-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0178-103">accessPackage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0178-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。</span><span class="sxs-lookup"><span data-stu-id="f0178-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="f0178-105">每个访问包都由一个访问包目录引用，并从该目录中的资源链接到来自定义该程序包提供的访问权限的特定于资源的角色作用域。</span><span class="sxs-lookup"><span data-stu-id="f0178-105">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="f0178-106">访问包还链接到访问包分配策略，每个分配策略都定义了可以请求或分配访问包分配的成员。</span><span class="sxs-lookup"><span data-stu-id="f0178-106">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="f0178-107">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="f0178-107">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="f0178-108">方法</span><span class="sxs-lookup"><span data-stu-id="f0178-108">Methods</span></span>

| <span data-ttu-id="f0178-109">方法</span><span class="sxs-lookup"><span data-stu-id="f0178-109">Method</span></span>       | <span data-ttu-id="f0178-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f0178-110">Return Type</span></span> | <span data-ttu-id="f0178-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0178-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f0178-112">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="f0178-112">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="f0178-113">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0178-113">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="f0178-114">检索**accesspackage**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f0178-114">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="f0178-115">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="f0178-115">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="f0178-116">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f0178-116">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="f0178-117">创建新的**accesspackage**对象。</span><span class="sxs-lookup"><span data-stu-id="f0178-117">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="f0178-118">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="f0178-118">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="f0178-119">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f0178-119">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="f0178-120">读取**accesspackage**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0178-120">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="f0178-121">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="f0178-121">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="f0178-122">无</span><span class="sxs-lookup"><span data-stu-id="f0178-122">None</span></span> | <span data-ttu-id="f0178-123">删除**accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="f0178-123">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="f0178-124">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="f0178-124">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="f0178-125">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0178-125">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="f0178-126">检索此访问包的**accessPackageResourceRoleScope**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f0178-126">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="f0178-127">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="f0178-127">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="f0178-128">无</span><span class="sxs-lookup"><span data-stu-id="f0178-128">None</span></span> | <span data-ttu-id="f0178-129">为此访问包创建一个新的**accessPackageResourceRoleScope**对象。</span><span class="sxs-lookup"><span data-stu-id="f0178-129">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="f0178-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0178-130">Properties</span></span>

| <span data-ttu-id="f0178-131">属性</span><span class="sxs-lookup"><span data-stu-id="f0178-131">Property</span></span>     | <span data-ttu-id="f0178-132">类型</span><span class="sxs-lookup"><span data-stu-id="f0178-132">Type</span></span>        | <span data-ttu-id="f0178-133">说明</span><span class="sxs-lookup"><span data-stu-id="f0178-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0178-134">catalogId</span><span class="sxs-lookup"><span data-stu-id="f0178-134">catalogId</span></span>|<span data-ttu-id="f0178-135">String</span><span class="sxs-lookup"><span data-stu-id="f0178-135">String</span></span>|<span data-ttu-id="f0178-136">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="f0178-136">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="f0178-137">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-137">Read-only.</span></span>|
|<span data-ttu-id="f0178-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="f0178-138">createdBy</span></span>|<span data-ttu-id="f0178-139">String</span><span class="sxs-lookup"><span data-stu-id="f0178-139">String</span></span>|<span data-ttu-id="f0178-140">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="f0178-140">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="f0178-141">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-141">Read-only.</span></span>|
|<span data-ttu-id="f0178-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0178-142">createdDateTime</span></span>|<span data-ttu-id="f0178-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0178-143">DateTimeOffset</span></span>|<span data-ttu-id="f0178-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f0178-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0178-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f0178-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f0178-146">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-146">Read-only.</span></span>|
|<span data-ttu-id="f0178-147">说明</span><span class="sxs-lookup"><span data-stu-id="f0178-147">description</span></span>|<span data-ttu-id="f0178-148">String</span><span class="sxs-lookup"><span data-stu-id="f0178-148">String</span></span>|<span data-ttu-id="f0178-149">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="f0178-149">The description of the access package.</span></span>|
|<span data-ttu-id="f0178-150">displayName</span><span class="sxs-lookup"><span data-stu-id="f0178-150">displayName</span></span>|<span data-ttu-id="f0178-151">String</span><span class="sxs-lookup"><span data-stu-id="f0178-151">String</span></span>|<span data-ttu-id="f0178-152">访问包的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f0178-152">The display name of the access package.</span></span>|
|<span data-ttu-id="f0178-153">id</span><span class="sxs-lookup"><span data-stu-id="f0178-153">id</span></span>|<span data-ttu-id="f0178-154">字符串</span><span class="sxs-lookup"><span data-stu-id="f0178-154">String</span></span>| <span data-ttu-id="f0178-155">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-155">Read-only.</span></span>|
|<span data-ttu-id="f0178-156">isHidden</span><span class="sxs-lookup"><span data-stu-id="f0178-156">isHidden</span></span>|<span data-ttu-id="f0178-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0178-157">Boolean</span></span>|<span data-ttu-id="f0178-158">访问包是否在请求程序中是隐藏的。</span><span class="sxs-lookup"><span data-stu-id="f0178-158">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="f0178-159">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="f0178-159">isRoleScopesVisible</span></span>|<span data-ttu-id="f0178-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0178-160">Boolean</span></span>|<span data-ttu-id="f0178-161">指示角色范围是否可见。</span><span class="sxs-lookup"><span data-stu-id="f0178-161">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="f0178-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="f0178-162">modifiedBy</span></span>|<span data-ttu-id="f0178-163">String</span><span class="sxs-lookup"><span data-stu-id="f0178-163">String</span></span>|<span data-ttu-id="f0178-164">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="f0178-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="f0178-165">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-165">Read-only.</span></span>|
|<span data-ttu-id="f0178-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0178-166">modifiedDateTime</span></span>|<span data-ttu-id="f0178-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0178-167">DateTimeOffset</span></span>|<span data-ttu-id="f0178-168">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f0178-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0178-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f0178-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f0178-170">只读。</span><span class="sxs-lookup"><span data-stu-id="f0178-170">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f0178-171">关系</span><span class="sxs-lookup"><span data-stu-id="f0178-171">Relationships</span></span>

| <span data-ttu-id="f0178-172">关系</span><span class="sxs-lookup"><span data-stu-id="f0178-172">Relationship</span></span> | <span data-ttu-id="f0178-173">类型</span><span class="sxs-lookup"><span data-stu-id="f0178-173">Type</span></span>        | <span data-ttu-id="f0178-174">说明</span><span class="sxs-lookup"><span data-stu-id="f0178-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f0178-175">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="f0178-175">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="f0178-176">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0178-176">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="f0178-177">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="f0178-177">Read-only.</span></span> <span data-ttu-id="f0178-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f0178-178">Nullable.</span></span>|
|<span data-ttu-id="f0178-179">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="f0178-179">accessPackageCatalog</span></span>|[<span data-ttu-id="f0178-180">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="f0178-180">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="f0178-181">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="f0178-181">Read-only.</span></span> <span data-ttu-id="f0178-182">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f0178-182">Nullable.</span></span>|
|<span data-ttu-id="f0178-183">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="f0178-183">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="f0178-184">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0178-184">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="f0178-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f0178-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0178-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0178-186">JSON representation</span></span>

<span data-ttu-id="f0178-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0178-187">The following is a JSON representation of the resource.</span></span>

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
