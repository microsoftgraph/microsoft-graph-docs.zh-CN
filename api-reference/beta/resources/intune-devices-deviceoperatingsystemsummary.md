---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8e61898cb7dfd8f2f058beaf668763ecda27928
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968398"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="f79eb-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f79eb-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="f79eb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f79eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f79eb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f79eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f79eb-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="f79eb-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="f79eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="f79eb-107">Properties</span></span>
|<span data-ttu-id="f79eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="f79eb-108">Property</span></span>|<span data-ttu-id="f79eb-109">类型</span><span class="sxs-lookup"><span data-stu-id="f79eb-109">Type</span></span>|<span data-ttu-id="f79eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="f79eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f79eb-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-111">androidCount</span></span>|<span data-ttu-id="f79eb-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-112">Int32</span></span>|<span data-ttu-id="f79eb-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-113">Number of android device count.</span></span>|
|<span data-ttu-id="f79eb-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-114">iosCount</span></span>|<span data-ttu-id="f79eb-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-115">Int32</span></span>|<span data-ttu-id="f79eb-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="f79eb-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-117">macOSCount</span></span>|<span data-ttu-id="f79eb-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-118">Int32</span></span>|<span data-ttu-id="f79eb-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="f79eb-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-120">windowsMobileCount</span></span>|<span data-ttu-id="f79eb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-121">Int32</span></span>|<span data-ttu-id="f79eb-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="f79eb-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-123">windowsCount</span></span>|<span data-ttu-id="f79eb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-124">Int32</span></span>|<span data-ttu-id="f79eb-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="f79eb-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f79eb-126">unknownCount</span></span>|<span data-ttu-id="f79eb-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f79eb-127">Int32</span></span>|<span data-ttu-id="f79eb-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="f79eb-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f79eb-129">关系</span><span class="sxs-lookup"><span data-stu-id="f79eb-129">Relationships</span></span>
<span data-ttu-id="f79eb-130">无</span><span class="sxs-lookup"><span data-stu-id="f79eb-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f79eb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f79eb-131">JSON Representation</span></span>
<span data-ttu-id="f79eb-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f79eb-132">Here is a JSON representation of the resource.</span></span>
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





