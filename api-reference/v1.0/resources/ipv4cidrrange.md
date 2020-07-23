---
title: iPv4CidrRange 资源类型
description: 表示使用 CIDR 表示法的 IPv4 范围。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 169be1976c57dc76ff85b5eaff5620b3938479d8
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384618"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="d83e6-103">iPv4CidrRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="d83e6-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="d83e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d83e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d83e6-105">表示使用 CIDR 表示法的 IPv4 范围。</span><span class="sxs-lookup"><span data-stu-id="d83e6-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="d83e6-106">继承自 [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="d83e6-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d83e6-107">属性</span><span class="sxs-lookup"><span data-stu-id="d83e6-107">Properties</span></span>

| <span data-ttu-id="d83e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d83e6-108">Property</span></span>     | <span data-ttu-id="d83e6-109">类型</span><span class="sxs-lookup"><span data-stu-id="d83e6-109">Type</span></span>        | <span data-ttu-id="d83e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="d83e6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d83e6-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="d83e6-111">cidrAddress</span></span>|<span data-ttu-id="d83e6-112">String</span><span class="sxs-lookup"><span data-stu-id="d83e6-112">String</span></span>|<span data-ttu-id="d83e6-113">CIDR 表示法中的 IPv4 地址</span><span class="sxs-lookup"><span data-stu-id="d83e6-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d83e6-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d83e6-114">JSON representation</span></span>

<span data-ttu-id="d83e6-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d83e6-115">The following is a JSON representation of the resource.</span></span>

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