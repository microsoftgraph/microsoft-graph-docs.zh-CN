---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81b95ebbfe4697b20156300cb7b383935556f17e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347967"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="07dae-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="07dae-103">iPv6Range resource type</span></span>

> <span data-ttu-id="07dae-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07dae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07dae-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07dae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07dae-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="07dae-106">IPv6 Range definition.</span></span>


<span data-ttu-id="07dae-107">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="07dae-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07dae-108">属性</span><span class="sxs-lookup"><span data-stu-id="07dae-108">Properties</span></span>
|<span data-ttu-id="07dae-109">属性</span><span class="sxs-lookup"><span data-stu-id="07dae-109">Property</span></span>|<span data-ttu-id="07dae-110">类型</span><span class="sxs-lookup"><span data-stu-id="07dae-110">Type</span></span>|<span data-ttu-id="07dae-111">说明</span><span class="sxs-lookup"><span data-stu-id="07dae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dae-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="07dae-112">lowerAddress</span></span>|<span data-ttu-id="07dae-113">String</span><span class="sxs-lookup"><span data-stu-id="07dae-113">String</span></span>|<span data-ttu-id="07dae-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="07dae-114">Lower address.</span></span>|
|<span data-ttu-id="07dae-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="07dae-115">upperAddress</span></span>|<span data-ttu-id="07dae-116">String</span><span class="sxs-lookup"><span data-stu-id="07dae-116">String</span></span>|<span data-ttu-id="07dae-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="07dae-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07dae-118">关系</span><span class="sxs-lookup"><span data-stu-id="07dae-118">Relationships</span></span>
<span data-ttu-id="07dae-119">无</span><span class="sxs-lookup"><span data-stu-id="07dae-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07dae-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07dae-120">JSON Representation</span></span>
<span data-ttu-id="07dae-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07dae-121">Here is a JSON representation of the resource.</span></span>
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



