---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bc0a60043c9877b4c48a889f93fa48a852c3780
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319581"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="1aca0-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aca0-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="1aca0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aca0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aca0-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色是对资源中定义的角色的引用。</span><span class="sxs-lookup"><span data-stu-id="1aca0-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="1aca0-106">创建访问包时，可以使用该引用来指定访问包应传递到的每个目录资源的角色，方法是 [创建访问包资源角色作用域](../api/accesspackage-post-accesspackageresourcerolescopes.md)。</span><span class="sxs-lookup"><span data-stu-id="1aca0-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1aca0-107">方法</span><span class="sxs-lookup"><span data-stu-id="1aca0-107">Methods</span></span>

| <span data-ttu-id="1aca0-108">方法</span><span class="sxs-lookup"><span data-stu-id="1aca0-108">Method</span></span>       | <span data-ttu-id="1aca0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1aca0-109">Return Type</span></span> | <span data-ttu-id="1aca0-110">说明</span><span class="sxs-lookup"><span data-stu-id="1aca0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1aca0-111">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="1aca0-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="1aca0-112">[accessPackageResourceRole](accesspackageresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1aca0-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="1aca0-113">检索目录的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1aca0-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="1aca0-114">属性</span><span class="sxs-lookup"><span data-stu-id="1aca0-114">Properties</span></span>

| <span data-ttu-id="1aca0-115">属性</span><span class="sxs-lookup"><span data-stu-id="1aca0-115">Property</span></span>     | <span data-ttu-id="1aca0-116">类型</span><span class="sxs-lookup"><span data-stu-id="1aca0-116">Type</span></span>        | <span data-ttu-id="1aca0-117">说明</span><span class="sxs-lookup"><span data-stu-id="1aca0-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1aca0-118">说明</span><span class="sxs-lookup"><span data-stu-id="1aca0-118">description</span></span>|<span data-ttu-id="1aca0-119">String</span><span class="sxs-lookup"><span data-stu-id="1aca0-119">String</span></span>|<span data-ttu-id="1aca0-120">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="1aca0-120">A description for the resource role.</span></span>|
|<span data-ttu-id="1aca0-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1aca0-121">displayName</span></span>|<span data-ttu-id="1aca0-122">String</span><span class="sxs-lookup"><span data-stu-id="1aca0-122">String</span></span>|<span data-ttu-id="1aca0-123">资源角色的显示名称，例如应用程序定义的角色。</span><span class="sxs-lookup"><span data-stu-id="1aca0-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="1aca0-124">id</span><span class="sxs-lookup"><span data-stu-id="1aca0-124">id</span></span>|<span data-ttu-id="1aca0-125">String</span><span class="sxs-lookup"><span data-stu-id="1aca0-125">String</span></span>| <span data-ttu-id="1aca0-126">只读。</span><span class="sxs-lookup"><span data-stu-id="1aca0-126">Read-only.</span></span>|
|<span data-ttu-id="1aca0-127">originId</span><span class="sxs-lookup"><span data-stu-id="1aca0-127">originId</span></span>|<span data-ttu-id="1aca0-128">String</span><span class="sxs-lookup"><span data-stu-id="1aca0-128">String</span></span>|<span data-ttu-id="1aca0-129">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1aca0-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="1aca0-130">originSystem</span><span class="sxs-lookup"><span data-stu-id="1aca0-130">originSystem</span></span>|<span data-ttu-id="1aca0-131">String</span><span class="sxs-lookup"><span data-stu-id="1aca0-131">String</span></span>|<span data-ttu-id="1aca0-132">源系统中资源的类型，例如 `SharePointOnline` `AadApplication` 或 `AadGroup` 。</span><span class="sxs-lookup"><span data-stu-id="1aca0-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aca0-133">关系</span><span class="sxs-lookup"><span data-stu-id="1aca0-133">Relationships</span></span>

| <span data-ttu-id="1aca0-134">关系</span><span class="sxs-lookup"><span data-stu-id="1aca0-134">Relationship</span></span> | <span data-ttu-id="1aca0-135">类型</span><span class="sxs-lookup"><span data-stu-id="1aca0-135">Type</span></span>        | <span data-ttu-id="1aca0-136">说明</span><span class="sxs-lookup"><span data-stu-id="1aca0-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1aca0-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1aca0-137">accessPackageResource</span></span>|[<span data-ttu-id="1aca0-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1aca0-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="1aca0-p102">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="1aca0-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1aca0-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aca0-141">JSON representation</span></span>

<span data-ttu-id="1aca0-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aca0-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
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
