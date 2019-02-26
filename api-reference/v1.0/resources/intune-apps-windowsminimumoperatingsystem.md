---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f337a61f3a0cfd52e042e65bb3d8de57dcf9f283
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254462"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="04df6-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="04df6-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="04df6-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04df6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04df6-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="04df6-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="04df6-106">属性</span><span class="sxs-lookup"><span data-stu-id="04df6-106">Properties</span></span>
|<span data-ttu-id="04df6-107">属性</span><span class="sxs-lookup"><span data-stu-id="04df6-107">Property</span></span>|<span data-ttu-id="04df6-108">类型</span><span class="sxs-lookup"><span data-stu-id="04df6-108">Type</span></span>|<span data-ttu-id="04df6-109">说明</span><span class="sxs-lookup"><span data-stu-id="04df6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04df6-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="04df6-110">v8_0</span></span>|<span data-ttu-id="04df6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="04df6-111">Boolean</span></span>|<span data-ttu-id="04df6-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="04df6-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="04df6-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="04df6-113">v8_1</span></span>|<span data-ttu-id="04df6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="04df6-114">Boolean</span></span>|<span data-ttu-id="04df6-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="04df6-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="04df6-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="04df6-116">v10_0</span></span>|<span data-ttu-id="04df6-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="04df6-117">Boolean</span></span>|<span data-ttu-id="04df6-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="04df6-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04df6-119">关系</span><span class="sxs-lookup"><span data-stu-id="04df6-119">Relationships</span></span>
<span data-ttu-id="04df6-120">无</span><span class="sxs-lookup"><span data-stu-id="04df6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04df6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04df6-121">JSON Representation</span></span>
<span data-ttu-id="04df6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04df6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



