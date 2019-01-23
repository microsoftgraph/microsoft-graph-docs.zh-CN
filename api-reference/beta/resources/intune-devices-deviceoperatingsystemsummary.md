---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 009998d495eb033510bbc27437b72f866fd4ed7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410768"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="34ce3-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="34ce3-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="34ce3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="34ce3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34ce3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="34ce3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34ce3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34ce3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ce3-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="34ce3-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="34ce3-108">属性</span><span class="sxs-lookup"><span data-stu-id="34ce3-108">Properties</span></span>
|<span data-ttu-id="34ce3-109">属性</span><span class="sxs-lookup"><span data-stu-id="34ce3-109">Property</span></span>|<span data-ttu-id="34ce3-110">类型</span><span class="sxs-lookup"><span data-stu-id="34ce3-110">Type</span></span>|<span data-ttu-id="34ce3-111">说明</span><span class="sxs-lookup"><span data-stu-id="34ce3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ce3-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-112">androidCount</span></span>|<span data-ttu-id="34ce3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-113">Int32</span></span>|<span data-ttu-id="34ce3-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-114">Number of android device count.</span></span>|
|<span data-ttu-id="34ce3-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-115">iosCount</span></span>|<span data-ttu-id="34ce3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-116">Int32</span></span>|<span data-ttu-id="34ce3-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="34ce3-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-118">macOSCount</span></span>|<span data-ttu-id="34ce3-119">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-119">Int32</span></span>|<span data-ttu-id="34ce3-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="34ce3-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-121">windowsMobileCount</span></span>|<span data-ttu-id="34ce3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-122">Int32</span></span>|<span data-ttu-id="34ce3-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="34ce3-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-124">windowsCount</span></span>|<span data-ttu-id="34ce3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-125">Int32</span></span>|<span data-ttu-id="34ce3-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="34ce3-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="34ce3-127">unknownCount</span></span>|<span data-ttu-id="34ce3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="34ce3-128">Int32</span></span>|<span data-ttu-id="34ce3-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="34ce3-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ce3-130">关系</span><span class="sxs-lookup"><span data-stu-id="34ce3-130">Relationships</span></span>
<span data-ttu-id="34ce3-131">无</span><span class="sxs-lookup"><span data-stu-id="34ce3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34ce3-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34ce3-132">JSON Representation</span></span>
<span data-ttu-id="34ce3-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34ce3-133">Here is a JSON representation of the resource.</span></span>
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




