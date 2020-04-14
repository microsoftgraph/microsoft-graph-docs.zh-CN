---
title: iPv6CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv6 范围。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46c4742a65ec8826f363187eaaba05a1bfb8f893
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384960"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="9b16d-103">iPv6CidrRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b16d-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="9b16d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b16d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b16d-105">表示使用 CIDR 表示法的 IPv6 范围。</span><span class="sxs-lookup"><span data-stu-id="9b16d-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="9b16d-106">继承自 [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="9b16d-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b16d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b16d-107">Properties</span></span>

| <span data-ttu-id="9b16d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b16d-108">Property</span></span>     | <span data-ttu-id="9b16d-109">类型</span><span class="sxs-lookup"><span data-stu-id="9b16d-109">Type</span></span>        | <span data-ttu-id="9b16d-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b16d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b16d-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="9b16d-111">cidrAddress</span></span>|<span data-ttu-id="9b16d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9b16d-112">String</span></span>|<span data-ttu-id="9b16d-113">CIDR 表示法中的 IPv6 地址</span><span class="sxs-lookup"><span data-stu-id="9b16d-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b16d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b16d-114">JSON representation</span></span>

<span data-ttu-id="9b16d-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b16d-115">The following is a JSON representation of the resource.</span></span>

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