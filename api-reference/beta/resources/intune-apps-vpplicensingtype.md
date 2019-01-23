---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399673"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="13a57-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="13a57-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="13a57-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="13a57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13a57-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="13a57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13a57-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13a57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a57-107">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="13a57-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="13a57-108">属性</span><span class="sxs-lookup"><span data-stu-id="13a57-108">Properties</span></span>
|<span data-ttu-id="13a57-109">属性</span><span class="sxs-lookup"><span data-stu-id="13a57-109">Property</span></span>|<span data-ttu-id="13a57-110">类型</span><span class="sxs-lookup"><span data-stu-id="13a57-110">Type</span></span>|<span data-ttu-id="13a57-111">说明</span><span class="sxs-lookup"><span data-stu-id="13a57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a57-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="13a57-112">supportUserLicensing</span></span>|<span data-ttu-id="13a57-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="13a57-113">Boolean</span></span>|<span data-ttu-id="13a57-114">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="13a57-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="13a57-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="13a57-115">supportDeviceLicensing</span></span>|<span data-ttu-id="13a57-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="13a57-116">Boolean</span></span>|<span data-ttu-id="13a57-117">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="13a57-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="13a57-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="13a57-118">supportsUserLicensing</span></span>|<span data-ttu-id="13a57-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="13a57-119">Boolean</span></span>|<span data-ttu-id="13a57-120">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="13a57-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="13a57-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="13a57-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="13a57-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="13a57-122">Boolean</span></span>|<span data-ttu-id="13a57-123">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="13a57-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13a57-124">关系</span><span class="sxs-lookup"><span data-stu-id="13a57-124">Relationships</span></span>
<span data-ttu-id="13a57-125">无</span><span class="sxs-lookup"><span data-stu-id="13a57-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13a57-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13a57-126">JSON Representation</span></span>
<span data-ttu-id="13a57-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13a57-127">Here is a JSON representation of the resource.</span></span>
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




