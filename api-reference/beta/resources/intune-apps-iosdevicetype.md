---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c842d27d3113210d96479388d2395b24dea8f123
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798124"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="19c95-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="19c95-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="19c95-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19c95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19c95-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19c95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c95-106">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="19c95-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="19c95-107">属性</span><span class="sxs-lookup"><span data-stu-id="19c95-107">Properties</span></span>
|<span data-ttu-id="19c95-108">属性</span><span class="sxs-lookup"><span data-stu-id="19c95-108">Property</span></span>|<span data-ttu-id="19c95-109">类型</span><span class="sxs-lookup"><span data-stu-id="19c95-109">Type</span></span>|<span data-ttu-id="19c95-110">说明</span><span class="sxs-lookup"><span data-stu-id="19c95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c95-111">iPad</span><span class="sxs-lookup"><span data-stu-id="19c95-111">iPad</span></span>|<span data-ttu-id="19c95-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="19c95-112">Boolean</span></span>|<span data-ttu-id="19c95-113">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="19c95-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="19c95-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="19c95-114">iPhoneAndIPod</span></span>|<span data-ttu-id="19c95-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="19c95-115">Boolean</span></span>|<span data-ttu-id="19c95-116">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="19c95-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c95-117">关系</span><span class="sxs-lookup"><span data-stu-id="19c95-117">Relationships</span></span>
<span data-ttu-id="19c95-118">无</span><span class="sxs-lookup"><span data-stu-id="19c95-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19c95-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19c95-119">JSON Representation</span></span>
<span data-ttu-id="19c95-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19c95-120">Here is a JSON representation of the resource.</span></span>
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



