---
title: iPv6CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv6 范围。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7201a95013551aa9629032bffc808f93156f66a0
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653844"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="e0795-103">iPv6CidrRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0795-103">iPv6CidrRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0795-104">表示使用 CIDR 表示法的 IPv6 范围。</span><span class="sxs-lookup"><span data-stu-id="e0795-104">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="e0795-105">继承自 [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e0795-105">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0795-106">属性</span><span class="sxs-lookup"><span data-stu-id="e0795-106">Properties</span></span>

| <span data-ttu-id="e0795-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0795-107">Property</span></span>     | <span data-ttu-id="e0795-108">类型</span><span class="sxs-lookup"><span data-stu-id="e0795-108">Type</span></span>        | <span data-ttu-id="e0795-109">说明</span><span class="sxs-lookup"><span data-stu-id="e0795-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0795-110">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="e0795-110">cidrAddress</span></span>|<span data-ttu-id="e0795-111">String</span><span class="sxs-lookup"><span data-stu-id="e0795-111">String</span></span>|<span data-ttu-id="e0795-112">CIDR 表示法中的 IPv6 地址</span><span class="sxs-lookup"><span data-stu-id="e0795-112">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0795-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0795-113">JSON representation</span></span>

<span data-ttu-id="e0795-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0795-114">The following is a JSON representation of the resource.</span></span>

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