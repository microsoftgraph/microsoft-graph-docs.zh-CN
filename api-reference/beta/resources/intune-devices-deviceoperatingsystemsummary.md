---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b55459189f86e298aa219e0f00d33df8e0625e68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995250"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="b7835-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7835-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="b7835-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7835-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7835-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="b7835-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="b7835-107">属性</span><span class="sxs-lookup"><span data-stu-id="b7835-107">Properties</span></span>
|<span data-ttu-id="b7835-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7835-108">Property</span></span>|<span data-ttu-id="b7835-109">类型</span><span class="sxs-lookup"><span data-stu-id="b7835-109">Type</span></span>|<span data-ttu-id="b7835-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7835-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7835-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="b7835-111">androidCount</span></span>|<span data-ttu-id="b7835-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-112">Int32</span></span>|<span data-ttu-id="b7835-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-113">Number of android device count.</span></span>|
|<span data-ttu-id="b7835-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="b7835-114">iosCount</span></span>|<span data-ttu-id="b7835-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-115">Int32</span></span>|<span data-ttu-id="b7835-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="b7835-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="b7835-117">macOSCount</span></span>|<span data-ttu-id="b7835-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-118">Int32</span></span>|<span data-ttu-id="b7835-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="b7835-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="b7835-120">windowsMobileCount</span></span>|<span data-ttu-id="b7835-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-121">Int32</span></span>|<span data-ttu-id="b7835-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="b7835-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="b7835-123">windowsCount</span></span>|<span data-ttu-id="b7835-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-124">Int32</span></span>|<span data-ttu-id="b7835-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="b7835-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="b7835-126">unknownCount</span></span>|<span data-ttu-id="b7835-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b7835-127">Int32</span></span>|<span data-ttu-id="b7835-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="b7835-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7835-129">关系</span><span class="sxs-lookup"><span data-stu-id="b7835-129">Relationships</span></span>
<span data-ttu-id="b7835-130">无</span><span class="sxs-lookup"><span data-stu-id="b7835-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7835-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7835-131">JSON Representation</span></span>
<span data-ttu-id="b7835-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7835-132">Here is a JSON representation of the resource.</span></span>
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





