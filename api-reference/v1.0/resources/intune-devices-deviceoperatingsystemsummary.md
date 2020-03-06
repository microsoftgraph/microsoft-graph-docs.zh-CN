---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82eb7fe0feb0f410a0ef80ab6756aa499f73b71d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533264"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="53317-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="53317-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="53317-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53317-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53317-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53317-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="53317-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="53317-107">属性</span><span class="sxs-lookup"><span data-stu-id="53317-107">Properties</span></span>
|<span data-ttu-id="53317-108">属性</span><span class="sxs-lookup"><span data-stu-id="53317-108">Property</span></span>|<span data-ttu-id="53317-109">类型</span><span class="sxs-lookup"><span data-stu-id="53317-109">Type</span></span>|<span data-ttu-id="53317-110">说明</span><span class="sxs-lookup"><span data-stu-id="53317-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53317-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="53317-111">androidCount</span></span>|<span data-ttu-id="53317-112">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-112">Int32</span></span>|<span data-ttu-id="53317-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-113">Number of android device count.</span></span>|
|<span data-ttu-id="53317-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="53317-114">iosCount</span></span>|<span data-ttu-id="53317-115">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-115">Int32</span></span>|<span data-ttu-id="53317-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="53317-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="53317-117">macOSCount</span></span>|<span data-ttu-id="53317-118">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-118">Int32</span></span>|<span data-ttu-id="53317-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="53317-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="53317-120">windowsMobileCount</span></span>|<span data-ttu-id="53317-121">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-121">Int32</span></span>|<span data-ttu-id="53317-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="53317-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="53317-123">windowsCount</span></span>|<span data-ttu-id="53317-124">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-124">Int32</span></span>|<span data-ttu-id="53317-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="53317-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="53317-126">unknownCount</span></span>|<span data-ttu-id="53317-127">Int32</span><span class="sxs-lookup"><span data-stu-id="53317-127">Int32</span></span>|<span data-ttu-id="53317-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="53317-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53317-129">关系</span><span class="sxs-lookup"><span data-stu-id="53317-129">Relationships</span></span>
<span data-ttu-id="53317-130">无</span><span class="sxs-lookup"><span data-stu-id="53317-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53317-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53317-131">JSON Representation</span></span>
<span data-ttu-id="53317-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53317-132">Here is a JSON representation of the resource.</span></span>
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




