---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259743"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="66716-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="66716-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="66716-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66716-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66716-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="66716-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="66716-106">属性</span><span class="sxs-lookup"><span data-stu-id="66716-106">Properties</span></span>
|<span data-ttu-id="66716-107">属性</span><span class="sxs-lookup"><span data-stu-id="66716-107">Property</span></span>|<span data-ttu-id="66716-108">类型</span><span class="sxs-lookup"><span data-stu-id="66716-108">Type</span></span>|<span data-ttu-id="66716-109">说明</span><span class="sxs-lookup"><span data-stu-id="66716-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66716-110">iPad</span><span class="sxs-lookup"><span data-stu-id="66716-110">iPad</span></span>|<span data-ttu-id="66716-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="66716-111">Boolean</span></span>|<span data-ttu-id="66716-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="66716-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="66716-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="66716-113">iPhoneAndIPod</span></span>|<span data-ttu-id="66716-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="66716-114">Boolean</span></span>|<span data-ttu-id="66716-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="66716-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66716-116">关系</span><span class="sxs-lookup"><span data-stu-id="66716-116">Relationships</span></span>
<span data-ttu-id="66716-117">无</span><span class="sxs-lookup"><span data-stu-id="66716-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66716-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66716-118">JSON Representation</span></span>
<span data-ttu-id="66716-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66716-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```



