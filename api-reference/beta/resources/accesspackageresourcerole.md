---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 188504dc96628ba0047f9feb2489e94b8f138874
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158574"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="d4873-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4873-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="d4873-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4873-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4873-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源角色是对资源中定义的角色的引用。</span><span class="sxs-lookup"><span data-stu-id="d4873-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="d4873-106">该引用可在创建访问包后使用，通过创建访问包资源角色作用域来指定访问包应交付到的每个目录 [资源的角色](../api/accesspackage-post-accesspackageresourcerolescopes.md)。</span><span class="sxs-lookup"><span data-stu-id="d4873-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d4873-107">方法</span><span class="sxs-lookup"><span data-stu-id="d4873-107">Methods</span></span>

| <span data-ttu-id="d4873-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4873-108">Method</span></span>       | <span data-ttu-id="d4873-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4873-109">Return Type</span></span> | <span data-ttu-id="d4873-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4873-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4873-111">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="d4873-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="d4873-112">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4873-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="d4873-113">检索目录的 accessPackageResourceRole 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d4873-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4873-114">属性</span><span class="sxs-lookup"><span data-stu-id="d4873-114">Properties</span></span>

| <span data-ttu-id="d4873-115">属性</span><span class="sxs-lookup"><span data-stu-id="d4873-115">Property</span></span>     | <span data-ttu-id="d4873-116">类型</span><span class="sxs-lookup"><span data-stu-id="d4873-116">Type</span></span>        | <span data-ttu-id="d4873-117">说明</span><span class="sxs-lookup"><span data-stu-id="d4873-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4873-118">说明</span><span class="sxs-lookup"><span data-stu-id="d4873-118">description</span></span>|<span data-ttu-id="d4873-119">String</span><span class="sxs-lookup"><span data-stu-id="d4873-119">String</span></span>|<span data-ttu-id="d4873-120">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="d4873-120">A description for the resource role.</span></span>|
|<span data-ttu-id="d4873-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d4873-121">displayName</span></span>|<span data-ttu-id="d4873-122">String</span><span class="sxs-lookup"><span data-stu-id="d4873-122">String</span></span>|<span data-ttu-id="d4873-123">资源显示名称角色（如应用程序定义的角色）的组。</span><span class="sxs-lookup"><span data-stu-id="d4873-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="d4873-124">id</span><span class="sxs-lookup"><span data-stu-id="d4873-124">id</span></span>|<span data-ttu-id="d4873-125">String</span><span class="sxs-lookup"><span data-stu-id="d4873-125">String</span></span>| <span data-ttu-id="d4873-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d4873-126">Read-only.</span></span>|
|<span data-ttu-id="d4873-127">originId</span><span class="sxs-lookup"><span data-stu-id="d4873-127">originId</span></span>|<span data-ttu-id="d4873-128">String</span><span class="sxs-lookup"><span data-stu-id="d4873-128">String</span></span>|<span data-ttu-id="d4873-129">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d4873-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="d4873-130">originSystem</span><span class="sxs-lookup"><span data-stu-id="d4873-130">originSystem</span></span>|<span data-ttu-id="d4873-131">String</span><span class="sxs-lookup"><span data-stu-id="d4873-131">String</span></span>|<span data-ttu-id="d4873-132">源系统中资源的类型，例如 `SharePointOnline` ， `AadApplication` 或 `AadGroup` 。</span><span class="sxs-lookup"><span data-stu-id="d4873-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4873-133">关系</span><span class="sxs-lookup"><span data-stu-id="d4873-133">Relationships</span></span>

| <span data-ttu-id="d4873-134">关系</span><span class="sxs-lookup"><span data-stu-id="d4873-134">Relationship</span></span> | <span data-ttu-id="d4873-135">类型</span><span class="sxs-lookup"><span data-stu-id="d4873-135">Type</span></span>        | <span data-ttu-id="d4873-136">说明</span><span class="sxs-lookup"><span data-stu-id="d4873-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4873-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="d4873-137">accessPackageResource</span></span>|[<span data-ttu-id="d4873-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="d4873-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="d4873-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="d4873-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4873-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4873-141">JSON representation</span></span>

<span data-ttu-id="d4873-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4873-142">The following is a JSON representation of the resource.</span></span>

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


