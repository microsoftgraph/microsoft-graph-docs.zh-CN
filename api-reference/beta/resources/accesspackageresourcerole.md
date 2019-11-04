---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b5ae5d321ac5fec86801ca11f60ead8a276fd73
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938917"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="fb88f-103">accessPackageResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb88f-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb88f-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色是对在资源中定义的角色的引用，可在 access 程序包中使用。</span><span class="sxs-lookup"><span data-stu-id="fb88f-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="fb88f-105">属性</span><span class="sxs-lookup"><span data-stu-id="fb88f-105">Properties</span></span>

| <span data-ttu-id="fb88f-106">属性</span><span class="sxs-lookup"><span data-stu-id="fb88f-106">Property</span></span>     | <span data-ttu-id="fb88f-107">类型</span><span class="sxs-lookup"><span data-stu-id="fb88f-107">Type</span></span>        | <span data-ttu-id="fb88f-108">说明</span><span class="sxs-lookup"><span data-stu-id="fb88f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb88f-109">说明</span><span class="sxs-lookup"><span data-stu-id="fb88f-109">description</span></span>|<span data-ttu-id="fb88f-110">String</span><span class="sxs-lookup"><span data-stu-id="fb88f-110">String</span></span>|<span data-ttu-id="fb88f-111">资源角色的说明。</span><span class="sxs-lookup"><span data-stu-id="fb88f-111">A description for the resource role.</span></span>|
|<span data-ttu-id="fb88f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fb88f-112">displayName</span></span>|<span data-ttu-id="fb88f-113">String</span><span class="sxs-lookup"><span data-stu-id="fb88f-113">String</span></span>|<span data-ttu-id="fb88f-114">资源角色的显示名称，例如应用程序定义的角色。</span><span class="sxs-lookup"><span data-stu-id="fb88f-114">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="fb88f-115">id</span><span class="sxs-lookup"><span data-stu-id="fb88f-115">id</span></span>|<span data-ttu-id="fb88f-116">字符串</span><span class="sxs-lookup"><span data-stu-id="fb88f-116">String</span></span>| <span data-ttu-id="fb88f-117">只读。</span><span class="sxs-lookup"><span data-stu-id="fb88f-117">Read-only.</span></span>|
|<span data-ttu-id="fb88f-118">originId</span><span class="sxs-lookup"><span data-stu-id="fb88f-118">originId</span></span>|<span data-ttu-id="fb88f-119">字符串</span><span class="sxs-lookup"><span data-stu-id="fb88f-119">String</span></span>|<span data-ttu-id="fb88f-120">源系统中资源角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fb88f-120">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="fb88f-121">originSystem</span><span class="sxs-lookup"><span data-stu-id="fb88f-121">originSystem</span></span>|<span data-ttu-id="fb88f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="fb88f-122">String</span></span>|<span data-ttu-id="fb88f-123">源系统中资源的类型。</span><span class="sxs-lookup"><span data-stu-id="fb88f-123">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb88f-124">关系</span><span class="sxs-lookup"><span data-stu-id="fb88f-124">Relationships</span></span>

| <span data-ttu-id="fb88f-125">关系</span><span class="sxs-lookup"><span data-stu-id="fb88f-125">Relationship</span></span> | <span data-ttu-id="fb88f-126">类型</span><span class="sxs-lookup"><span data-stu-id="fb88f-126">Type</span></span>        | <span data-ttu-id="fb88f-127">描述</span><span class="sxs-lookup"><span data-stu-id="fb88f-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb88f-128">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="fb88f-128">accessPackageResource</span></span>|[<span data-ttu-id="fb88f-129">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="fb88f-129">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="fb88f-p101">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="fb88f-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb88f-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb88f-132">JSON representation</span></span>

<span data-ttu-id="fb88f-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb88f-133">The following is a JSON representation of the resource.</span></span>

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
