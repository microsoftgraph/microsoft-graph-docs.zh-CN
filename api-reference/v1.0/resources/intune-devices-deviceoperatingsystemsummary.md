---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9dfce6c0947fffd861ae1cda205c1011a7500471
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754565"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="d1781-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1781-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="d1781-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1781-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1781-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1781-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1781-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="d1781-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="d1781-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1781-107">Properties</span></span>
|<span data-ttu-id="d1781-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1781-108">Property</span></span>|<span data-ttu-id="d1781-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1781-109">Type</span></span>|<span data-ttu-id="d1781-110">Description</span><span class="sxs-lookup"><span data-stu-id="d1781-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1781-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="d1781-111">androidCount</span></span>|<span data-ttu-id="d1781-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-112">Int32</span></span>|<span data-ttu-id="d1781-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-113">Number of android device count.</span></span>|
|<span data-ttu-id="d1781-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="d1781-114">iosCount</span></span>|<span data-ttu-id="d1781-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-115">Int32</span></span>|<span data-ttu-id="d1781-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="d1781-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="d1781-117">macOSCount</span></span>|<span data-ttu-id="d1781-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-118">Int32</span></span>|<span data-ttu-id="d1781-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="d1781-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="d1781-120">windowsMobileCount</span></span>|<span data-ttu-id="d1781-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-121">Int32</span></span>|<span data-ttu-id="d1781-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="d1781-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="d1781-123">windowsCount</span></span>|<span data-ttu-id="d1781-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-124">Int32</span></span>|<span data-ttu-id="d1781-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="d1781-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d1781-126">unknownCount</span></span>|<span data-ttu-id="d1781-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d1781-127">Int32</span></span>|<span data-ttu-id="d1781-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="d1781-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1781-129">关系</span><span class="sxs-lookup"><span data-stu-id="d1781-129">Relationships</span></span>
<span data-ttu-id="d1781-130">无</span><span class="sxs-lookup"><span data-stu-id="d1781-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1781-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1781-131">JSON Representation</span></span>
<span data-ttu-id="d1781-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1781-132">Here is a JSON representation of the resource.</span></span>
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




