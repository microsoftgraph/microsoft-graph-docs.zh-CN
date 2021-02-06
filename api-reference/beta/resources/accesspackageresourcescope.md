---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权利管理中，访问包资源范围是资源内范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1491028bb566e8742dcfc1e4928681f61e5272c7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133586"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="13aed-103">accessPackageResourceScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="13aed-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="13aed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13aed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13aed-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源范围是资源内对具有多个作用域的资源的作用域的引用。</span><span class="sxs-lookup"><span data-stu-id="13aed-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="13aed-106">通过使用列表 [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) 返回 [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 对象的集合，可以确定已添加到访问包的资源的访问包资源范围。</span><span class="sxs-lookup"><span data-stu-id="13aed-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="13aed-107">属性</span><span class="sxs-lookup"><span data-stu-id="13aed-107">Properties</span></span>

| <span data-ttu-id="13aed-108">属性</span><span class="sxs-lookup"><span data-stu-id="13aed-108">Property</span></span>     | <span data-ttu-id="13aed-109">类型</span><span class="sxs-lookup"><span data-stu-id="13aed-109">Type</span></span>        | <span data-ttu-id="13aed-110">说明</span><span class="sxs-lookup"><span data-stu-id="13aed-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13aed-111">说明</span><span class="sxs-lookup"><span data-stu-id="13aed-111">description</span></span>|<span data-ttu-id="13aed-112">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-112">String</span></span>|<span data-ttu-id="13aed-113">范围的说明。</span><span class="sxs-lookup"><span data-stu-id="13aed-113">The description of the scope.</span></span>|
|<span data-ttu-id="13aed-114">displayName</span><span class="sxs-lookup"><span data-stu-id="13aed-114">displayName</span></span>|<span data-ttu-id="13aed-115">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-115">String</span></span>|<span data-ttu-id="13aed-116">作用域显示名称的作用域。</span><span class="sxs-lookup"><span data-stu-id="13aed-116">The display name of the scope.</span></span>|
|<span data-ttu-id="13aed-117">id</span><span class="sxs-lookup"><span data-stu-id="13aed-117">id</span></span>|<span data-ttu-id="13aed-118">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-118">String</span></span>| <span data-ttu-id="13aed-119">只读。</span><span class="sxs-lookup"><span data-stu-id="13aed-119">Read-only.</span></span>|
|<span data-ttu-id="13aed-120">isRootScope</span><span class="sxs-lookup"><span data-stu-id="13aed-120">isRootScope</span></span>|<span data-ttu-id="13aed-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="13aed-121">Boolean</span></span>|<span data-ttu-id="13aed-122">如此 如果范围按层次结构排列，并且这是资源的顶部或根范围。</span><span class="sxs-lookup"><span data-stu-id="13aed-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="13aed-123">originId</span><span class="sxs-lookup"><span data-stu-id="13aed-123">originId</span></span>|<span data-ttu-id="13aed-124">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-124">String</span></span>|<span data-ttu-id="13aed-125">资源中范围的唯一标识符，如源系统中定义。</span><span class="sxs-lookup"><span data-stu-id="13aed-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="13aed-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="13aed-126">originSystem</span></span>|<span data-ttu-id="13aed-127">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-127">String</span></span>|<span data-ttu-id="13aed-128">范围的源系统。</span><span class="sxs-lookup"><span data-stu-id="13aed-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="13aed-129">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="13aed-129">roleOriginId</span></span>|<span data-ttu-id="13aed-130">字符串</span><span class="sxs-lookup"><span data-stu-id="13aed-130">String</span></span>|<span data-ttu-id="13aed-131">角色的源系统（如果不同）。</span><span class="sxs-lookup"><span data-stu-id="13aed-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="13aed-132">url</span><span class="sxs-lookup"><span data-stu-id="13aed-132">url</span></span>|<span data-ttu-id="13aed-133">String</span><span class="sxs-lookup"><span data-stu-id="13aed-133">String</span></span>|<span data-ttu-id="13aed-134">范围的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="13aed-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13aed-135">关系</span><span class="sxs-lookup"><span data-stu-id="13aed-135">Relationships</span></span>

| <span data-ttu-id="13aed-136">关系</span><span class="sxs-lookup"><span data-stu-id="13aed-136">Relationship</span></span> | <span data-ttu-id="13aed-137">类型</span><span class="sxs-lookup"><span data-stu-id="13aed-137">Type</span></span>        | <span data-ttu-id="13aed-138">说明</span><span class="sxs-lookup"><span data-stu-id="13aed-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13aed-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="13aed-139">accessPackageResource</span></span>|[<span data-ttu-id="13aed-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="13aed-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="13aed-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="13aed-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13aed-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13aed-143">JSON representation</span></span>

<span data-ttu-id="13aed-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13aed-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


