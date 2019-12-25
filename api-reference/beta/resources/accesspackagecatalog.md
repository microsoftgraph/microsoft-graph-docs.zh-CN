---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c8fde3b6ead60cada5e663b2150ba463187b22b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870413"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="7c726-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c726-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c726-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包目录是零个或多个 access 程序包的容器。</span><span class="sxs-lookup"><span data-stu-id="7c726-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="7c726-105">访问包目录还可能具有在这些访问包中使用的链接资源，以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="7c726-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="7c726-106">方法</span><span class="sxs-lookup"><span data-stu-id="7c726-106">Methods</span></span>

| <span data-ttu-id="7c726-107">方法</span><span class="sxs-lookup"><span data-stu-id="7c726-107">Method</span></span>       | <span data-ttu-id="7c726-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c726-108">Return Type</span></span> | <span data-ttu-id="7c726-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c726-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7c726-110">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="7c726-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="7c726-111">[accessPackageCatalog](accesspackagecatalog.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c726-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="7c726-112">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7c726-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="7c726-113">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c726-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="7c726-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c726-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="7c726-115">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="7c726-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="7c726-116">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c726-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="7c726-117">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c726-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="7c726-118">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c726-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="7c726-119">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7c726-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="7c726-120">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="7c726-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="7c726-121">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="7c726-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="7c726-122">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c726-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="7c726-123">检索目录中的 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7c726-123">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="7c726-124">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="7c726-124">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="7c726-125">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c726-125">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="7c726-126">检索目录中资源的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7c726-126">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c726-127">属性</span><span class="sxs-lookup"><span data-stu-id="7c726-127">Properties</span></span>

| <span data-ttu-id="7c726-128">属性</span><span class="sxs-lookup"><span data-stu-id="7c726-128">Property</span></span>     | <span data-ttu-id="7c726-129">类型</span><span class="sxs-lookup"><span data-stu-id="7c726-129">Type</span></span>        | <span data-ttu-id="7c726-130">说明</span><span class="sxs-lookup"><span data-stu-id="7c726-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c726-131">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="7c726-131">catalogStatus</span></span>|<span data-ttu-id="7c726-132">String</span><span class="sxs-lookup"><span data-stu-id="7c726-132">String</span></span>|<span data-ttu-id="7c726-133">如果访问包`Published`可用于管理，则具有值。</span><span class="sxs-lookup"><span data-stu-id="7c726-133">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="7c726-134">catalogType</span><span class="sxs-lookup"><span data-stu-id="7c726-134">catalogType</span></span>|<span data-ttu-id="7c726-135">String</span><span class="sxs-lookup"><span data-stu-id="7c726-135">String</span></span>|<span data-ttu-id="7c726-136">一个`UserManaged`或`ServiceDefault`。</span><span class="sxs-lookup"><span data-stu-id="7c726-136">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="7c726-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c726-137">createdBy</span></span>|<span data-ttu-id="7c726-138">String</span><span class="sxs-lookup"><span data-stu-id="7c726-138">String</span></span>|<span data-ttu-id="7c726-139">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="7c726-139">UPN of the user who created this resource.</span></span> <span data-ttu-id="7c726-140">只读。</span><span class="sxs-lookup"><span data-stu-id="7c726-140">Read-only.</span></span>|
|<span data-ttu-id="7c726-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c726-141">createdDateTime</span></span>|<span data-ttu-id="7c726-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c726-142">DateTimeOffset</span></span>|<span data-ttu-id="7c726-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7c726-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c726-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7c726-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7c726-145">只读。</span><span class="sxs-lookup"><span data-stu-id="7c726-145">Read-only.</span></span>|
|<span data-ttu-id="7c726-146">说明</span><span class="sxs-lookup"><span data-stu-id="7c726-146">description</span></span>|<span data-ttu-id="7c726-147">String</span><span class="sxs-lookup"><span data-stu-id="7c726-147">String</span></span>|<span data-ttu-id="7c726-148">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="7c726-148">The description of the access package catalog.</span></span>|
|<span data-ttu-id="7c726-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7c726-149">displayName</span></span>|<span data-ttu-id="7c726-150">String</span><span class="sxs-lookup"><span data-stu-id="7c726-150">String</span></span>|<span data-ttu-id="7c726-151">访问包目录的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c726-151">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="7c726-152">id</span><span class="sxs-lookup"><span data-stu-id="7c726-152">id</span></span>|<span data-ttu-id="7c726-153">字符串</span><span class="sxs-lookup"><span data-stu-id="7c726-153">String</span></span>| <span data-ttu-id="7c726-154">只读。</span><span class="sxs-lookup"><span data-stu-id="7c726-154">Read-only.</span></span>|
|<span data-ttu-id="7c726-155">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="7c726-155">isExternallyVisible</span></span>|<span data-ttu-id="7c726-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c726-156">Boolean</span></span>|<span data-ttu-id="7c726-157">租户外部的用户是否可以请求此目录中的访问程序包。</span><span class="sxs-lookup"><span data-stu-id="7c726-157">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="7c726-158">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="7c726-158">modifiedBy</span></span>|<span data-ttu-id="7c726-159">String</span><span class="sxs-lookup"><span data-stu-id="7c726-159">String</span></span>|<span data-ttu-id="7c726-160">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="7c726-160">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="7c726-161">只读。</span><span class="sxs-lookup"><span data-stu-id="7c726-161">Read-only.</span></span>|
|<span data-ttu-id="7c726-162">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c726-162">modifiedDateTime</span></span>|<span data-ttu-id="7c726-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c726-163">DateTimeOffset</span></span>|<span data-ttu-id="7c726-164">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7c726-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7c726-165">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7c726-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7c726-166">只读。</span><span class="sxs-lookup"><span data-stu-id="7c726-166">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="7c726-167">关系</span><span class="sxs-lookup"><span data-stu-id="7c726-167">Relationships</span></span>

| <span data-ttu-id="7c726-168">关系</span><span class="sxs-lookup"><span data-stu-id="7c726-168">Relationship</span></span> | <span data-ttu-id="7c726-169">类型</span><span class="sxs-lookup"><span data-stu-id="7c726-169">Type</span></span>        | <span data-ttu-id="7c726-170">说明</span><span class="sxs-lookup"><span data-stu-id="7c726-170">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c726-171">accessPackages</span><span class="sxs-lookup"><span data-stu-id="7c726-171">accessPackages</span></span>|<span data-ttu-id="7c726-172">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c726-172">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="7c726-173">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="7c726-173">The access packages in this catalog.</span></span> <span data-ttu-id="7c726-174">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7c726-174">Read-only.</span></span> <span data-ttu-id="7c726-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7c726-175">Nullable.</span></span>|
|<span data-ttu-id="7c726-176">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="7c726-176">accessPackageResources</span></span>|<span data-ttu-id="7c726-177">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c726-177">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="7c726-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="7c726-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c726-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c726-180">JSON representation</span></span>

<span data-ttu-id="7c726-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c726-181">The following is a JSON representation of the resource.</span></span>

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
