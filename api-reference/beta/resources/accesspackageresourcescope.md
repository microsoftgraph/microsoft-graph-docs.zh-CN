---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权限管理中，访问包资源作用域是对资源中的范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1418e2cb21a1023e864d842b760006e05f3afb03
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870962"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="e558c-103">accessPackageResourceScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="e558c-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e558c-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源作用域是对包含多个作用域的资源中的范围的引用。</span><span class="sxs-lookup"><span data-stu-id="e558c-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="e558c-105">您可以通过使用[List accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md)返回[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)对象的集合，来确定已添加到 access 程序包的资源的访问包资源范围。</span><span class="sxs-lookup"><span data-stu-id="e558c-105">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="e558c-106">属性</span><span class="sxs-lookup"><span data-stu-id="e558c-106">Properties</span></span>

| <span data-ttu-id="e558c-107">属性</span><span class="sxs-lookup"><span data-stu-id="e558c-107">Property</span></span>     | <span data-ttu-id="e558c-108">类型</span><span class="sxs-lookup"><span data-stu-id="e558c-108">Type</span></span>        | <span data-ttu-id="e558c-109">说明</span><span class="sxs-lookup"><span data-stu-id="e558c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e558c-110">说明</span><span class="sxs-lookup"><span data-stu-id="e558c-110">description</span></span>|<span data-ttu-id="e558c-111">String</span><span class="sxs-lookup"><span data-stu-id="e558c-111">String</span></span>|<span data-ttu-id="e558c-112">作用域的说明。</span><span class="sxs-lookup"><span data-stu-id="e558c-112">The description of the scope.</span></span>|
|<span data-ttu-id="e558c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e558c-113">displayName</span></span>|<span data-ttu-id="e558c-114">字符串</span><span class="sxs-lookup"><span data-stu-id="e558c-114">String</span></span>|<span data-ttu-id="e558c-115">作用域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e558c-115">The display name of the scope.</span></span>|
|<span data-ttu-id="e558c-116">id</span><span class="sxs-lookup"><span data-stu-id="e558c-116">id</span></span>|<span data-ttu-id="e558c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="e558c-117">String</span></span>| <span data-ttu-id="e558c-118">只读。</span><span class="sxs-lookup"><span data-stu-id="e558c-118">Read-only.</span></span>|
|<span data-ttu-id="e558c-119">isRootScope</span><span class="sxs-lookup"><span data-stu-id="e558c-119">isRootScope</span></span>|<span data-ttu-id="e558c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e558c-120">Boolean</span></span>|<span data-ttu-id="e558c-121">如此如果作用域在层次结构中排列，这是资源的顶部或根作用域。</span><span class="sxs-lookup"><span data-stu-id="e558c-121">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="e558c-122">originId</span><span class="sxs-lookup"><span data-stu-id="e558c-122">originId</span></span>|<span data-ttu-id="e558c-123">String</span><span class="sxs-lookup"><span data-stu-id="e558c-123">String</span></span>|<span data-ttu-id="e558c-124">在源系统中定义的资源中的范围的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e558c-124">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="e558c-125">originSystem</span><span class="sxs-lookup"><span data-stu-id="e558c-125">originSystem</span></span>|<span data-ttu-id="e558c-126">String</span><span class="sxs-lookup"><span data-stu-id="e558c-126">String</span></span>|<span data-ttu-id="e558c-127">作用域的源系统。</span><span class="sxs-lookup"><span data-stu-id="e558c-127">The origin system for the scope.</span></span>|
|<span data-ttu-id="e558c-128">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="e558c-128">roleOriginId</span></span>|<span data-ttu-id="e558c-129">String</span><span class="sxs-lookup"><span data-stu-id="e558c-129">String</span></span>|<span data-ttu-id="e558c-130">角色的原始系统（如果不同）。</span><span class="sxs-lookup"><span data-stu-id="e558c-130">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="e558c-131">url</span><span class="sxs-lookup"><span data-stu-id="e558c-131">url</span></span>|<span data-ttu-id="e558c-132">String</span><span class="sxs-lookup"><span data-stu-id="e558c-132">String</span></span>|<span data-ttu-id="e558c-133">作用域的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="e558c-133">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e558c-134">关系</span><span class="sxs-lookup"><span data-stu-id="e558c-134">Relationships</span></span>

| <span data-ttu-id="e558c-135">关系</span><span class="sxs-lookup"><span data-stu-id="e558c-135">Relationship</span></span> | <span data-ttu-id="e558c-136">类型</span><span class="sxs-lookup"><span data-stu-id="e558c-136">Type</span></span>        | <span data-ttu-id="e558c-137">说明</span><span class="sxs-lookup"><span data-stu-id="e558c-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e558c-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e558c-138">accessPackageResource</span></span>|[<span data-ttu-id="e558c-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e558c-139">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="e558c-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e558c-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e558c-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e558c-142">JSON representation</span></span>

<span data-ttu-id="e558c-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e558c-143">The following is a JSON representation of the resource.</span></span>

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
