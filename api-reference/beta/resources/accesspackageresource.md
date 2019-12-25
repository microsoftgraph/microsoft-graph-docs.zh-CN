---
title: accessPackageResource 资源类型
description: 访问包资源是对与目录关联的资源的引用。可在一个或多个访问包中使用的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0567ca9347b560b14ae96da4914a8801f9183019
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870972"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="4f3a9-103">accessPackageResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f3a9-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f3a9-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源是对与访问包目录关联的资源（可在一个或多个访问包中使用的角色）的引用。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="4f3a9-105">若要请求将资源与访问包目录相关联，请创建一个[accessPackageResourceRequest](accesspackageresourcerequest.md)。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-105">To request to associate a resource with an access package catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4f3a9-106">方法</span><span class="sxs-lookup"><span data-stu-id="4f3a9-106">Methods</span></span>

| <span data-ttu-id="4f3a9-107">方法</span><span class="sxs-lookup"><span data-stu-id="4f3a9-107">Method</span></span>       | <span data-ttu-id="4f3a9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f3a9-108">Return Type</span></span> | <span data-ttu-id="4f3a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f3a9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4f3a9-110">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="4f3a9-110">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="4f3a9-111">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f3a9-111">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="4f3a9-112">检索目录中的 accessPackageResource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-112">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f3a9-113">属性</span><span class="sxs-lookup"><span data-stu-id="4f3a9-113">Properties</span></span>

| <span data-ttu-id="4f3a9-114">属性</span><span class="sxs-lookup"><span data-stu-id="4f3a9-114">Property</span></span>     | <span data-ttu-id="4f3a9-115">类型</span><span class="sxs-lookup"><span data-stu-id="4f3a9-115">Type</span></span>        | <span data-ttu-id="4f3a9-116">说明</span><span class="sxs-lookup"><span data-stu-id="4f3a9-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f3a9-117">addedBy</span><span class="sxs-lookup"><span data-stu-id="4f3a9-117">addedBy</span></span>|<span data-ttu-id="4f3a9-118">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-118">String</span></span>|<span data-ttu-id="4f3a9-119">只读。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-119">Read-only.</span></span>|
|<span data-ttu-id="4f3a9-120">addedOn</span><span class="sxs-lookup"><span data-stu-id="4f3a9-120">addedOn</span></span>|<span data-ttu-id="4f3a9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f3a9-121">DateTimeOffset</span></span>|<span data-ttu-id="4f3a9-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4f3a9-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4f3a9-124">description</span><span class="sxs-lookup"><span data-stu-id="4f3a9-124">description</span></span>|<span data-ttu-id="4f3a9-125">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-125">String</span></span>|<span data-ttu-id="4f3a9-126">资源的说明。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-126">A description for the resource.</span></span>|
|<span data-ttu-id="4f3a9-127">displayName</span><span class="sxs-lookup"><span data-stu-id="4f3a9-127">displayName</span></span>|<span data-ttu-id="4f3a9-128">字符串</span><span class="sxs-lookup"><span data-stu-id="4f3a9-128">String</span></span>|<span data-ttu-id="4f3a9-129">资源的显示名称，例如应用程序名称、组名称或网站名称。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-129">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="4f3a9-130">id</span><span class="sxs-lookup"><span data-stu-id="4f3a9-130">id</span></span>|<span data-ttu-id="4f3a9-131">字符串</span><span class="sxs-lookup"><span data-stu-id="4f3a9-131">String</span></span>| <span data-ttu-id="4f3a9-132">只读。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-132">Read-only.</span></span>|
|<span data-ttu-id="4f3a9-133">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="4f3a9-133">isPendingOnboarding</span></span>|<span data-ttu-id="4f3a9-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f3a9-134">Boolean</span></span>|<span data-ttu-id="4f3a9-135">如果资源尚不可用于工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-135">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="4f3a9-136">originId</span><span class="sxs-lookup"><span data-stu-id="4f3a9-136">originId</span></span>|<span data-ttu-id="4f3a9-137">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-137">String</span></span>|<span data-ttu-id="4f3a9-138">源系统中资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-138">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="4f3a9-139">在 Azure AD 组的情况下，这是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-139">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="4f3a9-140">originSystem</span><span class="sxs-lookup"><span data-stu-id="4f3a9-140">originSystem</span></span>|<span data-ttu-id="4f3a9-141">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-141">String</span></span>|<span data-ttu-id="4f3a9-142">源系统中资源的类型，例如`SharePointOnline`或。 `AadGroup`</span><span class="sxs-lookup"><span data-stu-id="4f3a9-142">The type of the resource in the origin system, such as `SharePointOnline` or `AadGroup`.</span></span>|
|<span data-ttu-id="4f3a9-143">resourceType</span><span class="sxs-lookup"><span data-stu-id="4f3a9-143">resourceType</span></span>|<span data-ttu-id="4f3a9-144">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-144">String</span></span>|<span data-ttu-id="4f3a9-145">资源的类型，例如`Application` ，它是 Azure AD 连接的应用程序，或者`SharePoint Online Site`是 SharePoint Online 网站的类型。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-145">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="4f3a9-146">url</span><span class="sxs-lookup"><span data-stu-id="4f3a9-146">url</span></span>|<span data-ttu-id="4f3a9-147">String</span><span class="sxs-lookup"><span data-stu-id="4f3a9-147">String</span></span>|<span data-ttu-id="4f3a9-148">资源的唯一资源定位器，例如用于将用户签名到应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-148">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f3a9-149">关系</span><span class="sxs-lookup"><span data-stu-id="4f3a9-149">Relationships</span></span>

| <span data-ttu-id="4f3a9-150">关系</span><span class="sxs-lookup"><span data-stu-id="4f3a9-150">Relationship</span></span> | <span data-ttu-id="4f3a9-151">类型</span><span class="sxs-lookup"><span data-stu-id="4f3a9-151">Type</span></span>        | <span data-ttu-id="4f3a9-152">说明</span><span class="sxs-lookup"><span data-stu-id="4f3a9-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f3a9-153">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="4f3a9-153">accessPackageResourceRoles</span></span>|<span data-ttu-id="4f3a9-154">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f3a9-154">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="4f3a9-155">只读。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-155">Read-only.</span></span> <span data-ttu-id="4f3a9-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-156">Nullable.</span></span>|
|<span data-ttu-id="4f3a9-157">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="4f3a9-157">accessPackageResourceScopes</span></span>|<span data-ttu-id="4f3a9-158">[accessPackageResourceScope](accesspackageresourcescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f3a9-158">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="4f3a9-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f3a9-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f3a9-161">JSON representation</span></span>

<span data-ttu-id="4f3a9-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f3a9-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
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
