---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97c683ca47f453efdcd267839b3a2239a400db66
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158623"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="1c892-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c892-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="1c892-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c892-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c892-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包目录是零个或多个访问包的容器。</span><span class="sxs-lookup"><span data-stu-id="1c892-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="1c892-106">访问包目录可能还具有链接的资源，这些资源用于这些访问包中以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="1c892-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="1c892-107">方法</span><span class="sxs-lookup"><span data-stu-id="1c892-107">Methods</span></span>

| <span data-ttu-id="1c892-108">方法</span><span class="sxs-lookup"><span data-stu-id="1c892-108">Method</span></span>       | <span data-ttu-id="1c892-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c892-109">Return Type</span></span> | <span data-ttu-id="1c892-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c892-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1c892-111">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="1c892-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="1c892-112">[accessPackageCatalog](accesspackagecatalog.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c892-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="1c892-113">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1c892-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="1c892-114">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="1c892-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="1c892-116">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="1c892-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="1c892-117">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="1c892-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="1c892-119">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c892-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="1c892-120">更新 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="1c892-121">无</span><span class="sxs-lookup"><span data-stu-id="1c892-121">None</span></span> | <span data-ttu-id="1c892-122">更新 accessPackageCatalog 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1c892-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="1c892-123">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1c892-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="1c892-124">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="1c892-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="1c892-125">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="1c892-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="1c892-126">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c892-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="1c892-127">检索目录中的 accessPackageResource 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1c892-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="1c892-128">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="1c892-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="1c892-129">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c892-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="1c892-130">检索目录中资源的 accessPackageResourceRole 对象列表。</span><span class="sxs-lookup"><span data-stu-id="1c892-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="1c892-131">属性</span><span class="sxs-lookup"><span data-stu-id="1c892-131">Properties</span></span>

| <span data-ttu-id="1c892-132">属性</span><span class="sxs-lookup"><span data-stu-id="1c892-132">Property</span></span>     | <span data-ttu-id="1c892-133">类型</span><span class="sxs-lookup"><span data-stu-id="1c892-133">Type</span></span>        | <span data-ttu-id="1c892-134">说明</span><span class="sxs-lookup"><span data-stu-id="1c892-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c892-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="1c892-135">catalogStatus</span></span>|<span data-ttu-id="1c892-136">String</span><span class="sxs-lookup"><span data-stu-id="1c892-136">String</span></span>|<span data-ttu-id="1c892-137">如果访问 `Published` 包可用于管理，则具有值。</span><span class="sxs-lookup"><span data-stu-id="1c892-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="1c892-138">catalogType</span><span class="sxs-lookup"><span data-stu-id="1c892-138">catalogType</span></span>|<span data-ttu-id="1c892-139">String</span><span class="sxs-lookup"><span data-stu-id="1c892-139">String</span></span>|<span data-ttu-id="1c892-140">或 `UserManaged` `ServiceDefault` 之一。</span><span class="sxs-lookup"><span data-stu-id="1c892-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="1c892-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="1c892-141">createdBy</span></span>|<span data-ttu-id="1c892-142">String</span><span class="sxs-lookup"><span data-stu-id="1c892-142">String</span></span>|<span data-ttu-id="1c892-143">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="1c892-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="1c892-144">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-144">Read-only.</span></span>|
|<span data-ttu-id="1c892-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c892-145">createdDateTime</span></span>|<span data-ttu-id="1c892-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c892-146">DateTimeOffset</span></span>|<span data-ttu-id="1c892-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1c892-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c892-148">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1c892-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1c892-149">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-149">Read-only.</span></span>|
|<span data-ttu-id="1c892-150">说明</span><span class="sxs-lookup"><span data-stu-id="1c892-150">description</span></span>|<span data-ttu-id="1c892-151">String</span><span class="sxs-lookup"><span data-stu-id="1c892-151">String</span></span>|<span data-ttu-id="1c892-152">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="1c892-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="1c892-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1c892-153">displayName</span></span>|<span data-ttu-id="1c892-154">String</span><span class="sxs-lookup"><span data-stu-id="1c892-154">String</span></span>|<span data-ttu-id="1c892-155">访问显示名称目录的索引。</span><span class="sxs-lookup"><span data-stu-id="1c892-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="1c892-156">id</span><span class="sxs-lookup"><span data-stu-id="1c892-156">id</span></span>|<span data-ttu-id="1c892-157">String</span><span class="sxs-lookup"><span data-stu-id="1c892-157">String</span></span>| <span data-ttu-id="1c892-158">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-158">Read-only.</span></span>|
|<span data-ttu-id="1c892-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="1c892-159">isExternallyVisible</span></span>|<span data-ttu-id="1c892-160">布尔</span><span class="sxs-lookup"><span data-stu-id="1c892-160">Boolean</span></span>|<span data-ttu-id="1c892-161">租户外部的用户是否可以请求此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="1c892-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="1c892-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="1c892-162">modifiedBy</span></span>|<span data-ttu-id="1c892-163">String</span><span class="sxs-lookup"><span data-stu-id="1c892-163">String</span></span>|<span data-ttu-id="1c892-164">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="1c892-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="1c892-165">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-165">Read-only.</span></span>|
|<span data-ttu-id="1c892-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c892-166">modifiedDateTime</span></span>|<span data-ttu-id="1c892-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c892-167">DateTimeOffset</span></span>|<span data-ttu-id="1c892-168">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1c892-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c892-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1c892-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1c892-170">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="1c892-171">关系</span><span class="sxs-lookup"><span data-stu-id="1c892-171">Relationships</span></span>

| <span data-ttu-id="1c892-172">关系</span><span class="sxs-lookup"><span data-stu-id="1c892-172">Relationship</span></span> | <span data-ttu-id="1c892-173">类型</span><span class="sxs-lookup"><span data-stu-id="1c892-173">Type</span></span>        | <span data-ttu-id="1c892-174">说明</span><span class="sxs-lookup"><span data-stu-id="1c892-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c892-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="1c892-175">accessPackages</span></span>|<span data-ttu-id="1c892-176">[accessPackage](accesspackage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c892-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="1c892-177">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="1c892-177">The access packages in this catalog.</span></span> <span data-ttu-id="1c892-178">只读。</span><span class="sxs-lookup"><span data-stu-id="1c892-178">Read-only.</span></span> <span data-ttu-id="1c892-179">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1c892-179">Nullable.</span></span>|
|<span data-ttu-id="1c892-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="1c892-180">accessPackageResources</span></span>|<span data-ttu-id="1c892-181">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c892-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="1c892-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="1c892-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c892-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c892-184">JSON representation</span></span>

<span data-ttu-id="1c892-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c892-185">The following is a JSON representation of the resource.</span></span>

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


