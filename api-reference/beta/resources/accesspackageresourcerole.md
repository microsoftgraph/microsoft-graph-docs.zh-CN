---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5ab0cc6e2179adb62316cbcdc06b7dd52abc439
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508511"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="82209-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="82209-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="82209-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="82209-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82209-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色是对在资源中定义的角色的引用，可在 access 程序包中使用。</span><span class="sxs-lookup"><span data-stu-id="82209-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="82209-106">方法</span><span class="sxs-lookup"><span data-stu-id="82209-106">Methods</span></span>

| <span data-ttu-id="82209-107">方法</span><span class="sxs-lookup"><span data-stu-id="82209-107">Method</span></span>       | <span data-ttu-id="82209-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="82209-108">Return Type</span></span> | <span data-ttu-id="82209-109">说明</span><span class="sxs-lookup"><span data-stu-id="82209-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="82209-110">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="82209-110">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="82209-111">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="82209-111">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="82209-112">检索目录的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="82209-112">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="82209-113">属性</span><span class="sxs-lookup"><span data-stu-id="82209-113">Properties</span></span>

| <span data-ttu-id="82209-114">属性</span><span class="sxs-lookup"><span data-stu-id="82209-114">Property</span></span>     | <span data-ttu-id="82209-115">类型</span><span class="sxs-lookup"><span data-stu-id="82209-115">Type</span></span>        | <span data-ttu-id="82209-116">说明</span><span class="sxs-lookup"><span data-stu-id="82209-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82209-117">说明</span><span class="sxs-lookup"><span data-stu-id="82209-117">description</span></span>|<span data-ttu-id="82209-118">String</span><span class="sxs-lookup"><span data-stu-id="82209-118">String</span></span>|<span data-ttu-id="82209-119">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="82209-119">A description for the resource role.</span></span>|
|<span data-ttu-id="82209-120">displayName</span><span class="sxs-lookup"><span data-stu-id="82209-120">displayName</span></span>|<span data-ttu-id="82209-121">String</span><span class="sxs-lookup"><span data-stu-id="82209-121">String</span></span>|<span data-ttu-id="82209-122">资源角色的显示名称，例如应用程序定义的角色。</span><span class="sxs-lookup"><span data-stu-id="82209-122">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="82209-123">id</span><span class="sxs-lookup"><span data-stu-id="82209-123">id</span></span>|<span data-ttu-id="82209-124">字符串</span><span class="sxs-lookup"><span data-stu-id="82209-124">String</span></span>| <span data-ttu-id="82209-125">只读。</span><span class="sxs-lookup"><span data-stu-id="82209-125">Read-only.</span></span>|
|<span data-ttu-id="82209-126">originId</span><span class="sxs-lookup"><span data-stu-id="82209-126">originId</span></span>|<span data-ttu-id="82209-127">String</span><span class="sxs-lookup"><span data-stu-id="82209-127">String</span></span>|<span data-ttu-id="82209-128">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82209-128">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="82209-129">originSystem</span><span class="sxs-lookup"><span data-stu-id="82209-129">originSystem</span></span>|<span data-ttu-id="82209-130">String</span><span class="sxs-lookup"><span data-stu-id="82209-130">String</span></span>|<span data-ttu-id="82209-131">源系统中资源的类型。</span><span class="sxs-lookup"><span data-stu-id="82209-131">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82209-132">关系</span><span class="sxs-lookup"><span data-stu-id="82209-132">Relationships</span></span>

| <span data-ttu-id="82209-133">关系</span><span class="sxs-lookup"><span data-stu-id="82209-133">Relationship</span></span> | <span data-ttu-id="82209-134">类型</span><span class="sxs-lookup"><span data-stu-id="82209-134">Type</span></span>        | <span data-ttu-id="82209-135">说明</span><span class="sxs-lookup"><span data-stu-id="82209-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82209-136">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="82209-136">accessPackageResource</span></span>|[<span data-ttu-id="82209-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="82209-137">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="82209-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="82209-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82209-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82209-140">JSON representation</span></span>

<span data-ttu-id="82209-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82209-141">The following is a JSON representation of the resource.</span></span>

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
