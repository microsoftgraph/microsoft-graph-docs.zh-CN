---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503525"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="57696-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="57696-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="57696-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57696-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57696-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="57696-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="57696-106">属性</span><span class="sxs-lookup"><span data-stu-id="57696-106">Properties</span></span>
|<span data-ttu-id="57696-107">属性</span><span class="sxs-lookup"><span data-stu-id="57696-107">Property</span></span>|<span data-ttu-id="57696-108">类型</span><span class="sxs-lookup"><span data-stu-id="57696-108">Type</span></span>|<span data-ttu-id="57696-109">说明</span><span class="sxs-lookup"><span data-stu-id="57696-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57696-110">iPad</span><span class="sxs-lookup"><span data-stu-id="57696-110">iPad</span></span>|<span data-ttu-id="57696-111">布尔</span><span class="sxs-lookup"><span data-stu-id="57696-111">Boolean</span></span>|<span data-ttu-id="57696-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="57696-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="57696-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="57696-113">iPhoneAndIPod</span></span>|<span data-ttu-id="57696-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="57696-114">Boolean</span></span>|<span data-ttu-id="57696-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="57696-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57696-116">关系</span><span class="sxs-lookup"><span data-stu-id="57696-116">Relationships</span></span>
<span data-ttu-id="57696-117">无</span><span class="sxs-lookup"><span data-stu-id="57696-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57696-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57696-118">JSON Representation</span></span>
<span data-ttu-id="57696-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57696-119">Here is a JSON representation of the resource.</span></span>
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



