---
title: accessPackage 资源类型
description: 访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc08a1b92ccb8404a20cd5013be74d37f7659a5f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508567"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="3f657-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f657-103">accessPackage resource type</span></span>

<span data-ttu-id="3f657-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3f657-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f657-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。</span><span class="sxs-lookup"><span data-stu-id="3f657-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="3f657-106">每个访问包都由一个访问包目录引用，并从该目录中的资源链接到来自定义该程序包提供的访问权限的特定于资源的角色作用域。</span><span class="sxs-lookup"><span data-stu-id="3f657-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="3f657-107">访问包还链接到访问包分配策略，每个分配策略都定义了可以请求或分配访问包分配的成员。</span><span class="sxs-lookup"><span data-stu-id="3f657-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="3f657-108">若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。</span><span class="sxs-lookup"><span data-stu-id="3f657-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="3f657-109">方法</span><span class="sxs-lookup"><span data-stu-id="3f657-109">Methods</span></span>

| <span data-ttu-id="3f657-110">方法</span><span class="sxs-lookup"><span data-stu-id="3f657-110">Method</span></span>       | <span data-ttu-id="3f657-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f657-111">Return Type</span></span> | <span data-ttu-id="3f657-112">说明</span><span class="sxs-lookup"><span data-stu-id="3f657-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3f657-113">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="3f657-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="3f657-114">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f657-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="3f657-115">检索**accesspackage**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3f657-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="3f657-116">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="3f657-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="3f657-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="3f657-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="3f657-118">创建新的**accesspackage**对象。</span><span class="sxs-lookup"><span data-stu-id="3f657-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="3f657-119">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="3f657-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="3f657-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="3f657-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="3f657-121">读取**accesspackage**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f657-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="3f657-122">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="3f657-122">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="3f657-123">无</span><span class="sxs-lookup"><span data-stu-id="3f657-123">None</span></span> | <span data-ttu-id="3f657-124">删除**accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="3f657-124">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="3f657-125">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="3f657-125">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="3f657-126">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f657-126">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="3f657-127">检索此访问包的**accessPackageResourceRoleScope**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3f657-127">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="3f657-128">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="3f657-128">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="3f657-129">无</span><span class="sxs-lookup"><span data-stu-id="3f657-129">None</span></span> | <span data-ttu-id="3f657-130">为此访问包创建一个新的**accessPackageResourceRoleScope**对象。</span><span class="sxs-lookup"><span data-stu-id="3f657-130">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f657-131">属性</span><span class="sxs-lookup"><span data-stu-id="3f657-131">Properties</span></span>

| <span data-ttu-id="3f657-132">属性</span><span class="sxs-lookup"><span data-stu-id="3f657-132">Property</span></span>     | <span data-ttu-id="3f657-133">类型</span><span class="sxs-lookup"><span data-stu-id="3f657-133">Type</span></span>        | <span data-ttu-id="3f657-134">说明</span><span class="sxs-lookup"><span data-stu-id="3f657-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3f657-135">catalogId</span><span class="sxs-lookup"><span data-stu-id="3f657-135">catalogId</span></span>|<span data-ttu-id="3f657-136">String</span><span class="sxs-lookup"><span data-stu-id="3f657-136">String</span></span>|<span data-ttu-id="3f657-137">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f657-137">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="3f657-138">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-138">Read-only.</span></span>|
|<span data-ttu-id="3f657-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="3f657-139">createdBy</span></span>|<span data-ttu-id="3f657-140">String</span><span class="sxs-lookup"><span data-stu-id="3f657-140">String</span></span>|<span data-ttu-id="3f657-141">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="3f657-141">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="3f657-142">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-142">Read-only.</span></span>|
|<span data-ttu-id="3f657-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f657-143">createdDateTime</span></span>|<span data-ttu-id="3f657-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f657-144">DateTimeOffset</span></span>|<span data-ttu-id="3f657-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3f657-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f657-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="3f657-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3f657-147">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-147">Read-only.</span></span>|
|<span data-ttu-id="3f657-148">说明</span><span class="sxs-lookup"><span data-stu-id="3f657-148">description</span></span>|<span data-ttu-id="3f657-149">String</span><span class="sxs-lookup"><span data-stu-id="3f657-149">String</span></span>|<span data-ttu-id="3f657-150">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="3f657-150">The description of the access package.</span></span>|
|<span data-ttu-id="3f657-151">displayName</span><span class="sxs-lookup"><span data-stu-id="3f657-151">displayName</span></span>|<span data-ttu-id="3f657-152">String</span><span class="sxs-lookup"><span data-stu-id="3f657-152">String</span></span>|<span data-ttu-id="3f657-153">访问包的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3f657-153">The display name of the access package.</span></span>|
|<span data-ttu-id="3f657-154">id</span><span class="sxs-lookup"><span data-stu-id="3f657-154">id</span></span>|<span data-ttu-id="3f657-155">字符串</span><span class="sxs-lookup"><span data-stu-id="3f657-155">String</span></span>| <span data-ttu-id="3f657-156">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-156">Read-only.</span></span>|
|<span data-ttu-id="3f657-157">isHidden</span><span class="sxs-lookup"><span data-stu-id="3f657-157">isHidden</span></span>|<span data-ttu-id="3f657-158">布尔</span><span class="sxs-lookup"><span data-stu-id="3f657-158">Boolean</span></span>|<span data-ttu-id="3f657-159">访问包是否在请求程序中是隐藏的。</span><span class="sxs-lookup"><span data-stu-id="3f657-159">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="3f657-160">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="3f657-160">isRoleScopesVisible</span></span>|<span data-ttu-id="3f657-161">布尔</span><span class="sxs-lookup"><span data-stu-id="3f657-161">Boolean</span></span>|<span data-ttu-id="3f657-162">指示角色范围是否可见。</span><span class="sxs-lookup"><span data-stu-id="3f657-162">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="3f657-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="3f657-163">modifiedBy</span></span>|<span data-ttu-id="3f657-164">String</span><span class="sxs-lookup"><span data-stu-id="3f657-164">String</span></span>|<span data-ttu-id="3f657-165">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="3f657-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="3f657-166">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-166">Read-only.</span></span>|
|<span data-ttu-id="3f657-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f657-167">modifiedDateTime</span></span>|<span data-ttu-id="3f657-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f657-168">DateTimeOffset</span></span>|<span data-ttu-id="3f657-169">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3f657-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f657-170">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="3f657-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3f657-171">只读。</span><span class="sxs-lookup"><span data-stu-id="3f657-171">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f657-172">关系</span><span class="sxs-lookup"><span data-stu-id="3f657-172">Relationships</span></span>

| <span data-ttu-id="3f657-173">关系</span><span class="sxs-lookup"><span data-stu-id="3f657-173">Relationship</span></span> | <span data-ttu-id="3f657-174">类型</span><span class="sxs-lookup"><span data-stu-id="3f657-174">Type</span></span>        | <span data-ttu-id="3f657-175">说明</span><span class="sxs-lookup"><span data-stu-id="3f657-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3f657-176">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="3f657-176">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="3f657-177">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f657-177">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="3f657-178">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="3f657-178">Read-only.</span></span> <span data-ttu-id="3f657-179">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="3f657-179">Nullable.</span></span>|
|<span data-ttu-id="3f657-180">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3f657-180">accessPackageCatalog</span></span>|[<span data-ttu-id="3f657-181">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3f657-181">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="3f657-182">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="3f657-182">Read-only.</span></span> <span data-ttu-id="3f657-183">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="3f657-183">Nullable.</span></span>|
|<span data-ttu-id="3f657-184">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="3f657-184">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="3f657-185">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f657-185">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="3f657-186">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f657-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f657-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f657-187">JSON representation</span></span>

<span data-ttu-id="3f657-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f657-188">The following is a JSON representation of the resource.</span></span>

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
