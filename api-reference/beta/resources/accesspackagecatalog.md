---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 051657b5c8c7edb51a4c2c5c3a15bf3740052b86
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351095"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="4300d-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="4300d-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="4300d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4300d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4300d-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包目录是零个或多个访问包的容器。</span><span class="sxs-lookup"><span data-stu-id="4300d-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span> <span data-ttu-id="4300d-106">访问包目录还可能包含链接的资源，这些资源用于这些访问包中以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="4300d-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span> <span data-ttu-id="4300d-107">若要查看或更改目录作用域角色的成员身份，请使用角色分配 [API](unifiedroleassignment.md) 和权利管理 RBAC 提供程序。</span><span class="sxs-lookup"><span data-stu-id="4300d-107">To view or change the membership of catalog-scoped roles, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>



## <a name="methods"></a><span data-ttu-id="4300d-108">方法</span><span class="sxs-lookup"><span data-stu-id="4300d-108">Methods</span></span>

| <span data-ttu-id="4300d-109">方法</span><span class="sxs-lookup"><span data-stu-id="4300d-109">Method</span></span>       | <span data-ttu-id="4300d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4300d-110">Return Type</span></span> | <span data-ttu-id="4300d-111">说明</span><span class="sxs-lookup"><span data-stu-id="4300d-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4300d-112">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="4300d-112">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="4300d-113">[accessPackageCatalog](accesspackagecatalog.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4300d-113">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="4300d-114">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4300d-114">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="4300d-115">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-115">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="4300d-116">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-116">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="4300d-117">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="4300d-117">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="4300d-118">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-118">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="4300d-119">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-119">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="4300d-120">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4300d-120">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="4300d-121">更新 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-121">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="4300d-122">无</span><span class="sxs-lookup"><span data-stu-id="4300d-122">None</span></span> | <span data-ttu-id="4300d-123">更新 accessPackageCatalog 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4300d-123">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="4300d-124">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="4300d-124">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="4300d-125">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="4300d-125">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="4300d-126">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="4300d-126">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="4300d-127">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4300d-127">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="4300d-128">检索目录中的 accessPackageResource 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4300d-128">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="4300d-129">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="4300d-129">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="4300d-130">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4300d-130">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="4300d-131">检索目录中资源的 accessPackageResourceRole 对象列表。</span><span class="sxs-lookup"><span data-stu-id="4300d-131">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="4300d-132">属性</span><span class="sxs-lookup"><span data-stu-id="4300d-132">Properties</span></span>

| <span data-ttu-id="4300d-133">属性</span><span class="sxs-lookup"><span data-stu-id="4300d-133">Property</span></span>     | <span data-ttu-id="4300d-134">类型</span><span class="sxs-lookup"><span data-stu-id="4300d-134">Type</span></span>        | <span data-ttu-id="4300d-135">说明</span><span class="sxs-lookup"><span data-stu-id="4300d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4300d-136">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="4300d-136">catalogStatus</span></span>|<span data-ttu-id="4300d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-137">String</span></span>|<span data-ttu-id="4300d-138">如果访问 `Published` 包可用于管理，则具有 值。</span><span class="sxs-lookup"><span data-stu-id="4300d-138">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="4300d-139">catalogType</span><span class="sxs-lookup"><span data-stu-id="4300d-139">catalogType</span></span>|<span data-ttu-id="4300d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-140">String</span></span>|<span data-ttu-id="4300d-141">或 `UserManaged` `ServiceDefault` 之一。</span><span class="sxs-lookup"><span data-stu-id="4300d-141">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="4300d-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="4300d-142">createdBy</span></span>|<span data-ttu-id="4300d-143">String</span><span class="sxs-lookup"><span data-stu-id="4300d-143">String</span></span>|<span data-ttu-id="4300d-144">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4300d-144">UPN of the user who created this resource.</span></span> <span data-ttu-id="4300d-145">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-145">Read-only.</span></span>|
|<span data-ttu-id="4300d-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4300d-146">createdDateTime</span></span>|<span data-ttu-id="4300d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4300d-147">DateTimeOffset</span></span>|<span data-ttu-id="4300d-148">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4300d-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4300d-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="4300d-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4300d-150">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-150">Read-only.</span></span>|
|<span data-ttu-id="4300d-151">说明</span><span class="sxs-lookup"><span data-stu-id="4300d-151">description</span></span>|<span data-ttu-id="4300d-152">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-152">String</span></span>|<span data-ttu-id="4300d-153">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="4300d-153">The description of the access package catalog.</span></span>|
|<span data-ttu-id="4300d-154">displayName</span><span class="sxs-lookup"><span data-stu-id="4300d-154">displayName</span></span>|<span data-ttu-id="4300d-155">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-155">String</span></span>|<span data-ttu-id="4300d-156">访问显示名称目录的索引。</span><span class="sxs-lookup"><span data-stu-id="4300d-156">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="4300d-157">id</span><span class="sxs-lookup"><span data-stu-id="4300d-157">id</span></span>|<span data-ttu-id="4300d-158">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-158">String</span></span>| <span data-ttu-id="4300d-159">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-159">Read-only.</span></span>|
|<span data-ttu-id="4300d-160">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="4300d-160">isExternallyVisible</span></span>|<span data-ttu-id="4300d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4300d-161">Boolean</span></span>|<span data-ttu-id="4300d-162">租户外部的用户是否可以请求此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="4300d-162">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="4300d-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="4300d-163">modifiedBy</span></span>|<span data-ttu-id="4300d-164">字符串</span><span class="sxs-lookup"><span data-stu-id="4300d-164">String</span></span>|<span data-ttu-id="4300d-165">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4300d-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="4300d-166">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-166">Read-only.</span></span>|
|<span data-ttu-id="4300d-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4300d-167">modifiedDateTime</span></span>|<span data-ttu-id="4300d-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4300d-168">DateTimeOffset</span></span>|<span data-ttu-id="4300d-169">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4300d-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4300d-170">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="4300d-170">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="4300d-171">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-171">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="4300d-172">关系</span><span class="sxs-lookup"><span data-stu-id="4300d-172">Relationships</span></span>

| <span data-ttu-id="4300d-173">关系</span><span class="sxs-lookup"><span data-stu-id="4300d-173">Relationship</span></span> | <span data-ttu-id="4300d-174">类型</span><span class="sxs-lookup"><span data-stu-id="4300d-174">Type</span></span>        | <span data-ttu-id="4300d-175">说明</span><span class="sxs-lookup"><span data-stu-id="4300d-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4300d-176">accessPackages</span><span class="sxs-lookup"><span data-stu-id="4300d-176">accessPackages</span></span>|<span data-ttu-id="4300d-177">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4300d-177">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="4300d-178">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="4300d-178">The access packages in this catalog.</span></span> <span data-ttu-id="4300d-179">只读。</span><span class="sxs-lookup"><span data-stu-id="4300d-179">Read-only.</span></span> <span data-ttu-id="4300d-180">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4300d-180">Nullable.</span></span>|
|<span data-ttu-id="4300d-181">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="4300d-181">accessPackageResources</span></span>|<span data-ttu-id="4300d-182">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4300d-182">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="4300d-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4300d-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4300d-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4300d-185">JSON representation</span></span>

<span data-ttu-id="4300d-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4300d-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

