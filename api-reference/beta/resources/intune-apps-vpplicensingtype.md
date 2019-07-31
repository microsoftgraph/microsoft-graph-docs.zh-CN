---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe6e59ba5703d5c069781db6331f0ea6dbbfa240
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012378"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="83b0a-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="83b0a-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="83b0a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83b0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83b0a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83b0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83b0a-106">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="83b0a-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="83b0a-107">属性</span><span class="sxs-lookup"><span data-stu-id="83b0a-107">Properties</span></span>
|<span data-ttu-id="83b0a-108">属性</span><span class="sxs-lookup"><span data-stu-id="83b0a-108">Property</span></span>|<span data-ttu-id="83b0a-109">类型</span><span class="sxs-lookup"><span data-stu-id="83b0a-109">Type</span></span>|<span data-ttu-id="83b0a-110">说明</span><span class="sxs-lookup"><span data-stu-id="83b0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b0a-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="83b0a-111">supportUserLicensing</span></span>|<span data-ttu-id="83b0a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b0a-112">Boolean</span></span>|<span data-ttu-id="83b0a-113">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="83b0a-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="83b0a-114">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="83b0a-114">supportDeviceLicensing</span></span>|<span data-ttu-id="83b0a-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="83b0a-115">Boolean</span></span>|<span data-ttu-id="83b0a-116">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="83b0a-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="83b0a-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="83b0a-117">supportsUserLicensing</span></span>|<span data-ttu-id="83b0a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="83b0a-118">Boolean</span></span>|<span data-ttu-id="83b0a-119">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="83b0a-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="83b0a-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="83b0a-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="83b0a-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="83b0a-121">Boolean</span></span>|<span data-ttu-id="83b0a-122">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="83b0a-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83b0a-123">关系</span><span class="sxs-lookup"><span data-stu-id="83b0a-123">Relationships</span></span>
<span data-ttu-id="83b0a-124">无</span><span class="sxs-lookup"><span data-stu-id="83b0a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83b0a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83b0a-125">JSON Representation</span></span>
<span data-ttu-id="83b0a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83b0a-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





