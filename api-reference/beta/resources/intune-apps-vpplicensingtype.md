---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f31388de57835ea91ae3dc9fd104dd3b74b0ae32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362763"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="1dc17-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="1dc17-103">vppLicensingType resource type</span></span>

<span data-ttu-id="1dc17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dc17-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dc17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dc17-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dc17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc17-107">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="1dc17-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="1dc17-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dc17-108">Properties</span></span>
|<span data-ttu-id="1dc17-109">属性</span><span class="sxs-lookup"><span data-stu-id="1dc17-109">Property</span></span>|<span data-ttu-id="1dc17-110">类型</span><span class="sxs-lookup"><span data-stu-id="1dc17-110">Type</span></span>|<span data-ttu-id="1dc17-111">说明</span><span class="sxs-lookup"><span data-stu-id="1dc17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc17-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="1dc17-112">supportUserLicensing</span></span>|<span data-ttu-id="1dc17-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc17-113">Boolean</span></span>|<span data-ttu-id="1dc17-114">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="1dc17-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="1dc17-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1dc17-115">supportDeviceLicensing</span></span>|<span data-ttu-id="1dc17-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="1dc17-116">Boolean</span></span>|<span data-ttu-id="1dc17-117">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="1dc17-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="1dc17-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="1dc17-118">supportsUserLicensing</span></span>|<span data-ttu-id="1dc17-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc17-119">Boolean</span></span>|<span data-ttu-id="1dc17-120">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="1dc17-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="1dc17-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1dc17-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="1dc17-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="1dc17-122">Boolean</span></span>|<span data-ttu-id="1dc17-123">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="1dc17-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dc17-124">关系</span><span class="sxs-lookup"><span data-stu-id="1dc17-124">Relationships</span></span>
<span data-ttu-id="1dc17-125">无</span><span class="sxs-lookup"><span data-stu-id="1dc17-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dc17-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1dc17-126">JSON Representation</span></span>
<span data-ttu-id="1dc17-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dc17-127">Here is a JSON representation of the resource.</span></span>
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



