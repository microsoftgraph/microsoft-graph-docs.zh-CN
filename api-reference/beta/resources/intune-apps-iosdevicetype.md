---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 312db37bcd7f8750f35db55d0303ece2f875415b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493690"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="c27fd-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="c27fd-103">iosDeviceType resource type</span></span>

<span data-ttu-id="c27fd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c27fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c27fd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c27fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c27fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c27fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c27fd-107">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="c27fd-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="c27fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="c27fd-108">Properties</span></span>
|<span data-ttu-id="c27fd-109">属性</span><span class="sxs-lookup"><span data-stu-id="c27fd-109">Property</span></span>|<span data-ttu-id="c27fd-110">类型</span><span class="sxs-lookup"><span data-stu-id="c27fd-110">Type</span></span>|<span data-ttu-id="c27fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="c27fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c27fd-112">iPad</span><span class="sxs-lookup"><span data-stu-id="c27fd-112">iPad</span></span>|<span data-ttu-id="c27fd-113">布尔</span><span class="sxs-lookup"><span data-stu-id="c27fd-113">Boolean</span></span>|<span data-ttu-id="c27fd-114">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="c27fd-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="c27fd-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="c27fd-115">iPhoneAndIPod</span></span>|<span data-ttu-id="c27fd-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="c27fd-116">Boolean</span></span>|<span data-ttu-id="c27fd-117">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="c27fd-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c27fd-118">关系</span><span class="sxs-lookup"><span data-stu-id="c27fd-118">Relationships</span></span>
<span data-ttu-id="c27fd-119">无</span><span class="sxs-lookup"><span data-stu-id="c27fd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c27fd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c27fd-120">JSON Representation</span></span>
<span data-ttu-id="c27fd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c27fd-121">Here is a JSON representation of the resource.</span></span>
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



