---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1194c27e929a14f738384441ab57f5090d8b1149
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401597"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="da1b2-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="da1b2-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="da1b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da1b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1b2-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源角色是资源中定义的角色的引用。</span><span class="sxs-lookup"><span data-stu-id="da1b2-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="da1b2-106">该引用可在创建访问包后使用，以通过创建访问包资源角色作用域来指定访问包应交付到其中 [的每个目录资源的角色](../api/accesspackage-post-accesspackageresourcerolescopes.md)。</span><span class="sxs-lookup"><span data-stu-id="da1b2-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="da1b2-107">方法</span><span class="sxs-lookup"><span data-stu-id="da1b2-107">Methods</span></span>

| <span data-ttu-id="da1b2-108">方法</span><span class="sxs-lookup"><span data-stu-id="da1b2-108">Method</span></span>       | <span data-ttu-id="da1b2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="da1b2-109">Return Type</span></span> | <span data-ttu-id="da1b2-110">说明</span><span class="sxs-lookup"><span data-stu-id="da1b2-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da1b2-111">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="da1b2-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="da1b2-112">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da1b2-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="da1b2-113">检索目录的 accessPackageResourceRole 对象列表。</span><span class="sxs-lookup"><span data-stu-id="da1b2-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="da1b2-114">属性</span><span class="sxs-lookup"><span data-stu-id="da1b2-114">Properties</span></span>

| <span data-ttu-id="da1b2-115">属性</span><span class="sxs-lookup"><span data-stu-id="da1b2-115">Property</span></span>     | <span data-ttu-id="da1b2-116">类型</span><span class="sxs-lookup"><span data-stu-id="da1b2-116">Type</span></span>        | <span data-ttu-id="da1b2-117">说明</span><span class="sxs-lookup"><span data-stu-id="da1b2-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da1b2-118">说明</span><span class="sxs-lookup"><span data-stu-id="da1b2-118">description</span></span>|<span data-ttu-id="da1b2-119">String</span><span class="sxs-lookup"><span data-stu-id="da1b2-119">String</span></span>|<span data-ttu-id="da1b2-120">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="da1b2-120">A description for the resource role.</span></span>|
|<span data-ttu-id="da1b2-121">displayName</span><span class="sxs-lookup"><span data-stu-id="da1b2-121">displayName</span></span>|<span data-ttu-id="da1b2-122">String</span><span class="sxs-lookup"><span data-stu-id="da1b2-122">String</span></span>|<span data-ttu-id="da1b2-123">资源显示名称角色（如应用程序定义的角色）的组。</span><span class="sxs-lookup"><span data-stu-id="da1b2-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="da1b2-124">id</span><span class="sxs-lookup"><span data-stu-id="da1b2-124">id</span></span>|<span data-ttu-id="da1b2-125">String</span><span class="sxs-lookup"><span data-stu-id="da1b2-125">String</span></span>| <span data-ttu-id="da1b2-126">只读。</span><span class="sxs-lookup"><span data-stu-id="da1b2-126">Read-only.</span></span>|
|<span data-ttu-id="da1b2-127">originId</span><span class="sxs-lookup"><span data-stu-id="da1b2-127">originId</span></span>|<span data-ttu-id="da1b2-128">String</span><span class="sxs-lookup"><span data-stu-id="da1b2-128">String</span></span>|<span data-ttu-id="da1b2-129">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="da1b2-129">The unique identifier of the resource role in the origin system.</span></span> <span data-ttu-id="da1b2-130">对于 SharePoint Online 网站，originId 将是网站中角色的序列号。</span><span class="sxs-lookup"><span data-stu-id="da1b2-130">For a SharePoint Online site, the originId will be the sequence number of the role in the site.</span></span> |
|<span data-ttu-id="da1b2-131">originSystem</span><span class="sxs-lookup"><span data-stu-id="da1b2-131">originSystem</span></span>|<span data-ttu-id="da1b2-132">String</span><span class="sxs-lookup"><span data-stu-id="da1b2-132">String</span></span>|<span data-ttu-id="da1b2-133">源系统中资源的类型，如 `SharePointOnline` 或 `AadApplication` `AadGroup` 。</span><span class="sxs-lookup"><span data-stu-id="da1b2-133">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da1b2-134">关系</span><span class="sxs-lookup"><span data-stu-id="da1b2-134">Relationships</span></span>

| <span data-ttu-id="da1b2-135">关系</span><span class="sxs-lookup"><span data-stu-id="da1b2-135">Relationship</span></span> | <span data-ttu-id="da1b2-136">类型</span><span class="sxs-lookup"><span data-stu-id="da1b2-136">Type</span></span>        | <span data-ttu-id="da1b2-137">说明</span><span class="sxs-lookup"><span data-stu-id="da1b2-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da1b2-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="da1b2-138">accessPackageResource</span></span>|[<span data-ttu-id="da1b2-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="da1b2-139">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="da1b2-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="da1b2-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da1b2-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da1b2-142">JSON representation</span></span>

<span data-ttu-id="da1b2-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da1b2-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


