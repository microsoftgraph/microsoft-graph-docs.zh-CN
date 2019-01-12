---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b541310ced9c9aaa781077639203950d00f56f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976749"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e6376-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6376-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="e6376-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6376-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6376-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="e6376-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="e6376-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6376-106">Properties</span></span>
|<span data-ttu-id="e6376-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6376-107">Property</span></span>|<span data-ttu-id="e6376-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6376-108">Type</span></span>|<span data-ttu-id="e6376-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6376-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6376-110">iPad</span><span class="sxs-lookup"><span data-stu-id="e6376-110">iPad</span></span>|<span data-ttu-id="e6376-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="e6376-111">Boolean</span></span>|<span data-ttu-id="e6376-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="e6376-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e6376-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e6376-113">iPhoneAndIPod</span></span>|<span data-ttu-id="e6376-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="e6376-114">Boolean</span></span>|<span data-ttu-id="e6376-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="e6376-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6376-116">关系</span><span class="sxs-lookup"><span data-stu-id="e6376-116">Relationships</span></span>
<span data-ttu-id="e6376-117">无</span><span class="sxs-lookup"><span data-stu-id="e6376-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6376-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6376-118">JSON Representation</span></span>
<span data-ttu-id="e6376-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6376-119">Here is a JSON representation of the resource.</span></span>
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



