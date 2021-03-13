---
title: iPv4CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv4 范围。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6251c06678c811a4553cdc28a76422d75d494284
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760712"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="ea781-103">iPv4CidrRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea781-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="ea781-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea781-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea781-105">表示使用 CIDR 表示法的 IPv4 范围。</span><span class="sxs-lookup"><span data-stu-id="ea781-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="ea781-106">继承自 [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ea781-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea781-107">属性</span><span class="sxs-lookup"><span data-stu-id="ea781-107">Properties</span></span>

| <span data-ttu-id="ea781-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea781-108">Property</span></span>     | <span data-ttu-id="ea781-109">类型</span><span class="sxs-lookup"><span data-stu-id="ea781-109">Type</span></span>        | <span data-ttu-id="ea781-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea781-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ea781-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="ea781-111">cidrAddress</span></span>|<span data-ttu-id="ea781-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ea781-112">String</span></span>|<span data-ttu-id="ea781-113">CIDR 表示法中的 IPv4 地址</span><span class="sxs-lookup"><span data-stu-id="ea781-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea781-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea781-114">JSON representation</span></span>

<span data-ttu-id="ea781-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea781-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv4CidrRange",
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
  "description": "iPv4CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

