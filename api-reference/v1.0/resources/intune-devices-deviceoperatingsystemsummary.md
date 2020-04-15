---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 460edb4724dcff002e207d7c5df6095cc3a8f130
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453974"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="290b6-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="290b6-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="290b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="290b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="290b6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="290b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="290b6-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="290b6-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="290b6-107">属性</span><span class="sxs-lookup"><span data-stu-id="290b6-107">Properties</span></span>
|<span data-ttu-id="290b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="290b6-108">Property</span></span>|<span data-ttu-id="290b6-109">类型</span><span class="sxs-lookup"><span data-stu-id="290b6-109">Type</span></span>|<span data-ttu-id="290b6-110">说明</span><span class="sxs-lookup"><span data-stu-id="290b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290b6-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="290b6-111">androidCount</span></span>|<span data-ttu-id="290b6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-112">Int32</span></span>|<span data-ttu-id="290b6-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-113">Number of android device count.</span></span>|
|<span data-ttu-id="290b6-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="290b6-114">iosCount</span></span>|<span data-ttu-id="290b6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-115">Int32</span></span>|<span data-ttu-id="290b6-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="290b6-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="290b6-117">macOSCount</span></span>|<span data-ttu-id="290b6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-118">Int32</span></span>|<span data-ttu-id="290b6-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="290b6-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="290b6-120">windowsMobileCount</span></span>|<span data-ttu-id="290b6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-121">Int32</span></span>|<span data-ttu-id="290b6-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="290b6-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="290b6-123">windowsCount</span></span>|<span data-ttu-id="290b6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-124">Int32</span></span>|<span data-ttu-id="290b6-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="290b6-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="290b6-126">unknownCount</span></span>|<span data-ttu-id="290b6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="290b6-127">Int32</span></span>|<span data-ttu-id="290b6-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="290b6-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="290b6-129">关系</span><span class="sxs-lookup"><span data-stu-id="290b6-129">Relationships</span></span>
<span data-ttu-id="290b6-130">无</span><span class="sxs-lookup"><span data-stu-id="290b6-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="290b6-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="290b6-131">JSON Representation</span></span>
<span data-ttu-id="290b6-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="290b6-132">Here is a JSON representation of the resource.</span></span>
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







