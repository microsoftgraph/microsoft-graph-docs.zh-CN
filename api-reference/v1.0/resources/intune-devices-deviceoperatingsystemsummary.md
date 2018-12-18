---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
ms.openlocfilehash: 73615964d0c2b187c36b57956d534fa08d60684f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346618"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="0b546-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b546-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="0b546-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b546-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b546-105">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="0b546-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="0b546-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b546-106">Properties</span></span>
|<span data-ttu-id="0b546-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b546-107">Property</span></span>|<span data-ttu-id="0b546-108">类型</span><span class="sxs-lookup"><span data-stu-id="0b546-108">Type</span></span>|<span data-ttu-id="0b546-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b546-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b546-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="0b546-110">androidCount</span></span>|<span data-ttu-id="0b546-111">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-111">Int32</span></span>|<span data-ttu-id="0b546-112">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-112">Number of android device count.</span></span>|
|<span data-ttu-id="0b546-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="0b546-113">iosCount</span></span>|<span data-ttu-id="0b546-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-114">Int32</span></span>|<span data-ttu-id="0b546-115">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="0b546-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="0b546-116">macOSCount</span></span>|<span data-ttu-id="0b546-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-117">Int32</span></span>|<span data-ttu-id="0b546-118">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="0b546-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="0b546-119">windowsMobileCount</span></span>|<span data-ttu-id="0b546-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-120">Int32</span></span>|<span data-ttu-id="0b546-121">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="0b546-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="0b546-122">windowsCount</span></span>|<span data-ttu-id="0b546-123">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-123">Int32</span></span>|<span data-ttu-id="0b546-124">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="0b546-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="0b546-125">unknownCount</span></span>|<span data-ttu-id="0b546-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0b546-126">Int32</span></span>|<span data-ttu-id="0b546-127">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="0b546-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b546-128">关系</span><span class="sxs-lookup"><span data-stu-id="0b546-128">Relationships</span></span>
<span data-ttu-id="0b546-129">无</span><span class="sxs-lookup"><span data-stu-id="0b546-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b546-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b546-130">JSON Representation</span></span>
<span data-ttu-id="0b546-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b546-131">Here is a JSON representation of the resource.</span></span>
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



