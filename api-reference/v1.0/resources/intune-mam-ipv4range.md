---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 545de5eb3a2d2bb53fe40f1c23c03014c2391562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533197"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="1c82e-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c82e-103">iPv4Range resource type</span></span>

<span data-ttu-id="1c82e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c82e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c82e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c82e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c82e-106">IPv4 范围定义。</span><span class="sxs-lookup"><span data-stu-id="1c82e-106">IPv4 Range definition.</span></span>


<span data-ttu-id="1c82e-107">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1c82e-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c82e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c82e-108">Properties</span></span>
|<span data-ttu-id="1c82e-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c82e-109">Property</span></span>|<span data-ttu-id="1c82e-110">类型</span><span class="sxs-lookup"><span data-stu-id="1c82e-110">Type</span></span>|<span data-ttu-id="1c82e-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c82e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c82e-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="1c82e-112">lowerAddress</span></span>|<span data-ttu-id="1c82e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1c82e-113">String</span></span>|<span data-ttu-id="1c82e-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="1c82e-114">Lower address.</span></span>|
|<span data-ttu-id="1c82e-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="1c82e-115">upperAddress</span></span>|<span data-ttu-id="1c82e-116">String</span><span class="sxs-lookup"><span data-stu-id="1c82e-116">String</span></span>|<span data-ttu-id="1c82e-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="1c82e-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c82e-118">关系</span><span class="sxs-lookup"><span data-stu-id="1c82e-118">Relationships</span></span>
<span data-ttu-id="1c82e-119">无</span><span class="sxs-lookup"><span data-stu-id="1c82e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c82e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c82e-120">JSON Representation</span></span>
<span data-ttu-id="1c82e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c82e-121">Here is a JSON representation of the resource.</span></span>
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




