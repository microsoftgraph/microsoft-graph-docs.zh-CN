---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62fe2496e505ac0d281381b9d53604aa98094f3c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356934"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="ed6d3-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed6d3-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="ed6d3-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed6d3-105">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="ed6d3-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed6d3-106">Properties</span></span>
|<span data-ttu-id="ed6d3-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed6d3-107">Property</span></span>|<span data-ttu-id="ed6d3-108">类型</span><span class="sxs-lookup"><span data-stu-id="ed6d3-108">Type</span></span>|<span data-ttu-id="ed6d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="ed6d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed6d3-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-110">androidCount</span></span>|<span data-ttu-id="ed6d3-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-111">Int32</span></span>|<span data-ttu-id="ed6d3-112">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-112">Number of android device count.</span></span>|
|<span data-ttu-id="ed6d3-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-113">iosCount</span></span>|<span data-ttu-id="ed6d3-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-114">Int32</span></span>|<span data-ttu-id="ed6d3-115">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="ed6d3-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-116">macOSCount</span></span>|<span data-ttu-id="ed6d3-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-117">Int32</span></span>|<span data-ttu-id="ed6d3-118">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="ed6d3-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-119">windowsMobileCount</span></span>|<span data-ttu-id="ed6d3-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-120">Int32</span></span>|<span data-ttu-id="ed6d3-121">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="ed6d3-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-122">windowsCount</span></span>|<span data-ttu-id="ed6d3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-123">Int32</span></span>|<span data-ttu-id="ed6d3-124">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="ed6d3-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="ed6d3-125">unknownCount</span></span>|<span data-ttu-id="ed6d3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6d3-126">Int32</span></span>|<span data-ttu-id="ed6d3-127">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed6d3-128">关系</span><span class="sxs-lookup"><span data-stu-id="ed6d3-128">Relationships</span></span>
<span data-ttu-id="ed6d3-129">无</span><span class="sxs-lookup"><span data-stu-id="ed6d3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed6d3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed6d3-130">JSON Representation</span></span>
<span data-ttu-id="ed6d3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed6d3-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```




