---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a62cb711b70352d98650ae03945316de9ed2b5d2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356251"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="0522b-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="0522b-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="0522b-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0522b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0522b-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="0522b-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="0522b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0522b-106">Properties</span></span>
|<span data-ttu-id="0522b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0522b-107">Property</span></span>|<span data-ttu-id="0522b-108">类型</span><span class="sxs-lookup"><span data-stu-id="0522b-108">Type</span></span>|<span data-ttu-id="0522b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0522b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0522b-110">iPad</span><span class="sxs-lookup"><span data-stu-id="0522b-110">iPad</span></span>|<span data-ttu-id="0522b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0522b-111">Boolean</span></span>|<span data-ttu-id="0522b-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="0522b-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="0522b-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="0522b-113">iPhoneAndIPod</span></span>|<span data-ttu-id="0522b-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="0522b-114">Boolean</span></span>|<span data-ttu-id="0522b-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="0522b-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0522b-116">关系</span><span class="sxs-lookup"><span data-stu-id="0522b-116">Relationships</span></span>
<span data-ttu-id="0522b-117">无</span><span class="sxs-lookup"><span data-stu-id="0522b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0522b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0522b-118">JSON Representation</span></span>
<span data-ttu-id="0522b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0522b-119">Here is a JSON representation of the resource.</span></span>
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




