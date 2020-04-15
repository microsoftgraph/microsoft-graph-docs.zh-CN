---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77533c24fe08d6d949c2b50776c92295ac2ad0d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397289"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="161a0-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="161a0-103">iosDeviceType resource type</span></span>

<span data-ttu-id="161a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="161a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="161a0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="161a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="161a0-106">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="161a0-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="161a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="161a0-107">Properties</span></span>
|<span data-ttu-id="161a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="161a0-108">Property</span></span>|<span data-ttu-id="161a0-109">类型</span><span class="sxs-lookup"><span data-stu-id="161a0-109">Type</span></span>|<span data-ttu-id="161a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="161a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="161a0-111">iPad</span><span class="sxs-lookup"><span data-stu-id="161a0-111">iPad</span></span>|<span data-ttu-id="161a0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="161a0-112">Boolean</span></span>|<span data-ttu-id="161a0-113">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="161a0-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="161a0-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="161a0-114">iPhoneAndIPod</span></span>|<span data-ttu-id="161a0-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="161a0-115">Boolean</span></span>|<span data-ttu-id="161a0-116">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="161a0-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="161a0-117">关系</span><span class="sxs-lookup"><span data-stu-id="161a0-117">Relationships</span></span>
<span data-ttu-id="161a0-118">无</span><span class="sxs-lookup"><span data-stu-id="161a0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="161a0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="161a0-119">JSON Representation</span></span>
<span data-ttu-id="161a0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="161a0-120">Here is a JSON representation of the resource.</span></span>
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







