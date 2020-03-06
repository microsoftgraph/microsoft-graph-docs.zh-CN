---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 057de993f7e9cef948c3334b8dcb22e34f49ba23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531240"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="74d21-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="74d21-103">iosDeviceType resource type</span></span>

<span data-ttu-id="74d21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74d21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74d21-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74d21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74d21-106">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="74d21-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="74d21-107">属性</span><span class="sxs-lookup"><span data-stu-id="74d21-107">Properties</span></span>
|<span data-ttu-id="74d21-108">属性</span><span class="sxs-lookup"><span data-stu-id="74d21-108">Property</span></span>|<span data-ttu-id="74d21-109">类型</span><span class="sxs-lookup"><span data-stu-id="74d21-109">Type</span></span>|<span data-ttu-id="74d21-110">说明</span><span class="sxs-lookup"><span data-stu-id="74d21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74d21-111">iPad</span><span class="sxs-lookup"><span data-stu-id="74d21-111">iPad</span></span>|<span data-ttu-id="74d21-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="74d21-112">Boolean</span></span>|<span data-ttu-id="74d21-113">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="74d21-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="74d21-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="74d21-114">iPhoneAndIPod</span></span>|<span data-ttu-id="74d21-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="74d21-115">Boolean</span></span>|<span data-ttu-id="74d21-116">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="74d21-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74d21-117">关系</span><span class="sxs-lookup"><span data-stu-id="74d21-117">Relationships</span></span>
<span data-ttu-id="74d21-118">无</span><span class="sxs-lookup"><span data-stu-id="74d21-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74d21-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74d21-119">JSON Representation</span></span>
<span data-ttu-id="74d21-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74d21-120">Here is a JSON representation of the resource.</span></span>
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




