---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7fe455bc0e934e08b858a084009ac5c8364a673
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950961"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="0ba7e-103">operatingSystemVersionRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ba7e-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="0ba7e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ba7e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ba7e-106">操作系统版本范围。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="0ba7e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ba7e-107">Properties</span></span>
|<span data-ttu-id="0ba7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ba7e-108">Property</span></span>|<span data-ttu-id="0ba7e-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ba7e-109">Type</span></span>|<span data-ttu-id="0ba7e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ba7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ba7e-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ba7e-111">description</span></span>|<span data-ttu-id="0ba7e-112">String</span><span class="sxs-lookup"><span data-stu-id="0ba7e-112">String</span></span>|<span data-ttu-id="0ba7e-113">此范围的说明 (例如, 有效的1702版本)</span><span class="sxs-lookup"><span data-stu-id="0ba7e-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="0ba7e-114">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="0ba7e-114">lowestVersion</span></span>|<span data-ttu-id="0ba7e-115">String</span><span class="sxs-lookup"><span data-stu-id="0ba7e-115">String</span></span>|<span data-ttu-id="0ba7e-116">此范围包含的最低包含版本。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="0ba7e-117">highestVersion</span><span class="sxs-lookup"><span data-stu-id="0ba7e-117">highestVersion</span></span>|<span data-ttu-id="0ba7e-118">String</span><span class="sxs-lookup"><span data-stu-id="0ba7e-118">String</span></span>|<span data-ttu-id="0ba7e-119">此范围包含的最高包含版本。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ba7e-120">关系</span><span class="sxs-lookup"><span data-stu-id="0ba7e-120">Relationships</span></span>
<span data-ttu-id="0ba7e-121">无</span><span class="sxs-lookup"><span data-stu-id="0ba7e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ba7e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ba7e-122">JSON Representation</span></span>
<span data-ttu-id="0ba7e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ba7e-123">Here is a JSON representation of the resource.</span></span>
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




