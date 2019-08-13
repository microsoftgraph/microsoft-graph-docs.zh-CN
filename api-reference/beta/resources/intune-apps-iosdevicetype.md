---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ea8f52e41a8cc363975dd3bb2f8bd22d1990d1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366075"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e636c-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e636c-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="e636c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e636c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e636c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e636c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e636c-106">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="e636c-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="e636c-107">属性</span><span class="sxs-lookup"><span data-stu-id="e636c-107">Properties</span></span>
|<span data-ttu-id="e636c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e636c-108">Property</span></span>|<span data-ttu-id="e636c-109">类型</span><span class="sxs-lookup"><span data-stu-id="e636c-109">Type</span></span>|<span data-ttu-id="e636c-110">说明</span><span class="sxs-lookup"><span data-stu-id="e636c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e636c-111">iPad</span><span class="sxs-lookup"><span data-stu-id="e636c-111">iPad</span></span>|<span data-ttu-id="e636c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e636c-112">Boolean</span></span>|<span data-ttu-id="e636c-113">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="e636c-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e636c-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e636c-114">iPhoneAndIPod</span></span>|<span data-ttu-id="e636c-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e636c-115">Boolean</span></span>|<span data-ttu-id="e636c-116">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="e636c-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e636c-117">关系</span><span class="sxs-lookup"><span data-stu-id="e636c-117">Relationships</span></span>
<span data-ttu-id="e636c-118">无</span><span class="sxs-lookup"><span data-stu-id="e636c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e636c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e636c-119">JSON Representation</span></span>
<span data-ttu-id="e636c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e636c-120">Here is a JSON representation of the resource.</span></span>
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



