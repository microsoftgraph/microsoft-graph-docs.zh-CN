---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c747f86592394d6e9efc93bba2775872010b254
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356427"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="24bd4-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="24bd4-103">iPv6Range resource type</span></span>

> <span data-ttu-id="24bd4-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24bd4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24bd4-105">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="24bd4-105">IPv6 Range definition.</span></span>


<span data-ttu-id="24bd4-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="24bd4-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24bd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="24bd4-107">Properties</span></span>
|<span data-ttu-id="24bd4-108">属性</span><span class="sxs-lookup"><span data-stu-id="24bd4-108">Property</span></span>|<span data-ttu-id="24bd4-109">类型</span><span class="sxs-lookup"><span data-stu-id="24bd4-109">Type</span></span>|<span data-ttu-id="24bd4-110">说明</span><span class="sxs-lookup"><span data-stu-id="24bd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24bd4-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="24bd4-111">lowerAddress</span></span>|<span data-ttu-id="24bd4-112">String</span><span class="sxs-lookup"><span data-stu-id="24bd4-112">String</span></span>|<span data-ttu-id="24bd4-113">低地址</span><span class="sxs-lookup"><span data-stu-id="24bd4-113">Lower address</span></span>|
|<span data-ttu-id="24bd4-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="24bd4-114">upperAddress</span></span>|<span data-ttu-id="24bd4-115">String</span><span class="sxs-lookup"><span data-stu-id="24bd4-115">String</span></span>|<span data-ttu-id="24bd4-116">地址上限</span><span class="sxs-lookup"><span data-stu-id="24bd4-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="24bd4-117">关系</span><span class="sxs-lookup"><span data-stu-id="24bd4-117">Relationships</span></span>
<span data-ttu-id="24bd4-118">无</span><span class="sxs-lookup"><span data-stu-id="24bd4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24bd4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24bd4-119">JSON Representation</span></span>
<span data-ttu-id="24bd4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24bd4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




