---
title: accessPackageResource 资源类型
description: 访问包资源是一种对与目录关联的资源的引用，该目录的角色可在一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9c7b5e91c191ceaa747393e42e278bf9146bdc3a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722195"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="17c3e-103">accessPackageResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="17c3e-103">accessPackageResource resource type</span></span>

<span data-ttu-id="17c3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17c3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17c3e-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源是一个对与访问包目录关联的资源的引用。</span><span class="sxs-lookup"><span data-stu-id="17c3e-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog.</span></span> <span data-ttu-id="17c3e-106">访问包资源的角色可在一个或多个访问包中使用。</span><span class="sxs-lookup"><span data-stu-id="17c3e-106">The roles for the access package resource can be used in one or more access packages.</span></span>  <span data-ttu-id="17c3e-107">若要请求将资源与访问包目录关联，或者从目录中删除资源，请创建[accessPackageResourceRequest。](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="17c3e-107">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="17c3e-108">方法</span><span class="sxs-lookup"><span data-stu-id="17c3e-108">Methods</span></span>

| <span data-ttu-id="17c3e-109">方法</span><span class="sxs-lookup"><span data-stu-id="17c3e-109">Method</span></span>       | <span data-ttu-id="17c3e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="17c3e-110">Return Type</span></span> | <span data-ttu-id="17c3e-111">说明</span><span class="sxs-lookup"><span data-stu-id="17c3e-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="17c3e-112">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="17c3e-112">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="17c3e-113">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17c3e-113">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="17c3e-114">检索目录中 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="17c3e-114">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="17c3e-115">属性</span><span class="sxs-lookup"><span data-stu-id="17c3e-115">Properties</span></span>

| <span data-ttu-id="17c3e-116">属性</span><span class="sxs-lookup"><span data-stu-id="17c3e-116">Property</span></span>     | <span data-ttu-id="17c3e-117">类型</span><span class="sxs-lookup"><span data-stu-id="17c3e-117">Type</span></span>        | <span data-ttu-id="17c3e-118">说明</span><span class="sxs-lookup"><span data-stu-id="17c3e-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17c3e-119">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17c3e-119">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="17c3e-120">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17c3e-120">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="17c3e-121">包含资源的环境信息。</span><span class="sxs-lookup"><span data-stu-id="17c3e-121">Contains the environment information for the resource.</span></span> <span data-ttu-id="17c3e-122">可以使用批注或环境的 `@odata.bind` *originId 进行设置*。</span><span class="sxs-lookup"><span data-stu-id="17c3e-122">This can be set using either the `@odata.bind` annotation or the environment's *originId*.</span></span>|
|<span data-ttu-id="17c3e-123">addedBy</span><span class="sxs-lookup"><span data-stu-id="17c3e-123">addedBy</span></span>|<span data-ttu-id="17c3e-124">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-124">String</span></span>|<span data-ttu-id="17c3e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="17c3e-125">Read-only.</span></span>|
|<span data-ttu-id="17c3e-126">addedOn</span><span class="sxs-lookup"><span data-stu-id="17c3e-126">addedOn</span></span>|<span data-ttu-id="17c3e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17c3e-127">DateTimeOffset</span></span>|<span data-ttu-id="17c3e-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="17c3e-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17c3e-129">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="17c3e-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="17c3e-130">说明</span><span class="sxs-lookup"><span data-stu-id="17c3e-130">description</span></span>|<span data-ttu-id="17c3e-131">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-131">String</span></span>|<span data-ttu-id="17c3e-132">资源的说明。</span><span class="sxs-lookup"><span data-stu-id="17c3e-132">A description for the resource.</span></span>|
|<span data-ttu-id="17c3e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="17c3e-133">displayName</span></span>|<span data-ttu-id="17c3e-134">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-134">String</span></span>|<span data-ttu-id="17c3e-135">资源显示名称，如应用程序名称、组名称或网站名称。</span><span class="sxs-lookup"><span data-stu-id="17c3e-135">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="17c3e-136">id</span><span class="sxs-lookup"><span data-stu-id="17c3e-136">id</span></span>|<span data-ttu-id="17c3e-137">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-137">String</span></span>| <span data-ttu-id="17c3e-138">只读。</span><span class="sxs-lookup"><span data-stu-id="17c3e-138">Read-only.</span></span>|
|<span data-ttu-id="17c3e-139">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="17c3e-139">isPendingOnboarding</span></span>|<span data-ttu-id="17c3e-140">布尔</span><span class="sxs-lookup"><span data-stu-id="17c3e-140">Boolean</span></span>|<span data-ttu-id="17c3e-141">如果资源尚未可用于工作分配，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="17c3e-141">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="17c3e-142">originId</span><span class="sxs-lookup"><span data-stu-id="17c3e-142">originId</span></span>|<span data-ttu-id="17c3e-143">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-143">String</span></span>|<span data-ttu-id="17c3e-144">源系统中资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="17c3e-144">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="17c3e-145">对于 Azure AD 组，这是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="17c3e-145">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="17c3e-146">originSystem</span><span class="sxs-lookup"><span data-stu-id="17c3e-146">originSystem</span></span>|<span data-ttu-id="17c3e-147">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-147">String</span></span>|<span data-ttu-id="17c3e-148">源系统中资源的类型，例如 `SharePointOnline` ， `AadApplication` 或 `AadGroup` 。</span><span class="sxs-lookup"><span data-stu-id="17c3e-148">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="17c3e-149">resourceType</span><span class="sxs-lookup"><span data-stu-id="17c3e-149">resourceType</span></span>|<span data-ttu-id="17c3e-150">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-150">String</span></span>|<span data-ttu-id="17c3e-151">资源的类型，例如它是 Azure `Application` AD 连接应用程序或 `SharePoint Online Site` SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="17c3e-151">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="17c3e-152">url</span><span class="sxs-lookup"><span data-stu-id="17c3e-152">url</span></span>|<span data-ttu-id="17c3e-153">String</span><span class="sxs-lookup"><span data-stu-id="17c3e-153">String</span></span>|<span data-ttu-id="17c3e-154">资源的唯一资源定位器，例如用于将用户登录应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="17c3e-154">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17c3e-155">关系</span><span class="sxs-lookup"><span data-stu-id="17c3e-155">Relationships</span></span>

| <span data-ttu-id="17c3e-156">关系</span><span class="sxs-lookup"><span data-stu-id="17c3e-156">Relationship</span></span> | <span data-ttu-id="17c3e-157">类型</span><span class="sxs-lookup"><span data-stu-id="17c3e-157">Type</span></span>        | <span data-ttu-id="17c3e-158">说明</span><span class="sxs-lookup"><span data-stu-id="17c3e-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17c3e-159">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17c3e-159">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="17c3e-160">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="17c3e-160">accessPackageResourceEnvironment</span></span>](accesspackageresourceenvironment.md)| <span data-ttu-id="17c3e-161">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="17c3e-161">Nullable.</span></span>|
|<span data-ttu-id="17c3e-162">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="17c3e-162">accessPackageResourceRoles</span></span>|<span data-ttu-id="17c3e-163">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17c3e-163">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="17c3e-164">只读。</span><span class="sxs-lookup"><span data-stu-id="17c3e-164">Read-only.</span></span> <span data-ttu-id="17c3e-165">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="17c3e-165">Nullable.</span></span>|
|<span data-ttu-id="17c3e-166">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="17c3e-166">accessPackageResourceScopes</span></span>|<span data-ttu-id="17c3e-167">[accessPackageResourceScope](accesspackageresourcescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17c3e-167">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="17c3e-p106">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="17c3e-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17c3e-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17c3e-170">JSON representation</span></span>

<span data-ttu-id="17c3e-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17c3e-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
