---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权限管理中，访问包资源作用域是对资源中的范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 242c90e9d0e506dbeb6576975305d0a0f8397f86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508497"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="920d4-103">accessPackageResourceScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="920d4-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="920d4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="920d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="920d4-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源作用域是对包含多个作用域的资源中的范围的引用。</span><span class="sxs-lookup"><span data-stu-id="920d4-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="920d4-106">您可以通过使用[List accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md)返回[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)对象的集合，来确定已添加到 access 程序包的资源的访问包资源范围。</span><span class="sxs-lookup"><span data-stu-id="920d4-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="920d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="920d4-107">Properties</span></span>

| <span data-ttu-id="920d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="920d4-108">Property</span></span>     | <span data-ttu-id="920d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="920d4-109">Type</span></span>        | <span data-ttu-id="920d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="920d4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="920d4-111">说明</span><span class="sxs-lookup"><span data-stu-id="920d4-111">description</span></span>|<span data-ttu-id="920d4-112">String</span><span class="sxs-lookup"><span data-stu-id="920d4-112">String</span></span>|<span data-ttu-id="920d4-113">作用域的说明。</span><span class="sxs-lookup"><span data-stu-id="920d4-113">The description of the scope.</span></span>|
|<span data-ttu-id="920d4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="920d4-114">displayName</span></span>|<span data-ttu-id="920d4-115">字符串</span><span class="sxs-lookup"><span data-stu-id="920d4-115">String</span></span>|<span data-ttu-id="920d4-116">作用域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="920d4-116">The display name of the scope.</span></span>|
|<span data-ttu-id="920d4-117">id</span><span class="sxs-lookup"><span data-stu-id="920d4-117">id</span></span>|<span data-ttu-id="920d4-118">字符串</span><span class="sxs-lookup"><span data-stu-id="920d4-118">String</span></span>| <span data-ttu-id="920d4-119">只读。</span><span class="sxs-lookup"><span data-stu-id="920d4-119">Read-only.</span></span>|
|<span data-ttu-id="920d4-120">isRootScope</span><span class="sxs-lookup"><span data-stu-id="920d4-120">isRootScope</span></span>|<span data-ttu-id="920d4-121">布尔</span><span class="sxs-lookup"><span data-stu-id="920d4-121">Boolean</span></span>|<span data-ttu-id="920d4-122">如此如果作用域在层次结构中排列，这是资源的顶部或根作用域。</span><span class="sxs-lookup"><span data-stu-id="920d4-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="920d4-123">originId</span><span class="sxs-lookup"><span data-stu-id="920d4-123">originId</span></span>|<span data-ttu-id="920d4-124">String</span><span class="sxs-lookup"><span data-stu-id="920d4-124">String</span></span>|<span data-ttu-id="920d4-125">在源系统中定义的资源中的范围的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="920d4-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="920d4-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="920d4-126">originSystem</span></span>|<span data-ttu-id="920d4-127">String</span><span class="sxs-lookup"><span data-stu-id="920d4-127">String</span></span>|<span data-ttu-id="920d4-128">作用域的源系统。</span><span class="sxs-lookup"><span data-stu-id="920d4-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="920d4-129">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="920d4-129">roleOriginId</span></span>|<span data-ttu-id="920d4-130">String</span><span class="sxs-lookup"><span data-stu-id="920d4-130">String</span></span>|<span data-ttu-id="920d4-131">角色的原始系统（如果不同）。</span><span class="sxs-lookup"><span data-stu-id="920d4-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="920d4-132">url</span><span class="sxs-lookup"><span data-stu-id="920d4-132">url</span></span>|<span data-ttu-id="920d4-133">String</span><span class="sxs-lookup"><span data-stu-id="920d4-133">String</span></span>|<span data-ttu-id="920d4-134">作用域的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="920d4-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="920d4-135">关系</span><span class="sxs-lookup"><span data-stu-id="920d4-135">Relationships</span></span>

| <span data-ttu-id="920d4-136">关系</span><span class="sxs-lookup"><span data-stu-id="920d4-136">Relationship</span></span> | <span data-ttu-id="920d4-137">类型</span><span class="sxs-lookup"><span data-stu-id="920d4-137">Type</span></span>        | <span data-ttu-id="920d4-138">说明</span><span class="sxs-lookup"><span data-stu-id="920d4-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="920d4-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="920d4-139">accessPackageResource</span></span>|[<span data-ttu-id="920d4-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="920d4-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="920d4-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="920d4-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="920d4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="920d4-143">JSON representation</span></span>

<span data-ttu-id="920d4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="920d4-144">The following is a JSON representation of the resource.</span></span>

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
