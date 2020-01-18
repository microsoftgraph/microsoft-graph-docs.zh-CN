---
title: policyBase 资源类型
description: 表示要从其继承的策略类型的抽象基类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 757f6771065d60818611662da4dfdcc37ff65853
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234208"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="4ecb3-103">policyBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ecb3-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecb3-104">表示要从其继承的策略类型的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-104">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="4ecb3-105">方法</span><span class="sxs-lookup"><span data-stu-id="4ecb3-105">Methods</span></span>

<span data-ttu-id="4ecb3-106">无</span><span class="sxs-lookup"><span data-stu-id="4ecb3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="4ecb3-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ecb3-107">Properties</span></span>

| <span data-ttu-id="4ecb3-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ecb3-108">Property</span></span>     | <span data-ttu-id="4ecb3-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ecb3-109">Type</span></span>        | <span data-ttu-id="4ecb3-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ecb3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ecb3-111">id</span><span class="sxs-lookup"><span data-stu-id="4ecb3-111">id</span></span>|<span data-ttu-id="4ecb3-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4ecb3-112">String</span></span>| <span data-ttu-id="4ecb3-113">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-113">Unique identifier for this policy.</span></span> <span data-ttu-id="4ecb3-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-114">Read-only.</span></span>|
|<span data-ttu-id="4ecb3-115">说明</span><span class="sxs-lookup"><span data-stu-id="4ecb3-115">description</span></span>|<span data-ttu-id="4ecb3-116">String</span><span class="sxs-lookup"><span data-stu-id="4ecb3-116">String</span></span>| <span data-ttu-id="4ecb3-117">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-117">Description for this policy.</span></span>|
|<span data-ttu-id="4ecb3-118">displayName</span><span class="sxs-lookup"><span data-stu-id="4ecb3-118">displayName</span></span>|<span data-ttu-id="4ecb3-119">String</span><span class="sxs-lookup"><span data-stu-id="4ecb3-119">String</span></span>| <span data-ttu-id="4ecb3-120">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-120">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4ecb3-121">关系</span><span class="sxs-lookup"><span data-stu-id="4ecb3-121">Relationships</span></span>

<span data-ttu-id="4ecb3-122">无</span><span class="sxs-lookup"><span data-stu-id="4ecb3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ecb3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ecb3-123">JSON representation</span></span>

<span data-ttu-id="4ecb3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ecb3-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->