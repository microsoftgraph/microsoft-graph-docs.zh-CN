---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 587c5e319490807369590585e53a06e0dcc7f2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37369056"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="05710-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="05710-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="05710-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05710-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05710-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="05710-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="05710-106">属性</span><span class="sxs-lookup"><span data-stu-id="05710-106">Properties</span></span>
|<span data-ttu-id="05710-107">属性</span><span class="sxs-lookup"><span data-stu-id="05710-107">Property</span></span>|<span data-ttu-id="05710-108">类型</span><span class="sxs-lookup"><span data-stu-id="05710-108">Type</span></span>|<span data-ttu-id="05710-109">说明</span><span class="sxs-lookup"><span data-stu-id="05710-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05710-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="05710-110">supportsUserLicensing</span></span>|<span data-ttu-id="05710-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="05710-111">Boolean</span></span>|<span data-ttu-id="05710-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="05710-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="05710-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="05710-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="05710-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="05710-114">Boolean</span></span>|<span data-ttu-id="05710-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="05710-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05710-116">关系</span><span class="sxs-lookup"><span data-stu-id="05710-116">Relationships</span></span>
<span data-ttu-id="05710-117">无</span><span class="sxs-lookup"><span data-stu-id="05710-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05710-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05710-118">JSON Representation</span></span>
<span data-ttu-id="05710-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05710-119">Here is a JSON representation of the resource.</span></span>
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




