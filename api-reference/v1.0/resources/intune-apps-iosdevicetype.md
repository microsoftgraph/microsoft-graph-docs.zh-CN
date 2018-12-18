---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: tfitzmac
ms.openlocfilehash: 3111bc4b5fc78f6ed60b4a241b48e443923f7159
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313599"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="e4cd7-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4cd7-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="e4cd7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4cd7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4cd7-105">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="e4cd7-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="e4cd7-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4cd7-106">Properties</span></span>
|<span data-ttu-id="e4cd7-107">属性</span><span class="sxs-lookup"><span data-stu-id="e4cd7-107">Property</span></span>|<span data-ttu-id="e4cd7-108">类型</span><span class="sxs-lookup"><span data-stu-id="e4cd7-108">Type</span></span>|<span data-ttu-id="e4cd7-109">说明</span><span class="sxs-lookup"><span data-stu-id="e4cd7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4cd7-110">iPad</span><span class="sxs-lookup"><span data-stu-id="e4cd7-110">iPad</span></span>|<span data-ttu-id="e4cd7-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4cd7-111">Boolean</span></span>|<span data-ttu-id="e4cd7-112">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="e4cd7-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="e4cd7-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="e4cd7-113">iPhoneAndIPod</span></span>|<span data-ttu-id="e4cd7-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4cd7-114">Boolean</span></span>|<span data-ttu-id="e4cd7-115">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="e4cd7-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4cd7-116">关系</span><span class="sxs-lookup"><span data-stu-id="e4cd7-116">Relationships</span></span>
<span data-ttu-id="e4cd7-117">无</span><span class="sxs-lookup"><span data-stu-id="e4cd7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4cd7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4cd7-118">JSON Representation</span></span>
<span data-ttu-id="e4cd7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4cd7-119">Here is a JSON representation of the resource.</span></span>
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



