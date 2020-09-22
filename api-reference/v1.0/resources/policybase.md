---
title: policyBase 资源类型
description: 表示要从其继承的策略类型的抽象基类型。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e0d1d59698b8a82252c4cbc2ae8edf2ae1e3b62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037330"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="8ccb0-103">policyBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ccb0-103">policyBase resource type</span></span>

<span data-ttu-id="8ccb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ccb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ccb0-105">表示要从其继承的策略类型的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="8ccb0-106">方法</span><span class="sxs-lookup"><span data-stu-id="8ccb0-106">Methods</span></span>

<span data-ttu-id="8ccb0-107">无</span><span class="sxs-lookup"><span data-stu-id="8ccb0-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="8ccb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ccb0-108">Properties</span></span>

| <span data-ttu-id="8ccb0-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ccb0-109">Property</span></span>     | <span data-ttu-id="8ccb0-110">类型</span><span class="sxs-lookup"><span data-stu-id="8ccb0-110">Type</span></span>        | <span data-ttu-id="8ccb0-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ccb0-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ccb0-112">id</span><span class="sxs-lookup"><span data-stu-id="8ccb0-112">id</span></span>|<span data-ttu-id="8ccb0-113">String</span><span class="sxs-lookup"><span data-stu-id="8ccb0-113">String</span></span>| <span data-ttu-id="8ccb0-114">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-114">Unique identifier for this policy.</span></span> <span data-ttu-id="8ccb0-115">只读。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-115">Read-only.</span></span>|
|<span data-ttu-id="8ccb0-116">说明</span><span class="sxs-lookup"><span data-stu-id="8ccb0-116">description</span></span>|<span data-ttu-id="8ccb0-117">String</span><span class="sxs-lookup"><span data-stu-id="8ccb0-117">String</span></span>| <span data-ttu-id="8ccb0-118">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-118">Description for this policy.</span></span>|
|<span data-ttu-id="8ccb0-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8ccb0-119">displayName</span></span>|<span data-ttu-id="8ccb0-120">String</span><span class="sxs-lookup"><span data-stu-id="8ccb0-120">String</span></span>| <span data-ttu-id="8ccb0-121">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ccb0-122">关系</span><span class="sxs-lookup"><span data-stu-id="8ccb0-122">Relationships</span></span>

<span data-ttu-id="8ccb0-123">无</span><span class="sxs-lookup"><span data-stu-id="8ccb0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ccb0-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ccb0-124">JSON representation</span></span>

<span data-ttu-id="8ccb0-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ccb0-125">The following is a JSON representation of the resource.</span></span>

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
