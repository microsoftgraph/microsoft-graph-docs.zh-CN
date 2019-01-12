---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975643"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="bfdd0-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfdd0-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="bfdd0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfdd0-105">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="bfdd0-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfdd0-106">Properties</span></span>
|<span data-ttu-id="bfdd0-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfdd0-107">Property</span></span>|<span data-ttu-id="bfdd0-108">类型</span><span class="sxs-lookup"><span data-stu-id="bfdd0-108">Type</span></span>|<span data-ttu-id="bfdd0-109">说明</span><span class="sxs-lookup"><span data-stu-id="bfdd0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfdd0-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-110">androidCount</span></span>|<span data-ttu-id="bfdd0-111">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-111">Int32</span></span>|<span data-ttu-id="bfdd0-112">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-112">Number of android device count.</span></span>|
|<span data-ttu-id="bfdd0-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-113">iosCount</span></span>|<span data-ttu-id="bfdd0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-114">Int32</span></span>|<span data-ttu-id="bfdd0-115">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="bfdd0-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-116">macOSCount</span></span>|<span data-ttu-id="bfdd0-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-117">Int32</span></span>|<span data-ttu-id="bfdd0-118">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="bfdd0-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-119">windowsMobileCount</span></span>|<span data-ttu-id="bfdd0-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-120">Int32</span></span>|<span data-ttu-id="bfdd0-121">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="bfdd0-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-122">windowsCount</span></span>|<span data-ttu-id="bfdd0-123">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-123">Int32</span></span>|<span data-ttu-id="bfdd0-124">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="bfdd0-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="bfdd0-125">unknownCount</span></span>|<span data-ttu-id="bfdd0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdd0-126">Int32</span></span>|<span data-ttu-id="bfdd0-127">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfdd0-128">关系</span><span class="sxs-lookup"><span data-stu-id="bfdd0-128">Relationships</span></span>
<span data-ttu-id="bfdd0-129">无</span><span class="sxs-lookup"><span data-stu-id="bfdd0-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bfdd0-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfdd0-130">JSON Representation</span></span>
<span data-ttu-id="bfdd0-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfdd0-131">Here is a JSON representation of the resource.</span></span>
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



