---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
ms.openlocfilehash: c9f691c2fdeb25bad54c105450c71dd7c65f30b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342754"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="6d292-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d292-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="6d292-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6d292-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d292-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6d292-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d292-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6d292-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d292-107">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="6d292-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="6d292-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d292-108">Properties</span></span>
|<span data-ttu-id="6d292-109">属性</span><span class="sxs-lookup"><span data-stu-id="6d292-109">Property</span></span>|<span data-ttu-id="6d292-110">类型</span><span class="sxs-lookup"><span data-stu-id="6d292-110">Type</span></span>|<span data-ttu-id="6d292-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d292-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d292-112">iPad</span><span class="sxs-lookup"><span data-stu-id="6d292-112">iPad</span></span>|<span data-ttu-id="6d292-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="6d292-113">Boolean</span></span>|<span data-ttu-id="6d292-114">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="6d292-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="6d292-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="6d292-115">iPhoneAndIPod</span></span>|<span data-ttu-id="6d292-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="6d292-116">Boolean</span></span>|<span data-ttu-id="6d292-117">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="6d292-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d292-118">关系</span><span class="sxs-lookup"><span data-stu-id="6d292-118">Relationships</span></span>
<span data-ttu-id="6d292-119">无</span><span class="sxs-lookup"><span data-stu-id="6d292-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d292-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d292-120">JSON Representation</span></span>
<span data-ttu-id="6d292-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d292-121">Here is a JSON representation of the resource.</span></span>
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





