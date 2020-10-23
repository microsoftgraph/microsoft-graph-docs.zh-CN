---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12cf34dd1ecf2bdad349bf5f20125b8484e22826
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707953"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="e479d-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="e479d-103">vppLicensingType resource type</span></span>

<span data-ttu-id="e479d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e479d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e479d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e479d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e479d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e479d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e479d-107">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="e479d-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="e479d-108">属性</span><span class="sxs-lookup"><span data-stu-id="e479d-108">Properties</span></span>
|<span data-ttu-id="e479d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e479d-109">Property</span></span>|<span data-ttu-id="e479d-110">类型</span><span class="sxs-lookup"><span data-stu-id="e479d-110">Type</span></span>|<span data-ttu-id="e479d-111">说明</span><span class="sxs-lookup"><span data-stu-id="e479d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e479d-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="e479d-112">supportUserLicensing</span></span>|<span data-ttu-id="e479d-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="e479d-113">Boolean</span></span>|<span data-ttu-id="e479d-114">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="e479d-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="e479d-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e479d-115">supportDeviceLicensing</span></span>|<span data-ttu-id="e479d-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="e479d-116">Boolean</span></span>|<span data-ttu-id="e479d-117">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="e479d-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="e479d-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="e479d-118">supportsUserLicensing</span></span>|<span data-ttu-id="e479d-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="e479d-119">Boolean</span></span>|<span data-ttu-id="e479d-120">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="e479d-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="e479d-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e479d-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="e479d-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="e479d-122">Boolean</span></span>|<span data-ttu-id="e479d-123">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="e479d-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e479d-124">关系</span><span class="sxs-lookup"><span data-stu-id="e479d-124">Relationships</span></span>
<span data-ttu-id="e479d-125">无</span><span class="sxs-lookup"><span data-stu-id="e479d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e479d-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e479d-126">JSON Representation</span></span>
<span data-ttu-id="e479d-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e479d-127">Here is a JSON representation of the resource.</span></span>
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





