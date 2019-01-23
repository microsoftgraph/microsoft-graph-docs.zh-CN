---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68c7ce163dbf0f9232bf53d919ae84c7906c997
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395382"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="596d9-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="596d9-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="596d9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="596d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="596d9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="596d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="596d9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="596d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="596d9-107">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="596d9-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="596d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="596d9-108">Properties</span></span>
|<span data-ttu-id="596d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="596d9-109">Property</span></span>|<span data-ttu-id="596d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="596d9-110">Type</span></span>|<span data-ttu-id="596d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="596d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="596d9-112">iPad</span><span class="sxs-lookup"><span data-stu-id="596d9-112">iPad</span></span>|<span data-ttu-id="596d9-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="596d9-113">Boolean</span></span>|<span data-ttu-id="596d9-114">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="596d9-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="596d9-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="596d9-115">iPhoneAndIPod</span></span>|<span data-ttu-id="596d9-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="596d9-116">Boolean</span></span>|<span data-ttu-id="596d9-117">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="596d9-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="596d9-118">关系</span><span class="sxs-lookup"><span data-stu-id="596d9-118">Relationships</span></span>
<span data-ttu-id="596d9-119">无</span><span class="sxs-lookup"><span data-stu-id="596d9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="596d9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="596d9-120">JSON Representation</span></span>
<span data-ttu-id="596d9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="596d9-121">Here is a JSON representation of the resource.</span></span>
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




