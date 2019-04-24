---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13bfc5d8d4e85f31b178801becd56e744a40c106
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521353"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="e9d21-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9d21-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="e9d21-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9d21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9d21-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9d21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9d21-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="e9d21-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="e9d21-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9d21-107">Properties</span></span>
|<span data-ttu-id="e9d21-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9d21-108">Property</span></span>|<span data-ttu-id="e9d21-109">类型</span><span class="sxs-lookup"><span data-stu-id="e9d21-109">Type</span></span>|<span data-ttu-id="e9d21-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9d21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9d21-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-111">androidCount</span></span>|<span data-ttu-id="e9d21-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-112">Int32</span></span>|<span data-ttu-id="e9d21-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-113">Number of android device count.</span></span>|
|<span data-ttu-id="e9d21-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-114">iosCount</span></span>|<span data-ttu-id="e9d21-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-115">Int32</span></span>|<span data-ttu-id="e9d21-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="e9d21-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-117">macOSCount</span></span>|<span data-ttu-id="e9d21-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-118">Int32</span></span>|<span data-ttu-id="e9d21-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="e9d21-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-120">windowsMobileCount</span></span>|<span data-ttu-id="e9d21-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-121">Int32</span></span>|<span data-ttu-id="e9d21-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="e9d21-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-123">windowsCount</span></span>|<span data-ttu-id="e9d21-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-124">Int32</span></span>|<span data-ttu-id="e9d21-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="e9d21-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e9d21-126">unknownCount</span></span>|<span data-ttu-id="e9d21-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d21-127">Int32</span></span>|<span data-ttu-id="e9d21-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="e9d21-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9d21-129">关系</span><span class="sxs-lookup"><span data-stu-id="e9d21-129">Relationships</span></span>
<span data-ttu-id="e9d21-130">无</span><span class="sxs-lookup"><span data-stu-id="e9d21-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9d21-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9d21-131">JSON Representation</span></span>
<span data-ttu-id="e9d21-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9d21-132">Here is a JSON representation of the resource.</span></span>
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





