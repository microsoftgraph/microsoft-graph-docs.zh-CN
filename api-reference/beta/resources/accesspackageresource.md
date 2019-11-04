---
title: accessPackageResource 资源类型
description: 访问包资源是对与目录关联的资源的引用。可在一个或多个访问包中使用的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e964a8ce2e9bd4165a29037a56ec4f95fe969422
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938924"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="41b8a-103">accessPackageResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="41b8a-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41b8a-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源是对与目录关联的资源的引用。可在一个或多个访问包中使用的角色。</span><span class="sxs-lookup"><span data-stu-id="41b8a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with a catalog the roles for which can be used in one or more access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="41b8a-105">方法</span><span class="sxs-lookup"><span data-stu-id="41b8a-105">Methods</span></span>

| <span data-ttu-id="41b8a-106">方法</span><span class="sxs-lookup"><span data-stu-id="41b8a-106">Method</span></span>       | <span data-ttu-id="41b8a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="41b8a-107">Return Type</span></span> | <span data-ttu-id="41b8a-108">说明</span><span class="sxs-lookup"><span data-stu-id="41b8a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="41b8a-109">列出 accessPackageCatalog 资源</span><span class="sxs-lookup"><span data-stu-id="41b8a-109">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="41b8a-110">[accessPackageResource](accesspackageresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="41b8a-110">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="41b8a-111">检索 accesspackageresource 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="41b8a-111">Retrieve a list of accesspackageresource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="41b8a-112">属性</span><span class="sxs-lookup"><span data-stu-id="41b8a-112">Properties</span></span>

| <span data-ttu-id="41b8a-113">属性</span><span class="sxs-lookup"><span data-stu-id="41b8a-113">Property</span></span>     | <span data-ttu-id="41b8a-114">类型</span><span class="sxs-lookup"><span data-stu-id="41b8a-114">Type</span></span>        | <span data-ttu-id="41b8a-115">描述</span><span class="sxs-lookup"><span data-stu-id="41b8a-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41b8a-116">addedBy</span><span class="sxs-lookup"><span data-stu-id="41b8a-116">addedBy</span></span>|<span data-ttu-id="41b8a-117">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-117">String</span></span>|<span data-ttu-id="41b8a-118">只读。</span><span class="sxs-lookup"><span data-stu-id="41b8a-118">Read-only.</span></span>|
|<span data-ttu-id="41b8a-119">addedOn</span><span class="sxs-lookup"><span data-stu-id="41b8a-119">addedOn</span></span>|<span data-ttu-id="41b8a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41b8a-120">DateTimeOffset</span></span>|<span data-ttu-id="41b8a-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="41b8a-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="41b8a-123">description</span><span class="sxs-lookup"><span data-stu-id="41b8a-123">description</span></span>|<span data-ttu-id="41b8a-124">String</span><span class="sxs-lookup"><span data-stu-id="41b8a-124">String</span></span>|<span data-ttu-id="41b8a-125">资源的说明。</span><span class="sxs-lookup"><span data-stu-id="41b8a-125">A description for the resource.</span></span>|
|<span data-ttu-id="41b8a-126">displayName</span><span class="sxs-lookup"><span data-stu-id="41b8a-126">displayName</span></span>|<span data-ttu-id="41b8a-127">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-127">String</span></span>|<span data-ttu-id="41b8a-128">资源的显示名称，例如应用程序名称、组名称或网站名称。</span><span class="sxs-lookup"><span data-stu-id="41b8a-128">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="41b8a-129">id</span><span class="sxs-lookup"><span data-stu-id="41b8a-129">id</span></span>|<span data-ttu-id="41b8a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-130">String</span></span>| <span data-ttu-id="41b8a-131">只读。</span><span class="sxs-lookup"><span data-stu-id="41b8a-131">Read-only.</span></span>|
|<span data-ttu-id="41b8a-132">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="41b8a-132">isPendingOnboarding</span></span>|<span data-ttu-id="41b8a-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="41b8a-133">Boolean</span></span>|<span data-ttu-id="41b8a-134">如果资源尚不可用于工作分配，则为 True。</span><span class="sxs-lookup"><span data-stu-id="41b8a-134">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="41b8a-135">originId</span><span class="sxs-lookup"><span data-stu-id="41b8a-135">originId</span></span>|<span data-ttu-id="41b8a-136">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-136">String</span></span>|<span data-ttu-id="41b8a-137">源系统中资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="41b8a-137">The unique identifier of the resource in the origin system.</span></span> |
|<span data-ttu-id="41b8a-138">originSystem</span><span class="sxs-lookup"><span data-stu-id="41b8a-138">originSystem</span></span>|<span data-ttu-id="41b8a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-139">String</span></span>|<span data-ttu-id="41b8a-140">源系统中资源的类型。</span><span class="sxs-lookup"><span data-stu-id="41b8a-140">The type of the resource in the origin system.</span></span>|
|<span data-ttu-id="41b8a-141">resourceType</span><span class="sxs-lookup"><span data-stu-id="41b8a-141">resourceType</span></span>|<span data-ttu-id="41b8a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="41b8a-142">String</span></span>|<span data-ttu-id="41b8a-143">资源的类型，例如， `Application`如果是 Azure AD 连接的应用程序。</span><span class="sxs-lookup"><span data-stu-id="41b8a-143">The type of the resource, such as `Application` if it is an Azure AD connected application.</span></span>|
|<span data-ttu-id="41b8a-144">url</span><span class="sxs-lookup"><span data-stu-id="41b8a-144">url</span></span>|<span data-ttu-id="41b8a-145">String</span><span class="sxs-lookup"><span data-stu-id="41b8a-145">String</span></span>|<span data-ttu-id="41b8a-146">资源的唯一资源定位器，例如用于将用户签名到应用程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="41b8a-146">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41b8a-147">关系</span><span class="sxs-lookup"><span data-stu-id="41b8a-147">Relationships</span></span>

| <span data-ttu-id="41b8a-148">关系</span><span class="sxs-lookup"><span data-stu-id="41b8a-148">Relationship</span></span> | <span data-ttu-id="41b8a-149">类型</span><span class="sxs-lookup"><span data-stu-id="41b8a-149">Type</span></span>        | <span data-ttu-id="41b8a-150">描述</span><span class="sxs-lookup"><span data-stu-id="41b8a-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="41b8a-151">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="41b8a-151">accessPackageResourceRoles</span></span>|<span data-ttu-id="41b8a-152">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="41b8a-152">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="41b8a-153">只读。</span><span class="sxs-lookup"><span data-stu-id="41b8a-153">Read-only.</span></span> <span data-ttu-id="41b8a-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="41b8a-154">Nullable.</span></span>|
|<span data-ttu-id="41b8a-155">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="41b8a-155">accessPackageResourceScopes</span></span>|<span data-ttu-id="41b8a-156">[accessPackageResourceScope](accesspackageresourcescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="41b8a-156">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="41b8a-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="41b8a-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41b8a-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41b8a-159">JSON representation</span></span>

<span data-ttu-id="41b8a-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41b8a-160">The following is a JSON representation of the resource.</span></span>

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
