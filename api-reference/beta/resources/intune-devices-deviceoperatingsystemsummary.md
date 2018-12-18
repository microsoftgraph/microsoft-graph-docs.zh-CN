---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
ms.openlocfilehash: 8dd3bf85a75d5acf6ae4bb0cecb8fd360c4e0459
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341858"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="3b66e-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b66e-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="3b66e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b66e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b66e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b66e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b66e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3b66e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b66e-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="3b66e-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="3b66e-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b66e-108">Properties</span></span>
|<span data-ttu-id="3b66e-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b66e-109">Property</span></span>|<span data-ttu-id="3b66e-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b66e-110">Type</span></span>|<span data-ttu-id="3b66e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b66e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b66e-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-112">androidCount</span></span>|<span data-ttu-id="3b66e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-113">Int32</span></span>|<span data-ttu-id="3b66e-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-114">Number of android device count.</span></span>|
|<span data-ttu-id="3b66e-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-115">iosCount</span></span>|<span data-ttu-id="3b66e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-116">Int32</span></span>|<span data-ttu-id="3b66e-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="3b66e-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-118">macOSCount</span></span>|<span data-ttu-id="3b66e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-119">Int32</span></span>|<span data-ttu-id="3b66e-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="3b66e-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-121">windowsMobileCount</span></span>|<span data-ttu-id="3b66e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-122">Int32</span></span>|<span data-ttu-id="3b66e-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="3b66e-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-124">windowsCount</span></span>|<span data-ttu-id="3b66e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-125">Int32</span></span>|<span data-ttu-id="3b66e-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="3b66e-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="3b66e-127">unknownCount</span></span>|<span data-ttu-id="3b66e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3b66e-128">Int32</span></span>|<span data-ttu-id="3b66e-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="3b66e-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b66e-130">关系</span><span class="sxs-lookup"><span data-stu-id="3b66e-130">Relationships</span></span>
<span data-ttu-id="3b66e-131">无</span><span class="sxs-lookup"><span data-stu-id="3b66e-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b66e-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b66e-132">JSON Representation</span></span>
<span data-ttu-id="3b66e-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b66e-133">Here is a JSON representation of the resource.</span></span>
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





