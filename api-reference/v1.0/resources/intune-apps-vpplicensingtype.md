---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
ms.openlocfilehash: 7958266fe208e0a04bc72ab658291c58455c763b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322559"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="94a67-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="94a67-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="94a67-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94a67-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94a67-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="94a67-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="94a67-106">属性</span><span class="sxs-lookup"><span data-stu-id="94a67-106">Properties</span></span>
|<span data-ttu-id="94a67-107">属性</span><span class="sxs-lookup"><span data-stu-id="94a67-107">Property</span></span>|<span data-ttu-id="94a67-108">类型</span><span class="sxs-lookup"><span data-stu-id="94a67-108">Type</span></span>|<span data-ttu-id="94a67-109">说明</span><span class="sxs-lookup"><span data-stu-id="94a67-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94a67-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="94a67-110">supportsUserLicensing</span></span>|<span data-ttu-id="94a67-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="94a67-111">Boolean</span></span>|<span data-ttu-id="94a67-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="94a67-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="94a67-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="94a67-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="94a67-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="94a67-114">Boolean</span></span>|<span data-ttu-id="94a67-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="94a67-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94a67-116">关系</span><span class="sxs-lookup"><span data-stu-id="94a67-116">Relationships</span></span>
<span data-ttu-id="94a67-117">无</span><span class="sxs-lookup"><span data-stu-id="94a67-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94a67-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94a67-118">JSON Representation</span></span>
<span data-ttu-id="94a67-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a67-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



