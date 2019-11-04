---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d95037bdf1e377f8981f99a06670957d838a2c92
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938931"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="62304-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="62304-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62304-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包目录是零个或多个 access 程序包的容器。</span><span class="sxs-lookup"><span data-stu-id="62304-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="62304-105">访问包目录还可能具有在这些访问包中使用的链接资源，以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="62304-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="62304-106">方法</span><span class="sxs-lookup"><span data-stu-id="62304-106">Methods</span></span>

| <span data-ttu-id="62304-107">方法</span><span class="sxs-lookup"><span data-stu-id="62304-107">Method</span></span>       | <span data-ttu-id="62304-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="62304-108">Return Type</span></span> | <span data-ttu-id="62304-109">说明</span><span class="sxs-lookup"><span data-stu-id="62304-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62304-110">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="62304-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="62304-111">[accessPackageCatalog](accesspackagecatalog.md)集合</span><span class="sxs-lookup"><span data-stu-id="62304-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="62304-112">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="62304-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="62304-113">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="62304-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="62304-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="62304-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="62304-115">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="62304-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="62304-116">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="62304-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="62304-117">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="62304-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="62304-118">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62304-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="62304-119">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="62304-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="62304-120">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="62304-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="62304-121">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="62304-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="62304-122">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="62304-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="62304-123">检索 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="62304-123">Retrieve a list of accessPackageResource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="62304-124">属性</span><span class="sxs-lookup"><span data-stu-id="62304-124">Properties</span></span>

| <span data-ttu-id="62304-125">属性</span><span class="sxs-lookup"><span data-stu-id="62304-125">Property</span></span>     | <span data-ttu-id="62304-126">类型</span><span class="sxs-lookup"><span data-stu-id="62304-126">Type</span></span>        | <span data-ttu-id="62304-127">描述</span><span class="sxs-lookup"><span data-stu-id="62304-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62304-128">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="62304-128">catalogStatus</span></span>|<span data-ttu-id="62304-129">字符串</span><span class="sxs-lookup"><span data-stu-id="62304-129">String</span></span>|<span data-ttu-id="62304-130">如果访问包`Published`可用于管理，则具有值。</span><span class="sxs-lookup"><span data-stu-id="62304-130">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="62304-131">catalogType</span><span class="sxs-lookup"><span data-stu-id="62304-131">catalogType</span></span>|<span data-ttu-id="62304-132">字符串</span><span class="sxs-lookup"><span data-stu-id="62304-132">String</span></span>|<span data-ttu-id="62304-133">一个`UserManaged`或`ServiceDefault`。</span><span class="sxs-lookup"><span data-stu-id="62304-133">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="62304-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="62304-134">createdBy</span></span>|<span data-ttu-id="62304-135">字符串</span><span class="sxs-lookup"><span data-stu-id="62304-135">String</span></span>|<span data-ttu-id="62304-136">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="62304-136">UPN of the user who created this resource.</span></span> <span data-ttu-id="62304-137">只读。</span><span class="sxs-lookup"><span data-stu-id="62304-137">Read-only.</span></span>|
|<span data-ttu-id="62304-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62304-138">createdDateTime</span></span>|<span data-ttu-id="62304-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62304-139">DateTimeOffset</span></span>|<span data-ttu-id="62304-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="62304-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="62304-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="62304-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="62304-142">只读。</span><span class="sxs-lookup"><span data-stu-id="62304-142">Read-only.</span></span>|
|<span data-ttu-id="62304-143">说明</span><span class="sxs-lookup"><span data-stu-id="62304-143">description</span></span>|<span data-ttu-id="62304-144">String</span><span class="sxs-lookup"><span data-stu-id="62304-144">String</span></span>|<span data-ttu-id="62304-145">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="62304-145">The description of the access package catalog.</span></span>|
|<span data-ttu-id="62304-146">displayName</span><span class="sxs-lookup"><span data-stu-id="62304-146">displayName</span></span>|<span data-ttu-id="62304-147">String</span><span class="sxs-lookup"><span data-stu-id="62304-147">String</span></span>|<span data-ttu-id="62304-148">访问包目录的显示名称。</span><span class="sxs-lookup"><span data-stu-id="62304-148">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="62304-149">id</span><span class="sxs-lookup"><span data-stu-id="62304-149">id</span></span>|<span data-ttu-id="62304-150">字符串</span><span class="sxs-lookup"><span data-stu-id="62304-150">String</span></span>| <span data-ttu-id="62304-151">只读。</span><span class="sxs-lookup"><span data-stu-id="62304-151">Read-only.</span></span>|
|<span data-ttu-id="62304-152">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="62304-152">isExternallyVisible</span></span>|<span data-ttu-id="62304-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="62304-153">Boolean</span></span>|<span data-ttu-id="62304-154">租户外部的用户是否可以请求此目录中的访问程序包。</span><span class="sxs-lookup"><span data-stu-id="62304-154">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="62304-155">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="62304-155">modifiedBy</span></span>|<span data-ttu-id="62304-156">字符串</span><span class="sxs-lookup"><span data-stu-id="62304-156">String</span></span>|<span data-ttu-id="62304-157">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="62304-157">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="62304-158">只读。</span><span class="sxs-lookup"><span data-stu-id="62304-158">Read-only.</span></span>|
|<span data-ttu-id="62304-159">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62304-159">modifiedDateTime</span></span>|<span data-ttu-id="62304-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62304-160">DateTimeOffset</span></span>|<span data-ttu-id="62304-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="62304-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="62304-162">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="62304-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="62304-163">只读。</span><span class="sxs-lookup"><span data-stu-id="62304-163">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="62304-164">关系</span><span class="sxs-lookup"><span data-stu-id="62304-164">Relationships</span></span>

| <span data-ttu-id="62304-165">关系</span><span class="sxs-lookup"><span data-stu-id="62304-165">Relationship</span></span> | <span data-ttu-id="62304-166">类型</span><span class="sxs-lookup"><span data-stu-id="62304-166">Type</span></span>        | <span data-ttu-id="62304-167">描述</span><span class="sxs-lookup"><span data-stu-id="62304-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62304-168">accessPackages</span><span class="sxs-lookup"><span data-stu-id="62304-168">accessPackages</span></span>|<span data-ttu-id="62304-169">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="62304-169">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="62304-170">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="62304-170">The access packages in this catalog.</span></span> <span data-ttu-id="62304-171">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="62304-171">Read-only.</span></span> <span data-ttu-id="62304-172">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="62304-172">Nullable.</span></span>|
|<span data-ttu-id="62304-173">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="62304-173">accessPackageResources</span></span>|<span data-ttu-id="62304-174">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="62304-174">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="62304-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="62304-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62304-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62304-177">JSON representation</span></span>

<span data-ttu-id="62304-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62304-178">The following is a JSON representation of the resource.</span></span>

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
