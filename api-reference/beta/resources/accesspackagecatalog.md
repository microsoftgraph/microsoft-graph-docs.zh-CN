---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d8c93defc8d76fbee1efbc162677f21b4e7f827
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089852"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="5701c-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="5701c-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="5701c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5701c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5701c-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包目录是零个或多个 access 程序包的容器。</span><span class="sxs-lookup"><span data-stu-id="5701c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="5701c-106">访问包目录还可能具有在这些访问包中使用的链接资源，以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="5701c-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="5701c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5701c-107">Methods</span></span>

| <span data-ttu-id="5701c-108">方法</span><span class="sxs-lookup"><span data-stu-id="5701c-108">Method</span></span>       | <span data-ttu-id="5701c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5701c-109">Return Type</span></span> | <span data-ttu-id="5701c-110">说明</span><span class="sxs-lookup"><span data-stu-id="5701c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5701c-111">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="5701c-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="5701c-112">[accessPackageCatalog](accesspackagecatalog.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5701c-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="5701c-113">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5701c-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="5701c-114">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="5701c-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="5701c-116">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="5701c-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5701c-117">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="5701c-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="5701c-119">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5701c-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5701c-120">更新 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="5701c-121">无</span><span class="sxs-lookup"><span data-stu-id="5701c-121">None</span></span> | <span data-ttu-id="5701c-122">更新 accessPackageCatalog 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5701c-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5701c-123">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5701c-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="5701c-124">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="5701c-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="5701c-125">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="5701c-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="5701c-126">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5701c-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="5701c-127">检索目录中的 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5701c-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="5701c-128">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="5701c-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="5701c-129">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5701c-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="5701c-130">检索目录中资源的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5701c-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="5701c-131">属性</span><span class="sxs-lookup"><span data-stu-id="5701c-131">Properties</span></span>

| <span data-ttu-id="5701c-132">属性</span><span class="sxs-lookup"><span data-stu-id="5701c-132">Property</span></span>     | <span data-ttu-id="5701c-133">类型</span><span class="sxs-lookup"><span data-stu-id="5701c-133">Type</span></span>        | <span data-ttu-id="5701c-134">说明</span><span class="sxs-lookup"><span data-stu-id="5701c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5701c-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="5701c-135">catalogStatus</span></span>|<span data-ttu-id="5701c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-136">String</span></span>|<span data-ttu-id="5701c-137">`Published`如果访问包可用于管理，则具有值。</span><span class="sxs-lookup"><span data-stu-id="5701c-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="5701c-138">catalogType</span><span class="sxs-lookup"><span data-stu-id="5701c-138">catalogType</span></span>|<span data-ttu-id="5701c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-139">String</span></span>|<span data-ttu-id="5701c-140">一个 `UserManaged` 或 `ServiceDefault` 。</span><span class="sxs-lookup"><span data-stu-id="5701c-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="5701c-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="5701c-141">createdBy</span></span>|<span data-ttu-id="5701c-142">String</span><span class="sxs-lookup"><span data-stu-id="5701c-142">String</span></span>|<span data-ttu-id="5701c-143">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="5701c-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="5701c-144">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-144">Read-only.</span></span>|
|<span data-ttu-id="5701c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5701c-145">createdDateTime</span></span>|<span data-ttu-id="5701c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5701c-146">DateTimeOffset</span></span>|<span data-ttu-id="5701c-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5701c-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5701c-148">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5701c-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5701c-149">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-149">Read-only.</span></span>|
|<span data-ttu-id="5701c-150">说明</span><span class="sxs-lookup"><span data-stu-id="5701c-150">description</span></span>|<span data-ttu-id="5701c-151">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-151">String</span></span>|<span data-ttu-id="5701c-152">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="5701c-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="5701c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="5701c-153">displayName</span></span>|<span data-ttu-id="5701c-154">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-154">String</span></span>|<span data-ttu-id="5701c-155">访问包目录的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5701c-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="5701c-156">id</span><span class="sxs-lookup"><span data-stu-id="5701c-156">id</span></span>|<span data-ttu-id="5701c-157">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-157">String</span></span>| <span data-ttu-id="5701c-158">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-158">Read-only.</span></span>|
|<span data-ttu-id="5701c-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="5701c-159">isExternallyVisible</span></span>|<span data-ttu-id="5701c-160">布尔</span><span class="sxs-lookup"><span data-stu-id="5701c-160">Boolean</span></span>|<span data-ttu-id="5701c-161">租户外部的用户是否可以请求此目录中的访问程序包。</span><span class="sxs-lookup"><span data-stu-id="5701c-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="5701c-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="5701c-162">modifiedBy</span></span>|<span data-ttu-id="5701c-163">字符串</span><span class="sxs-lookup"><span data-stu-id="5701c-163">String</span></span>|<span data-ttu-id="5701c-164">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="5701c-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="5701c-165">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-165">Read-only.</span></span>|
|<span data-ttu-id="5701c-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5701c-166">modifiedDateTime</span></span>|<span data-ttu-id="5701c-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5701c-167">DateTimeOffset</span></span>|<span data-ttu-id="5701c-168">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5701c-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5701c-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5701c-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5701c-170">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="5701c-171">关系</span><span class="sxs-lookup"><span data-stu-id="5701c-171">Relationships</span></span>

| <span data-ttu-id="5701c-172">关系</span><span class="sxs-lookup"><span data-stu-id="5701c-172">Relationship</span></span> | <span data-ttu-id="5701c-173">类型</span><span class="sxs-lookup"><span data-stu-id="5701c-173">Type</span></span>        | <span data-ttu-id="5701c-174">说明</span><span class="sxs-lookup"><span data-stu-id="5701c-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5701c-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="5701c-175">accessPackages</span></span>|<span data-ttu-id="5701c-176">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5701c-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="5701c-177">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="5701c-177">The access packages in this catalog.</span></span> <span data-ttu-id="5701c-178">只读。</span><span class="sxs-lookup"><span data-stu-id="5701c-178">Read-only.</span></span> <span data-ttu-id="5701c-179">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5701c-179">Nullable.</span></span>|
|<span data-ttu-id="5701c-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="5701c-180">accessPackageResources</span></span>|<span data-ttu-id="5701c-181">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5701c-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="5701c-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="5701c-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5701c-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5701c-184">JSON representation</span></span>

<span data-ttu-id="5701c-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5701c-185">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "baseType": "",
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


