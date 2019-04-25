---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51815dffc0048ec88b81cbe6034a42e108e5b222
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550579"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="c92d3-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="c92d3-103">iPv6Range resource type</span></span>

> <span data-ttu-id="c92d3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c92d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c92d3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c92d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c92d3-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="c92d3-106">IPv6 Range definition.</span></span>


<span data-ttu-id="c92d3-107">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c92d3-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c92d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="c92d3-108">Properties</span></span>
|<span data-ttu-id="c92d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="c92d3-109">Property</span></span>|<span data-ttu-id="c92d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="c92d3-110">Type</span></span>|<span data-ttu-id="c92d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c92d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c92d3-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c92d3-112">lowerAddress</span></span>|<span data-ttu-id="c92d3-113">String</span><span class="sxs-lookup"><span data-stu-id="c92d3-113">String</span></span>|<span data-ttu-id="c92d3-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="c92d3-114">Lower address.</span></span>|
|<span data-ttu-id="c92d3-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c92d3-115">upperAddress</span></span>|<span data-ttu-id="c92d3-116">String</span><span class="sxs-lookup"><span data-stu-id="c92d3-116">String</span></span>|<span data-ttu-id="c92d3-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="c92d3-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c92d3-118">关系</span><span class="sxs-lookup"><span data-stu-id="c92d3-118">Relationships</span></span>
<span data-ttu-id="c92d3-119">无</span><span class="sxs-lookup"><span data-stu-id="c92d3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c92d3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c92d3-120">JSON Representation</span></span>
<span data-ttu-id="c92d3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c92d3-121">Here is a JSON representation of the resource.</span></span>
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





