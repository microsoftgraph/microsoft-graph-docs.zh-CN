---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权利管理中，访问包资源范围是资源内范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6da0211cad6dcca225f4c9848216eda2deaf7b0a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467174"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="63616-103">accessPackageResourceScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="63616-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="63616-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63616-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63616-105">在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包资源范围是资源中对具有多个范围的资源的作用域的引用。</span><span class="sxs-lookup"><span data-stu-id="63616-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="63616-106">通过使用 list [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) 返回 [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 对象的集合，可以确定访问包资源作用域（对于已将角色添加到访问包的资源）。</span><span class="sxs-lookup"><span data-stu-id="63616-106">You can determine the access package resource scope, for a resource which has roles already added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

<span data-ttu-id="63616-107">如果资源位于访问包目录中，但尚未将其角色添加到访问包中，则可以通过使用 [列表 accessPackageResources（](../api/accesspackagecatalog-list-accesspackageresources.md) 包括查询中）来确定访问包资源 `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` 范围。</span><span class="sxs-lookup"><span data-stu-id="63616-107">If the resource is in an access package catalog but has not yet had its roles added to an access package, you can determine the access package resource scope by using [list accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) and including `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span>

## <a name="properties"></a><span data-ttu-id="63616-108">属性</span><span class="sxs-lookup"><span data-stu-id="63616-108">Properties</span></span>

| <span data-ttu-id="63616-109">属性</span><span class="sxs-lookup"><span data-stu-id="63616-109">Property</span></span>     | <span data-ttu-id="63616-110">类型</span><span class="sxs-lookup"><span data-stu-id="63616-110">Type</span></span>        | <span data-ttu-id="63616-111">说明</span><span class="sxs-lookup"><span data-stu-id="63616-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63616-112">说明</span><span class="sxs-lookup"><span data-stu-id="63616-112">description</span></span>|<span data-ttu-id="63616-113">String</span><span class="sxs-lookup"><span data-stu-id="63616-113">String</span></span>|<span data-ttu-id="63616-114">范围的说明。</span><span class="sxs-lookup"><span data-stu-id="63616-114">The description of the scope.</span></span>|
|<span data-ttu-id="63616-115">displayName</span><span class="sxs-lookup"><span data-stu-id="63616-115">displayName</span></span>|<span data-ttu-id="63616-116">String</span><span class="sxs-lookup"><span data-stu-id="63616-116">String</span></span>|<span data-ttu-id="63616-117">作用域显示名称。</span><span class="sxs-lookup"><span data-stu-id="63616-117">The display name of the scope.</span></span>|
|<span data-ttu-id="63616-118">id</span><span class="sxs-lookup"><span data-stu-id="63616-118">id</span></span>|<span data-ttu-id="63616-119">String</span><span class="sxs-lookup"><span data-stu-id="63616-119">String</span></span>| <span data-ttu-id="63616-120">只读。</span><span class="sxs-lookup"><span data-stu-id="63616-120">Read-only.</span></span>|
|<span data-ttu-id="63616-121">isRootScope</span><span class="sxs-lookup"><span data-stu-id="63616-121">isRootScope</span></span>|<span data-ttu-id="63616-122">布尔</span><span class="sxs-lookup"><span data-stu-id="63616-122">Boolean</span></span>|<span data-ttu-id="63616-123">如此 如果按层次结构排列范围，并且这是资源的顶部或根范围。</span><span class="sxs-lookup"><span data-stu-id="63616-123">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="63616-124">originId</span><span class="sxs-lookup"><span data-stu-id="63616-124">originId</span></span>|<span data-ttu-id="63616-125">String</span><span class="sxs-lookup"><span data-stu-id="63616-125">String</span></span>|<span data-ttu-id="63616-126">资源中范围的唯一标识符，如源系统中定义。</span><span class="sxs-lookup"><span data-stu-id="63616-126">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="63616-127">originSystem</span><span class="sxs-lookup"><span data-stu-id="63616-127">originSystem</span></span>|<span data-ttu-id="63616-128">String</span><span class="sxs-lookup"><span data-stu-id="63616-128">String</span></span>|<span data-ttu-id="63616-129">作用域的源系统。</span><span class="sxs-lookup"><span data-stu-id="63616-129">The origin system for the scope.</span></span>|
|<span data-ttu-id="63616-130">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="63616-130">roleOriginId</span></span>|<span data-ttu-id="63616-131">String</span><span class="sxs-lookup"><span data-stu-id="63616-131">String</span></span>|<span data-ttu-id="63616-132">角色的源系统（如果不同）。</span><span class="sxs-lookup"><span data-stu-id="63616-132">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="63616-133">url</span><span class="sxs-lookup"><span data-stu-id="63616-133">url</span></span>|<span data-ttu-id="63616-134">String</span><span class="sxs-lookup"><span data-stu-id="63616-134">String</span></span>|<span data-ttu-id="63616-135">范围的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="63616-135">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63616-136">关系</span><span class="sxs-lookup"><span data-stu-id="63616-136">Relationships</span></span>

| <span data-ttu-id="63616-137">关系</span><span class="sxs-lookup"><span data-stu-id="63616-137">Relationship</span></span> | <span data-ttu-id="63616-138">类型</span><span class="sxs-lookup"><span data-stu-id="63616-138">Type</span></span>        | <span data-ttu-id="63616-139">说明</span><span class="sxs-lookup"><span data-stu-id="63616-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63616-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="63616-140">accessPackageResource</span></span>|[<span data-ttu-id="63616-141">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="63616-141">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="63616-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="63616-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63616-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63616-144">JSON representation</span></span>

<span data-ttu-id="63616-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63616-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
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


