---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4b7983d20f22be5f8cce24a5c362926d00de55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851595"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="11ac5-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="11ac5-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="11ac5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="11ac5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11ac5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="11ac5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11ac5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="11ac5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11ac5-107">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="11ac5-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="11ac5-108">属性</span><span class="sxs-lookup"><span data-stu-id="11ac5-108">Properties</span></span>
|<span data-ttu-id="11ac5-109">属性</span><span class="sxs-lookup"><span data-stu-id="11ac5-109">Property</span></span>|<span data-ttu-id="11ac5-110">类型</span><span class="sxs-lookup"><span data-stu-id="11ac5-110">Type</span></span>|<span data-ttu-id="11ac5-111">Description</span><span class="sxs-lookup"><span data-stu-id="11ac5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ac5-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="11ac5-112">supportUserLicensing</span></span>|<span data-ttu-id="11ac5-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="11ac5-113">Boolean</span></span>|<span data-ttu-id="11ac5-114">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="11ac5-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="11ac5-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="11ac5-115">supportDeviceLicensing</span></span>|<span data-ttu-id="11ac5-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="11ac5-116">Boolean</span></span>|<span data-ttu-id="11ac5-117">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="11ac5-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="11ac5-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="11ac5-118">supportsUserLicensing</span></span>|<span data-ttu-id="11ac5-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="11ac5-119">Boolean</span></span>|<span data-ttu-id="11ac5-120">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="11ac5-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="11ac5-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="11ac5-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="11ac5-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="11ac5-122">Boolean</span></span>|<span data-ttu-id="11ac5-123">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="11ac5-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11ac5-124">关系</span><span class="sxs-lookup"><span data-stu-id="11ac5-124">Relationships</span></span>
<span data-ttu-id="11ac5-125">无</span><span class="sxs-lookup"><span data-stu-id="11ac5-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11ac5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11ac5-126">JSON Representation</span></span>
<span data-ttu-id="11ac5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11ac5-127">Here is a JSON representation of the resource.</span></span>
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





