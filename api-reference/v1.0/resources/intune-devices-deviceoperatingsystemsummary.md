---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4b53d7c7260e58458995093bbea17df5464e704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846072"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="10d03-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="10d03-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="10d03-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10d03-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10d03-105">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="10d03-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="10d03-106">属性</span><span class="sxs-lookup"><span data-stu-id="10d03-106">Properties</span></span>
|<span data-ttu-id="10d03-107">属性</span><span class="sxs-lookup"><span data-stu-id="10d03-107">Property</span></span>|<span data-ttu-id="10d03-108">类型</span><span class="sxs-lookup"><span data-stu-id="10d03-108">Type</span></span>|<span data-ttu-id="10d03-109">说明</span><span class="sxs-lookup"><span data-stu-id="10d03-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10d03-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="10d03-110">androidCount</span></span>|<span data-ttu-id="10d03-111">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-111">Int32</span></span>|<span data-ttu-id="10d03-112">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-112">Number of android device count.</span></span>|
|<span data-ttu-id="10d03-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="10d03-113">iosCount</span></span>|<span data-ttu-id="10d03-114">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-114">Int32</span></span>|<span data-ttu-id="10d03-115">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="10d03-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="10d03-116">macOSCount</span></span>|<span data-ttu-id="10d03-117">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-117">Int32</span></span>|<span data-ttu-id="10d03-118">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="10d03-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="10d03-119">windowsMobileCount</span></span>|<span data-ttu-id="10d03-120">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-120">Int32</span></span>|<span data-ttu-id="10d03-121">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="10d03-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="10d03-122">windowsCount</span></span>|<span data-ttu-id="10d03-123">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-123">Int32</span></span>|<span data-ttu-id="10d03-124">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="10d03-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="10d03-125">unknownCount</span></span>|<span data-ttu-id="10d03-126">Int32</span><span class="sxs-lookup"><span data-stu-id="10d03-126">Int32</span></span>|<span data-ttu-id="10d03-127">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="10d03-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10d03-128">关系</span><span class="sxs-lookup"><span data-stu-id="10d03-128">Relationships</span></span>
<span data-ttu-id="10d03-129">无</span><span class="sxs-lookup"><span data-stu-id="10d03-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10d03-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10d03-130">JSON Representation</span></span>
<span data-ttu-id="10d03-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10d03-131">Here is a JSON representation of the resource.</span></span>
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



