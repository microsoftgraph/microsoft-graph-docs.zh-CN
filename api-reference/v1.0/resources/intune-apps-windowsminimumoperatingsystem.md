---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffc5d67597f1790ffe5725f8a48b358d7679817a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356035"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="3a10a-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a10a-103">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="3a10a-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a10a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a10a-105">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="3a10a-105">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="3a10a-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a10a-106">Properties</span></span>
|<span data-ttu-id="3a10a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a10a-107">Property</span></span>|<span data-ttu-id="3a10a-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a10a-108">Type</span></span>|<span data-ttu-id="3a10a-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a10a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a10a-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="3a10a-110">v8_0</span></span>|<span data-ttu-id="3a10a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a10a-111">Boolean</span></span>|<span data-ttu-id="3a10a-112">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="3a10a-112">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="3a10a-113">v8_1</span><span class="sxs-lookup"><span data-stu-id="3a10a-113">v8_1</span></span>|<span data-ttu-id="3a10a-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="3a10a-114">Boolean</span></span>|<span data-ttu-id="3a10a-115">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="3a10a-115">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="3a10a-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="3a10a-116">v10_0</span></span>|<span data-ttu-id="3a10a-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="3a10a-117">Boolean</span></span>|<span data-ttu-id="3a10a-118">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="3a10a-118">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a10a-119">关系</span><span class="sxs-lookup"><span data-stu-id="3a10a-119">Relationships</span></span>
<span data-ttu-id="3a10a-120">无</span><span class="sxs-lookup"><span data-stu-id="3a10a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a10a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a10a-121">JSON Representation</span></span>
<span data-ttu-id="3a10a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a10a-122">Here is a JSON representation of the resource.</span></span>
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




