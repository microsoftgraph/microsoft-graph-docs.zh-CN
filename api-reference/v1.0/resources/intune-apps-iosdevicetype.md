---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
ms.openlocfilehash: b14abbb6713daf9fad7b0d2fd6f7865d251b6147
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009633"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="a9a77-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9a77-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="a9a77-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a9a77-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9a77-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="a9a77-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="a9a77-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9a77-106">Properties</span></span>
|<span data-ttu-id="a9a77-107">属性</span><span class="sxs-lookup"><span data-stu-id="a9a77-107">Property</span></span>|<span data-ttu-id="a9a77-108">类型</span><span class="sxs-lookup"><span data-stu-id="a9a77-108">Type</span></span>|<span data-ttu-id="a9a77-109">说明</span><span class="sxs-lookup"><span data-stu-id="a9a77-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9a77-110">iPad</span><span class="sxs-lookup"><span data-stu-id="a9a77-110">iPad</span></span>|<span data-ttu-id="a9a77-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="a9a77-111">Boolean</span></span>|<span data-ttu-id="a9a77-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="a9a77-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="a9a77-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="a9a77-113">iPhoneAndIPod</span></span>|<span data-ttu-id="a9a77-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="a9a77-114">Boolean</span></span>|<span data-ttu-id="a9a77-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="a9a77-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9a77-116">关系</span><span class="sxs-lookup"><span data-stu-id="a9a77-116">Relationships</span></span>
<span data-ttu-id="a9a77-117">无</span><span class="sxs-lookup"><span data-stu-id="a9a77-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9a77-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9a77-118">JSON Representation</span></span>
<span data-ttu-id="a9a77-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9a77-119">Here is a JSON representation of the resource.</span></span>
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



