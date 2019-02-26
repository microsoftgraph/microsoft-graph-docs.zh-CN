---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256838"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="b5c21-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5c21-103">iPv4Range resource type</span></span>

> <span data-ttu-id="b5c21-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5c21-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5c21-105">IPv4 范围定义。</span><span class="sxs-lookup"><span data-stu-id="b5c21-105">IPv4 Range definition.</span></span>


<span data-ttu-id="b5c21-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b5c21-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5c21-107">属性</span><span class="sxs-lookup"><span data-stu-id="b5c21-107">Properties</span></span>
|<span data-ttu-id="b5c21-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5c21-108">Property</span></span>|<span data-ttu-id="b5c21-109">类型</span><span class="sxs-lookup"><span data-stu-id="b5c21-109">Type</span></span>|<span data-ttu-id="b5c21-110">说明</span><span class="sxs-lookup"><span data-stu-id="b5c21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c21-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b5c21-111">lowerAddress</span></span>|<span data-ttu-id="b5c21-112">String</span><span class="sxs-lookup"><span data-stu-id="b5c21-112">String</span></span>|<span data-ttu-id="b5c21-113">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="b5c21-113">Lower address.</span></span>|
|<span data-ttu-id="b5c21-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b5c21-114">upperAddress</span></span>|<span data-ttu-id="b5c21-115">String</span><span class="sxs-lookup"><span data-stu-id="b5c21-115">String</span></span>|<span data-ttu-id="b5c21-116">地址上限。</span><span class="sxs-lookup"><span data-stu-id="b5c21-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5c21-117">关系</span><span class="sxs-lookup"><span data-stu-id="b5c21-117">Relationships</span></span>
<span data-ttu-id="b5c21-118">无</span><span class="sxs-lookup"><span data-stu-id="b5c21-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5c21-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5c21-119">JSON Representation</span></span>
<span data-ttu-id="b5c21-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5c21-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



