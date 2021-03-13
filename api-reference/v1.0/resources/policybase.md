---
title: policyBase 资源类型
description: 表示要继承的策略类型的抽象基本类型。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a091fb23be66f476b03b725e29dced32b138c9bc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761512"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="1f3e5-103">policyBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f3e5-103">policyBase resource type</span></span>

<span data-ttu-id="1f3e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f3e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f3e5-105">表示要继承的策略类型的抽象基本类型。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="1f3e5-106">方法</span><span class="sxs-lookup"><span data-stu-id="1f3e5-106">Methods</span></span>

<span data-ttu-id="1f3e5-107">无</span><span class="sxs-lookup"><span data-stu-id="1f3e5-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="1f3e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f3e5-108">Properties</span></span>

| <span data-ttu-id="1f3e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f3e5-109">Property</span></span>     | <span data-ttu-id="1f3e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="1f3e5-110">Type</span></span>        | <span data-ttu-id="1f3e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f3e5-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f3e5-112">id</span><span class="sxs-lookup"><span data-stu-id="1f3e5-112">id</span></span>|<span data-ttu-id="1f3e5-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1f3e5-113">String</span></span>| <span data-ttu-id="1f3e5-114">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-114">Unique identifier for this policy.</span></span> <span data-ttu-id="1f3e5-115">只读。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-115">Read-only.</span></span>|
|<span data-ttu-id="1f3e5-116">说明</span><span class="sxs-lookup"><span data-stu-id="1f3e5-116">description</span></span>|<span data-ttu-id="1f3e5-117">字符串</span><span class="sxs-lookup"><span data-stu-id="1f3e5-117">String</span></span>| <span data-ttu-id="1f3e5-118">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-118">Description for this policy.</span></span>|
|<span data-ttu-id="1f3e5-119">displayName</span><span class="sxs-lookup"><span data-stu-id="1f3e5-119">displayName</span></span>|<span data-ttu-id="1f3e5-120">字符串</span><span class="sxs-lookup"><span data-stu-id="1f3e5-120">String</span></span>| <span data-ttu-id="1f3e5-121">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f3e5-122">关系</span><span class="sxs-lookup"><span data-stu-id="1f3e5-122">Relationships</span></span>

<span data-ttu-id="1f3e5-123">无</span><span class="sxs-lookup"><span data-stu-id="1f3e5-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f3e5-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f3e5-124">JSON representation</span></span>

<span data-ttu-id="1f3e5-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f3e5-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
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
