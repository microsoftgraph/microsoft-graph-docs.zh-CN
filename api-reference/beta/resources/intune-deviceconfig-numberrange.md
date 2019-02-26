---
title: numberRange 资源类型
description: 号码范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166785"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="e8168-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8168-103">numberRange resource type</span></span>

> <span data-ttu-id="e8168-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8168-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8168-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8168-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8168-106">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="e8168-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e8168-107">属性</span><span class="sxs-lookup"><span data-stu-id="e8168-107">Properties</span></span>
|<span data-ttu-id="e8168-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8168-108">Property</span></span>|<span data-ttu-id="e8168-109">类型</span><span class="sxs-lookup"><span data-stu-id="e8168-109">Type</span></span>|<span data-ttu-id="e8168-110">说明</span><span class="sxs-lookup"><span data-stu-id="e8168-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8168-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="e8168-111">lowerNumber</span></span>|<span data-ttu-id="e8168-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e8168-112">Int32</span></span>|<span data-ttu-id="e8168-113">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="e8168-113">Lower number.</span></span>|
|<span data-ttu-id="e8168-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="e8168-114">upperNumber</span></span>|<span data-ttu-id="e8168-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e8168-115">Int32</span></span>|<span data-ttu-id="e8168-116">上限数。</span><span class="sxs-lookup"><span data-stu-id="e8168-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8168-117">关系</span><span class="sxs-lookup"><span data-stu-id="e8168-117">Relationships</span></span>
<span data-ttu-id="e8168-118">无</span><span class="sxs-lookup"><span data-stu-id="e8168-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8168-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8168-119">JSON Representation</span></span>
<span data-ttu-id="e8168-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8168-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




