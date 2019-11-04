---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权限管理中，访问包资源作用域是对资源中的范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7bfa2f617e746aee17a62a7550c41e3de54f47cd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939514"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="12c31-103">accessPackageResourceScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="12c31-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12c31-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源作用域是对包含多个作用域的资源中的范围的引用。</span><span class="sxs-lookup"><span data-stu-id="12c31-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="12c31-105">属性</span><span class="sxs-lookup"><span data-stu-id="12c31-105">Properties</span></span>

| <span data-ttu-id="12c31-106">属性</span><span class="sxs-lookup"><span data-stu-id="12c31-106">Property</span></span>     | <span data-ttu-id="12c31-107">类型</span><span class="sxs-lookup"><span data-stu-id="12c31-107">Type</span></span>        | <span data-ttu-id="12c31-108">说明</span><span class="sxs-lookup"><span data-stu-id="12c31-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12c31-109">说明</span><span class="sxs-lookup"><span data-stu-id="12c31-109">description</span></span>|<span data-ttu-id="12c31-110">String</span><span class="sxs-lookup"><span data-stu-id="12c31-110">String</span></span>|<span data-ttu-id="12c31-111">作用域的说明。</span><span class="sxs-lookup"><span data-stu-id="12c31-111">The description of the scope.</span></span>|
|<span data-ttu-id="12c31-112">displayName</span><span class="sxs-lookup"><span data-stu-id="12c31-112">displayName</span></span>|<span data-ttu-id="12c31-113">字符串</span><span class="sxs-lookup"><span data-stu-id="12c31-113">String</span></span>|<span data-ttu-id="12c31-114">作用域的显示名称。</span><span class="sxs-lookup"><span data-stu-id="12c31-114">The display name of the scope.</span></span>|
|<span data-ttu-id="12c31-115">id</span><span class="sxs-lookup"><span data-stu-id="12c31-115">id</span></span>|<span data-ttu-id="12c31-116">字符串</span><span class="sxs-lookup"><span data-stu-id="12c31-116">String</span></span>| <span data-ttu-id="12c31-117">只读。</span><span class="sxs-lookup"><span data-stu-id="12c31-117">Read-only.</span></span>|
|<span data-ttu-id="12c31-118">isRootScope</span><span class="sxs-lookup"><span data-stu-id="12c31-118">isRootScope</span></span>|<span data-ttu-id="12c31-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="12c31-119">Boolean</span></span>|<span data-ttu-id="12c31-120">如此如果作用域在层次结构中排列，这是资源的顶部或根作用域。</span><span class="sxs-lookup"><span data-stu-id="12c31-120">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="12c31-121">originId</span><span class="sxs-lookup"><span data-stu-id="12c31-121">originId</span></span>|<span data-ttu-id="12c31-122">字符串</span><span class="sxs-lookup"><span data-stu-id="12c31-122">String</span></span>|<span data-ttu-id="12c31-123">在源系统中定义的资源中的范围的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12c31-123">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="12c31-124">originSystem</span><span class="sxs-lookup"><span data-stu-id="12c31-124">originSystem</span></span>|<span data-ttu-id="12c31-125">字符串</span><span class="sxs-lookup"><span data-stu-id="12c31-125">String</span></span>|<span data-ttu-id="12c31-126">作用域的源系统。</span><span class="sxs-lookup"><span data-stu-id="12c31-126">The origin system for the scope.</span></span>|
|<span data-ttu-id="12c31-127">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="12c31-127">roleOriginId</span></span>|<span data-ttu-id="12c31-128">字符串</span><span class="sxs-lookup"><span data-stu-id="12c31-128">String</span></span>|<span data-ttu-id="12c31-129">角色的原始系统（如果不同）。</span><span class="sxs-lookup"><span data-stu-id="12c31-129">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="12c31-130">url</span><span class="sxs-lookup"><span data-stu-id="12c31-130">url</span></span>|<span data-ttu-id="12c31-131">String</span><span class="sxs-lookup"><span data-stu-id="12c31-131">String</span></span>|<span data-ttu-id="12c31-132">作用域的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="12c31-132">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12c31-133">关系</span><span class="sxs-lookup"><span data-stu-id="12c31-133">Relationships</span></span>

| <span data-ttu-id="12c31-134">关系</span><span class="sxs-lookup"><span data-stu-id="12c31-134">Relationship</span></span> | <span data-ttu-id="12c31-135">类型</span><span class="sxs-lookup"><span data-stu-id="12c31-135">Type</span></span>        | <span data-ttu-id="12c31-136">描述</span><span class="sxs-lookup"><span data-stu-id="12c31-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12c31-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="12c31-137">accessPackageResource</span></span>|[<span data-ttu-id="12c31-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="12c31-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="12c31-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="12c31-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12c31-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12c31-141">JSON representation</span></span>

<span data-ttu-id="12c31-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12c31-142">The following is a JSON representation of the resource.</span></span>

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
