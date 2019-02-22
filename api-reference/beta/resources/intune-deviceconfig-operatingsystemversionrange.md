---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521f7d0b0ec4ddab728ed3b95c27acf21695b0d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148606"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="033de-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="033de-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="033de-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="033de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="033de-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="033de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="033de-106">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="033de-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="033de-107">属性</span><span class="sxs-lookup"><span data-stu-id="033de-107">Properties</span></span>
|<span data-ttu-id="033de-108">属性</span><span class="sxs-lookup"><span data-stu-id="033de-108">Property</span></span>|<span data-ttu-id="033de-109">类型</span><span class="sxs-lookup"><span data-stu-id="033de-109">Type</span></span>|<span data-ttu-id="033de-110">说明</span><span class="sxs-lookup"><span data-stu-id="033de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="033de-111">说明</span><span class="sxs-lookup"><span data-stu-id="033de-111">description</span></span>|<span data-ttu-id="033de-112">字符串</span><span class="sxs-lookup"><span data-stu-id="033de-112">String</span></span>|<span data-ttu-id="033de-113">此范围的说明 (例如, 有效的1702版本)</span><span class="sxs-lookup"><span data-stu-id="033de-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="033de-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="033de-114">lowestVersion</span></span>|<span data-ttu-id="033de-115">字符串</span><span class="sxs-lookup"><span data-stu-id="033de-115">String</span></span>|<span data-ttu-id="033de-116">此范围包含的最低包含版本。</span><span class="sxs-lookup"><span data-stu-id="033de-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="033de-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="033de-117">highestVersion</span></span>|<span data-ttu-id="033de-118">字符串</span><span class="sxs-lookup"><span data-stu-id="033de-118">String</span></span>|<span data-ttu-id="033de-119">此范围包含的最高包含版本。</span><span class="sxs-lookup"><span data-stu-id="033de-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="033de-120">关系</span><span class="sxs-lookup"><span data-stu-id="033de-120">Relationships</span></span>
<span data-ttu-id="033de-121">无</span><span class="sxs-lookup"><span data-stu-id="033de-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="033de-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="033de-122">JSON Representation</span></span>
<span data-ttu-id="033de-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="033de-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




