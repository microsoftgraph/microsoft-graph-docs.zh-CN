---
title: accessPackageResource 资源类型
description: 访问包资源是一个对与目录关联的资源的引用，该目录的角色可在一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e34b850b19836eeb19cc63232c7af822512bfee4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934820"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="96db8-103">accessPackageResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="96db8-103">accessPackageResource resource type</span></span>

<span data-ttu-id="96db8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96db8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96db8-105">在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包资源是一个对与访问包目录（可在一个或多个访问包中使用的角色）关联的资源的引用。</span><span class="sxs-lookup"><span data-stu-id="96db8-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="96db8-106">若要请求将资源与访问包目录关联，或者从目录中删除资源，请创建[accessPackageResourceRequest。](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="96db8-106">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="96db8-107">方法</span><span class="sxs-lookup"><span data-stu-id="96db8-107">Methods</span></span>

| <span data-ttu-id="96db8-108">方法</span><span class="sxs-lookup"><span data-stu-id="96db8-108">Method</span></span>       | <span data-ttu-id="96db8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="96db8-109">Return Type</span></span> | <span data-ttu-id="96db8-110">说明</span><span class="sxs-lookup"><span data-stu-id="96db8-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="96db8-111">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="96db8-111">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="96db8-112">[accessPackageResource](accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96db8-112">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="96db8-113">检索目录中的 accessPackageResource 对象列表。</span><span class="sxs-lookup"><span data-stu-id="96db8-113">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="96db8-114">属性</span><span class="sxs-lookup"><span data-stu-id="96db8-114">Properties</span></span>

| <span data-ttu-id="96db8-115">属性</span><span class="sxs-lookup"><span data-stu-id="96db8-115">Property</span></span>     | <span data-ttu-id="96db8-116">类型</span><span class="sxs-lookup"><span data-stu-id="96db8-116">Type</span></span>        | <span data-ttu-id="96db8-117">说明</span><span class="sxs-lookup"><span data-stu-id="96db8-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96db8-118">addedBy</span><span class="sxs-lookup"><span data-stu-id="96db8-118">addedBy</span></span>|<span data-ttu-id="96db8-119">String</span><span class="sxs-lookup"><span data-stu-id="96db8-119">String</span></span>|<span data-ttu-id="96db8-120">只读。</span><span class="sxs-lookup"><span data-stu-id="96db8-120">Read-only.</span></span>|
|<span data-ttu-id="96db8-121">addedOn</span><span class="sxs-lookup"><span data-stu-id="96db8-121">addedOn</span></span>|<span data-ttu-id="96db8-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96db8-122">DateTimeOffset</span></span>|<span data-ttu-id="96db8-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96db8-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96db8-125">说明</span><span class="sxs-lookup"><span data-stu-id="96db8-125">description</span></span>|<span data-ttu-id="96db8-126">String</span><span class="sxs-lookup"><span data-stu-id="96db8-126">String</span></span>|<span data-ttu-id="96db8-127">资源的说明。</span><span class="sxs-lookup"><span data-stu-id="96db8-127">A description for the resource.</span></span>|
|<span data-ttu-id="96db8-128">displayName</span><span class="sxs-lookup"><span data-stu-id="96db8-128">displayName</span></span>|<span data-ttu-id="96db8-129">String</span><span class="sxs-lookup"><span data-stu-id="96db8-129">String</span></span>|<span data-ttu-id="96db8-130">资源的显示名称，如应用程序名称、组名称或网站名称。</span><span class="sxs-lookup"><span data-stu-id="96db8-130">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="96db8-131">id</span><span class="sxs-lookup"><span data-stu-id="96db8-131">id</span></span>|<span data-ttu-id="96db8-132">String</span><span class="sxs-lookup"><span data-stu-id="96db8-132">String</span></span>| <span data-ttu-id="96db8-133">只读。</span><span class="sxs-lookup"><span data-stu-id="96db8-133">Read-only.</span></span>|
|<span data-ttu-id="96db8-134">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="96db8-134">isPendingOnboarding</span></span>|<span data-ttu-id="96db8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="96db8-135">Boolean</span></span>|<span data-ttu-id="96db8-136">如果资源尚未可用于工作分配，则其为 True。</span><span class="sxs-lookup"><span data-stu-id="96db8-136">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="96db8-137">originId</span><span class="sxs-lookup"><span data-stu-id="96db8-137">originId</span></span>|<span data-ttu-id="96db8-138">String</span><span class="sxs-lookup"><span data-stu-id="96db8-138">String</span></span>|<span data-ttu-id="96db8-139">源系统中资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96db8-139">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="96db8-140">对于 Azure AD 组，这是该组的标识符。</span><span class="sxs-lookup"><span data-stu-id="96db8-140">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="96db8-141">originSystem</span><span class="sxs-lookup"><span data-stu-id="96db8-141">originSystem</span></span>|<span data-ttu-id="96db8-142">String</span><span class="sxs-lookup"><span data-stu-id="96db8-142">String</span></span>|<span data-ttu-id="96db8-143">源系统中资源的类型，例如 `SharePointOnline` ， `AadApplication` 或 `AadGroup` 。</span><span class="sxs-lookup"><span data-stu-id="96db8-143">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="96db8-144">resourceType</span><span class="sxs-lookup"><span data-stu-id="96db8-144">resourceType</span></span>|<span data-ttu-id="96db8-145">String</span><span class="sxs-lookup"><span data-stu-id="96db8-145">String</span></span>|<span data-ttu-id="96db8-146">资源的类型，例如它是 Azure `Application` AD 连接的应用程序或 `SharePoint Online Site` SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="96db8-146">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="96db8-147">url</span><span class="sxs-lookup"><span data-stu-id="96db8-147">url</span></span>|<span data-ttu-id="96db8-148">String</span><span class="sxs-lookup"><span data-stu-id="96db8-148">String</span></span>|<span data-ttu-id="96db8-149">资源的唯一资源定位器，例如用于将用户登录应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="96db8-149">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96db8-150">关系</span><span class="sxs-lookup"><span data-stu-id="96db8-150">Relationships</span></span>

| <span data-ttu-id="96db8-151">关系</span><span class="sxs-lookup"><span data-stu-id="96db8-151">Relationship</span></span> | <span data-ttu-id="96db8-152">类型</span><span class="sxs-lookup"><span data-stu-id="96db8-152">Type</span></span>        | <span data-ttu-id="96db8-153">说明</span><span class="sxs-lookup"><span data-stu-id="96db8-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96db8-154">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="96db8-154">accessPackageResourceRoles</span></span>|<span data-ttu-id="96db8-155">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96db8-155">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="96db8-156">只读。</span><span class="sxs-lookup"><span data-stu-id="96db8-156">Read-only.</span></span> <span data-ttu-id="96db8-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="96db8-157">Nullable.</span></span>|
|<span data-ttu-id="96db8-158">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="96db8-158">accessPackageResourceScopes</span></span>|<span data-ttu-id="96db8-159">[accessPackageResourceScope](accesspackageresourcescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96db8-159">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="96db8-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="96db8-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96db8-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96db8-162">JSON representation</span></span>

<span data-ttu-id="96db8-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96db8-163">The following is a JSON representation of the resource.</span></span>

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


