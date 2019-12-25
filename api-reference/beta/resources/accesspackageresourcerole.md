---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21cda352cb887a377248a3fbbf16a761773128ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870422"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="e7229-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7229-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7229-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色是对在资源中定义的角色的引用，可在 access 程序包中使用。</span><span class="sxs-lookup"><span data-stu-id="e7229-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="e7229-105">方法</span><span class="sxs-lookup"><span data-stu-id="e7229-105">Methods</span></span>

| <span data-ttu-id="e7229-106">方法</span><span class="sxs-lookup"><span data-stu-id="e7229-106">Method</span></span>       | <span data-ttu-id="e7229-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7229-107">Return Type</span></span> | <span data-ttu-id="e7229-108">说明</span><span class="sxs-lookup"><span data-stu-id="e7229-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7229-109">列出 accessPackageCatalog 资源角色</span><span class="sxs-lookup"><span data-stu-id="e7229-109">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="e7229-110">[accessPackageResourceRole](accesspackageresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="e7229-110">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="e7229-111">检索目录的 accessPackageResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e7229-111">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7229-112">属性</span><span class="sxs-lookup"><span data-stu-id="e7229-112">Properties</span></span>

| <span data-ttu-id="e7229-113">属性</span><span class="sxs-lookup"><span data-stu-id="e7229-113">Property</span></span>     | <span data-ttu-id="e7229-114">类型</span><span class="sxs-lookup"><span data-stu-id="e7229-114">Type</span></span>        | <span data-ttu-id="e7229-115">说明</span><span class="sxs-lookup"><span data-stu-id="e7229-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7229-116">说明</span><span class="sxs-lookup"><span data-stu-id="e7229-116">description</span></span>|<span data-ttu-id="e7229-117">String</span><span class="sxs-lookup"><span data-stu-id="e7229-117">String</span></span>|<span data-ttu-id="e7229-118">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="e7229-118">A description for the resource role.</span></span>|
|<span data-ttu-id="e7229-119">displayName</span><span class="sxs-lookup"><span data-stu-id="e7229-119">displayName</span></span>|<span data-ttu-id="e7229-120">String</span><span class="sxs-lookup"><span data-stu-id="e7229-120">String</span></span>|<span data-ttu-id="e7229-121">资源角色的显示名称，例如应用程序定义的角色。</span><span class="sxs-lookup"><span data-stu-id="e7229-121">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="e7229-122">id</span><span class="sxs-lookup"><span data-stu-id="e7229-122">id</span></span>|<span data-ttu-id="e7229-123">字符串</span><span class="sxs-lookup"><span data-stu-id="e7229-123">String</span></span>| <span data-ttu-id="e7229-124">只读。</span><span class="sxs-lookup"><span data-stu-id="e7229-124">Read-only.</span></span>|
|<span data-ttu-id="e7229-125">originId</span><span class="sxs-lookup"><span data-stu-id="e7229-125">originId</span></span>|<span data-ttu-id="e7229-126">String</span><span class="sxs-lookup"><span data-stu-id="e7229-126">String</span></span>|<span data-ttu-id="e7229-127">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e7229-127">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="e7229-128">originSystem</span><span class="sxs-lookup"><span data-stu-id="e7229-128">originSystem</span></span>|<span data-ttu-id="e7229-129">String</span><span class="sxs-lookup"><span data-stu-id="e7229-129">String</span></span>|<span data-ttu-id="e7229-130">源系统中资源的类型。</span><span class="sxs-lookup"><span data-stu-id="e7229-130">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7229-131">关系</span><span class="sxs-lookup"><span data-stu-id="e7229-131">Relationships</span></span>

| <span data-ttu-id="e7229-132">关系</span><span class="sxs-lookup"><span data-stu-id="e7229-132">Relationship</span></span> | <span data-ttu-id="e7229-133">类型</span><span class="sxs-lookup"><span data-stu-id="e7229-133">Type</span></span>        | <span data-ttu-id="e7229-134">说明</span><span class="sxs-lookup"><span data-stu-id="e7229-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7229-135">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e7229-135">accessPackageResource</span></span>|[<span data-ttu-id="e7229-136">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e7229-136">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="e7229-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e7229-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7229-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7229-139">JSON representation</span></span>

<span data-ttu-id="e7229-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7229-140">The following is a JSON representation of the resource.</span></span>

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
