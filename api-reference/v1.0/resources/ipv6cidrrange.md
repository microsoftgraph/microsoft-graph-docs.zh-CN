---
title: iPv6CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv6 范围。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 75c15484a310bdff66052b9381bea8b62779979c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967455"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="eeb74-103">iPv6CidrRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="eeb74-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="eeb74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeb74-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eeb74-105">表示使用 CIDR 表示法的 IPv6 范围。</span><span class="sxs-lookup"><span data-stu-id="eeb74-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="eeb74-106">继承自 [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="eeb74-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eeb74-107">属性</span><span class="sxs-lookup"><span data-stu-id="eeb74-107">Properties</span></span>

| <span data-ttu-id="eeb74-108">属性</span><span class="sxs-lookup"><span data-stu-id="eeb74-108">Property</span></span>     | <span data-ttu-id="eeb74-109">类型</span><span class="sxs-lookup"><span data-stu-id="eeb74-109">Type</span></span>        | <span data-ttu-id="eeb74-110">说明</span><span class="sxs-lookup"><span data-stu-id="eeb74-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eeb74-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="eeb74-111">cidrAddress</span></span>|<span data-ttu-id="eeb74-112">String</span><span class="sxs-lookup"><span data-stu-id="eeb74-112">String</span></span>|<span data-ttu-id="eeb74-113">CIDR 表示法中的 IPv6 地址</span><span class="sxs-lookup"><span data-stu-id="eeb74-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eeb74-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eeb74-114">JSON representation</span></span>

<span data-ttu-id="eeb74-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eeb74-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv6CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv6CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
