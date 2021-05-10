---
title: accessPackage 资源类型
description: 访问包定义资源角色的集合，以及一个或多个用户如何访问这些资源的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d288465b04986b98de7b67fa049657b8bcf0a58
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298529"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="a7450-103">accessPackage 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7450-103">accessPackage resource type</span></span>

<span data-ttu-id="a7450-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7450-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7450-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包定义资源角色的集合以及一个或多个用户可以如何访问这些资源的策略。</span><span class="sxs-lookup"><span data-stu-id="a7450-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  

<span data-ttu-id="a7450-106">每个访问包都由一个访问包目录引用，并且具有指向该目录中的资源的链接，这些资源通过定义包提供的访问的资源特定角色作用域。</span><span class="sxs-lookup"><span data-stu-id="a7450-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="a7450-107">访问包还会链接到访问包分配策略，其中每个策略定义可以请求或分配访问包分配的人。</span><span class="sxs-lookup"><span data-stu-id="a7450-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="a7450-108">若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="a7450-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="a7450-109">方法</span><span class="sxs-lookup"><span data-stu-id="a7450-109">Methods</span></span>

| <span data-ttu-id="a7450-110">方法</span><span class="sxs-lookup"><span data-stu-id="a7450-110">Method</span></span>       | <span data-ttu-id="a7450-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7450-111">Return Type</span></span> | <span data-ttu-id="a7450-112">说明</span><span class="sxs-lookup"><span data-stu-id="a7450-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a7450-113">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="a7450-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="a7450-114">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7450-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="a7450-115">检索 **accesspackage 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="a7450-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="a7450-116">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="a7450-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="a7450-118">创建新的 **accesspackage** 对象。</span><span class="sxs-lookup"><span data-stu-id="a7450-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="a7450-119">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="a7450-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="a7450-121">读取 **accesspackage 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="a7450-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="a7450-122">更新 accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="a7450-123">无</span><span class="sxs-lookup"><span data-stu-id="a7450-123">None</span></span> | <span data-ttu-id="a7450-124">更新 **accesspackage 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="a7450-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="a7450-125">删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="a7450-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="a7450-126">无</span><span class="sxs-lookup"><span data-stu-id="a7450-126">None</span></span> | <span data-ttu-id="a7450-127">删除 **accesspackage**。</span><span class="sxs-lookup"><span data-stu-id="a7450-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="a7450-128">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="a7450-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="a7450-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7450-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="a7450-130">检索此访问 **包的 accessPackageResourceRoleScope** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a7450-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="a7450-131">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="a7450-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="a7450-132">无</span><span class="sxs-lookup"><span data-stu-id="a7450-132">None</span></span> | <span data-ttu-id="a7450-133">为此访问 **包创建新的 accessPackageResourceRoleScope** 对象。</span><span class="sxs-lookup"><span data-stu-id="a7450-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |
|[<span data-ttu-id="a7450-134">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="a7450-134">filterByCurrentUser</span></span>](../api/accesspackage-filterbycurrentuser.md)|<span data-ttu-id="a7450-135">[accessPackage](../resources/accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7450-135">[accessPackage](../resources/accesspackage.md) collection</span></span>|<span data-ttu-id="a7450-136">检索在已登录用户上筛选的 **accessPackage** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a7450-136">Retrieve the list of **accessPackage** objects filtered on the signed-in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7450-137">属性</span><span class="sxs-lookup"><span data-stu-id="a7450-137">Properties</span></span>

| <span data-ttu-id="a7450-138">属性</span><span class="sxs-lookup"><span data-stu-id="a7450-138">Property</span></span>     | <span data-ttu-id="a7450-139">类型</span><span class="sxs-lookup"><span data-stu-id="a7450-139">Type</span></span>        | <span data-ttu-id="a7450-140">说明</span><span class="sxs-lookup"><span data-stu-id="a7450-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7450-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="a7450-141">catalogId</span></span>|<span data-ttu-id="a7450-142">String</span><span class="sxs-lookup"><span data-stu-id="a7450-142">String</span></span>|<span data-ttu-id="a7450-143">引用此访问包的访问包目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="a7450-143">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="a7450-144">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-144">Read-only.</span></span>|
|<span data-ttu-id="a7450-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="a7450-145">createdBy</span></span>|<span data-ttu-id="a7450-146">String</span><span class="sxs-lookup"><span data-stu-id="a7450-146">String</span></span>|<span data-ttu-id="a7450-147">创建此资源的主题的用户或标识的 UPN。</span><span class="sxs-lookup"><span data-stu-id="a7450-147">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="a7450-148">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-148">Read-only.</span></span>|
|<span data-ttu-id="a7450-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7450-149">createdDateTime</span></span>|<span data-ttu-id="a7450-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7450-150">DateTimeOffset</span></span>|<span data-ttu-id="a7450-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a7450-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a7450-152">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="a7450-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a7450-153">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-153">Read-only.</span></span>|
|<span data-ttu-id="a7450-154">说明</span><span class="sxs-lookup"><span data-stu-id="a7450-154">description</span></span>|<span data-ttu-id="a7450-155">String</span><span class="sxs-lookup"><span data-stu-id="a7450-155">String</span></span>|<span data-ttu-id="a7450-156">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="a7450-156">The description of the access package.</span></span>|
|<span data-ttu-id="a7450-157">displayName</span><span class="sxs-lookup"><span data-stu-id="a7450-157">displayName</span></span>|<span data-ttu-id="a7450-158">String</span><span class="sxs-lookup"><span data-stu-id="a7450-158">String</span></span>|<span data-ttu-id="a7450-159">访问显示名称的组。</span><span class="sxs-lookup"><span data-stu-id="a7450-159">The display name of the access package.</span></span>|
|<span data-ttu-id="a7450-160">id</span><span class="sxs-lookup"><span data-stu-id="a7450-160">id</span></span>|<span data-ttu-id="a7450-161">String</span><span class="sxs-lookup"><span data-stu-id="a7450-161">String</span></span>| <span data-ttu-id="a7450-162">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-162">Read-only.</span></span>|
|<span data-ttu-id="a7450-163">isHidden</span><span class="sxs-lookup"><span data-stu-id="a7450-163">isHidden</span></span>|<span data-ttu-id="a7450-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7450-164">Boolean</span></span>|<span data-ttu-id="a7450-165">访问包是否对请求程序隐藏。</span><span class="sxs-lookup"><span data-stu-id="a7450-165">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="a7450-166">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="a7450-166">isRoleScopesVisible</span></span>|<span data-ttu-id="a7450-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7450-167">Boolean</span></span>|<span data-ttu-id="a7450-168">指示角色作用域是否可见。</span><span class="sxs-lookup"><span data-stu-id="a7450-168">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="a7450-169">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="a7450-169">modifiedBy</span></span>|<span data-ttu-id="a7450-170">String</span><span class="sxs-lookup"><span data-stu-id="a7450-170">String</span></span>|<span data-ttu-id="a7450-171">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="a7450-171">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="a7450-172">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-172">Read-only.</span></span>|
|<span data-ttu-id="a7450-173">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7450-173">modifiedDateTime</span></span>|<span data-ttu-id="a7450-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7450-174">DateTimeOffset</span></span>|<span data-ttu-id="a7450-175">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a7450-175">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a7450-176">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="a7450-176">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a7450-177">只读。</span><span class="sxs-lookup"><span data-stu-id="a7450-177">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a7450-178">关系</span><span class="sxs-lookup"><span data-stu-id="a7450-178">Relationships</span></span>

| <span data-ttu-id="a7450-179">关系</span><span class="sxs-lookup"><span data-stu-id="a7450-179">Relationship</span></span> | <span data-ttu-id="a7450-180">类型</span><span class="sxs-lookup"><span data-stu-id="a7450-180">Type</span></span>        | <span data-ttu-id="a7450-181">说明</span><span class="sxs-lookup"><span data-stu-id="a7450-181">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7450-182">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="a7450-182">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="a7450-183">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7450-183">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="a7450-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="a7450-p107">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a7450-186">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a7450-186">accessPackageCatalog</span></span>|[<span data-ttu-id="a7450-187">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a7450-187">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="a7450-p108">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="a7450-p108">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a7450-190">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="a7450-190">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="a7450-191">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7450-191">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="a7450-192">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a7450-192">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7450-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7450-193">JSON representation</span></span>

<span data-ttu-id="a7450-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7450-194">The following is a JSON representation of the resource.</span></span>

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


