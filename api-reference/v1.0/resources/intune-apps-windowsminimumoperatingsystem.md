---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24ac15200fa293cc65a6207a91e5dc1132df1759
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531071"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="e5df6-103">windowsMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5df6-103">windowsMinimumOperatingSystem resource type</span></span>

<span data-ttu-id="e5df6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5df6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5df6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5df6-106">Windows 移动应用需要的最低操作系统。</span><span class="sxs-lookup"><span data-stu-id="e5df6-106">The minimum operating system required for a Windows mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="e5df6-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5df6-107">Properties</span></span>
|<span data-ttu-id="e5df6-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5df6-108">Property</span></span>|<span data-ttu-id="e5df6-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5df6-109">Type</span></span>|<span data-ttu-id="e5df6-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5df6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5df6-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="e5df6-111">v8_0</span></span>|<span data-ttu-id="e5df6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5df6-112">Boolean</span></span>|<span data-ttu-id="e5df6-113">Windows 版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="e5df6-113">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="e5df6-114">v8_1</span><span class="sxs-lookup"><span data-stu-id="e5df6-114">v8_1</span></span>|<span data-ttu-id="e5df6-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e5df6-115">Boolean</span></span>|<span data-ttu-id="e5df6-116">Windows 版本 8.1 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="e5df6-116">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="e5df6-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="e5df6-117">v10_0</span></span>|<span data-ttu-id="e5df6-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="e5df6-118">Boolean</span></span>|<span data-ttu-id="e5df6-119">Windows 版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="e5df6-119">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5df6-120">关系</span><span class="sxs-lookup"><span data-stu-id="e5df6-120">Relationships</span></span>
<span data-ttu-id="e5df6-121">无</span><span class="sxs-lookup"><span data-stu-id="e5df6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5df6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5df6-122">JSON Representation</span></span>
<span data-ttu-id="e5df6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5df6-123">Here is a JSON representation of the resource.</span></span>
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




