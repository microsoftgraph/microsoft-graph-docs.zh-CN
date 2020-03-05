---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66b7939541ba57dafc3be852c82c89781fc82381
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508532"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="81313-103">accessPackageCatalog 资源类型</span><span class="sxs-lookup"><span data-stu-id="81313-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="81313-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="81313-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81313-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包目录是零个或多个 access 程序包的容器。</span><span class="sxs-lookup"><span data-stu-id="81313-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="81313-106">访问包目录还可能具有在这些访问包中使用的链接资源，以提供访问权限。</span><span class="sxs-lookup"><span data-stu-id="81313-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="81313-107">方法</span><span class="sxs-lookup"><span data-stu-id="81313-107">Methods</span></span>

| <span data-ttu-id="81313-108">方法</span><span class="sxs-lookup"><span data-stu-id="81313-108">Method</span></span>       | <span data-ttu-id="81313-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="81313-109">Return Type</span></span> | <span data-ttu-id="81313-110">说明</span><span class="sxs-lookup"><span data-stu-id="81313-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81313-111">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="81313-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="81313-112">[accessPackageCatalog](accesspackagecatalog.md)集合</span><span class="sxs-lookup"><span data-stu-id="81313-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="81313-113">检索 accesspackagecatalog 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="81313-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="81313-114">创建 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="81313-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="81313-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="81313-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="81313-116">创建新的 accessPackageCatalog 对象。</span><span class="sxs-lookup"><span data-stu-id="81313-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="81313-117">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="81313-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="81313-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="81313-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="81313-119">读取 accessPackageCatalog 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81313-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="81313-120">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="81313-120">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="81313-121">删除 accessPackageCatalog。</span><span class="sxs-lookup"><span data-stu-id="81313-121">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="81313-122">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="81313-122">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="81313-123">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="81313-123">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="81313-124">检索目录中的 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="81313-124">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="81313-125">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="81313-125">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="81313-126">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="81313-126">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="81313-127">检索目录中资源的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="81313-127">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="81313-128">属性</span><span class="sxs-lookup"><span data-stu-id="81313-128">Properties</span></span>

| <span data-ttu-id="81313-129">属性</span><span class="sxs-lookup"><span data-stu-id="81313-129">Property</span></span>     | <span data-ttu-id="81313-130">类型</span><span class="sxs-lookup"><span data-stu-id="81313-130">Type</span></span>        | <span data-ttu-id="81313-131">说明</span><span class="sxs-lookup"><span data-stu-id="81313-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81313-132">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="81313-132">catalogStatus</span></span>|<span data-ttu-id="81313-133">String</span><span class="sxs-lookup"><span data-stu-id="81313-133">String</span></span>|<span data-ttu-id="81313-134">如果访问包`Published`可用于管理，则具有值。</span><span class="sxs-lookup"><span data-stu-id="81313-134">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="81313-135">catalogType</span><span class="sxs-lookup"><span data-stu-id="81313-135">catalogType</span></span>|<span data-ttu-id="81313-136">String</span><span class="sxs-lookup"><span data-stu-id="81313-136">String</span></span>|<span data-ttu-id="81313-137">一个`UserManaged`或`ServiceDefault`。</span><span class="sxs-lookup"><span data-stu-id="81313-137">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="81313-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="81313-138">createdBy</span></span>|<span data-ttu-id="81313-139">String</span><span class="sxs-lookup"><span data-stu-id="81313-139">String</span></span>|<span data-ttu-id="81313-140">创建此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="81313-140">UPN of the user who created this resource.</span></span> <span data-ttu-id="81313-141">只读。</span><span class="sxs-lookup"><span data-stu-id="81313-141">Read-only.</span></span>|
|<span data-ttu-id="81313-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81313-142">createdDateTime</span></span>|<span data-ttu-id="81313-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81313-143">DateTimeOffset</span></span>|<span data-ttu-id="81313-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="81313-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81313-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="81313-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="81313-146">只读。</span><span class="sxs-lookup"><span data-stu-id="81313-146">Read-only.</span></span>|
|<span data-ttu-id="81313-147">说明</span><span class="sxs-lookup"><span data-stu-id="81313-147">description</span></span>|<span data-ttu-id="81313-148">String</span><span class="sxs-lookup"><span data-stu-id="81313-148">String</span></span>|<span data-ttu-id="81313-149">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="81313-149">The description of the access package catalog.</span></span>|
|<span data-ttu-id="81313-150">displayName</span><span class="sxs-lookup"><span data-stu-id="81313-150">displayName</span></span>|<span data-ttu-id="81313-151">String</span><span class="sxs-lookup"><span data-stu-id="81313-151">String</span></span>|<span data-ttu-id="81313-152">访问包目录的显示名称。</span><span class="sxs-lookup"><span data-stu-id="81313-152">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="81313-153">id</span><span class="sxs-lookup"><span data-stu-id="81313-153">id</span></span>|<span data-ttu-id="81313-154">字符串</span><span class="sxs-lookup"><span data-stu-id="81313-154">String</span></span>| <span data-ttu-id="81313-155">只读。</span><span class="sxs-lookup"><span data-stu-id="81313-155">Read-only.</span></span>|
|<span data-ttu-id="81313-156">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="81313-156">isExternallyVisible</span></span>|<span data-ttu-id="81313-157">布尔</span><span class="sxs-lookup"><span data-stu-id="81313-157">Boolean</span></span>|<span data-ttu-id="81313-158">租户外部的用户是否可以请求此目录中的访问程序包。</span><span class="sxs-lookup"><span data-stu-id="81313-158">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="81313-159">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="81313-159">modifiedBy</span></span>|<span data-ttu-id="81313-160">String</span><span class="sxs-lookup"><span data-stu-id="81313-160">String</span></span>|<span data-ttu-id="81313-161">上次修改此资源的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="81313-161">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="81313-162">只读。</span><span class="sxs-lookup"><span data-stu-id="81313-162">Read-only.</span></span>|
|<span data-ttu-id="81313-163">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81313-163">modifiedDateTime</span></span>|<span data-ttu-id="81313-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81313-164">DateTimeOffset</span></span>|<span data-ttu-id="81313-165">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="81313-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81313-166">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="81313-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="81313-167">只读。</span><span class="sxs-lookup"><span data-stu-id="81313-167">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="81313-168">关系</span><span class="sxs-lookup"><span data-stu-id="81313-168">Relationships</span></span>

| <span data-ttu-id="81313-169">关系</span><span class="sxs-lookup"><span data-stu-id="81313-169">Relationship</span></span> | <span data-ttu-id="81313-170">类型</span><span class="sxs-lookup"><span data-stu-id="81313-170">Type</span></span>        | <span data-ttu-id="81313-171">说明</span><span class="sxs-lookup"><span data-stu-id="81313-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="81313-172">accessPackages</span><span class="sxs-lookup"><span data-stu-id="81313-172">accessPackages</span></span>|<span data-ttu-id="81313-173">[accessPackage](accesspackage.md)集合</span><span class="sxs-lookup"><span data-stu-id="81313-173">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="81313-174">此目录中的访问包。</span><span class="sxs-lookup"><span data-stu-id="81313-174">The access packages in this catalog.</span></span> <span data-ttu-id="81313-175">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="81313-175">Read-only.</span></span> <span data-ttu-id="81313-176">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="81313-176">Nullable.</span></span>|
|<span data-ttu-id="81313-177">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="81313-177">accessPackageResources</span></span>|<span data-ttu-id="81313-178">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="81313-178">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="81313-p107">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="81313-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81313-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81313-181">JSON representation</span></span>

<span data-ttu-id="81313-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81313-182">The following is a JSON representation of the resource.</span></span>

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
