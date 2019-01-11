---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ffa46d1e8fb693822051250fb4a722815b1dcb73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866778"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="d66ee-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="d66ee-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="d66ee-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d66ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d66ee-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="d66ee-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="d66ee-106">属性</span><span class="sxs-lookup"><span data-stu-id="d66ee-106">Properties</span></span>
|<span data-ttu-id="d66ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="d66ee-107">Property</span></span>|<span data-ttu-id="d66ee-108">类型</span><span class="sxs-lookup"><span data-stu-id="d66ee-108">Type</span></span>|<span data-ttu-id="d66ee-109">说明</span><span class="sxs-lookup"><span data-stu-id="d66ee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d66ee-110">iPad</span><span class="sxs-lookup"><span data-stu-id="d66ee-110">iPad</span></span>|<span data-ttu-id="d66ee-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="d66ee-111">Boolean</span></span>|<span data-ttu-id="d66ee-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="d66ee-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="d66ee-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="d66ee-113">iPhoneAndIPod</span></span>|<span data-ttu-id="d66ee-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="d66ee-114">Boolean</span></span>|<span data-ttu-id="d66ee-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="d66ee-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d66ee-116">关系</span><span class="sxs-lookup"><span data-stu-id="d66ee-116">Relationships</span></span>
<span data-ttu-id="d66ee-117">无</span><span class="sxs-lookup"><span data-stu-id="d66ee-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d66ee-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d66ee-118">JSON Representation</span></span>
<span data-ttu-id="d66ee-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d66ee-119">Here is a JSON representation of the resource.</span></span>
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



