---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5908d1e1d9d2c7eb902017bffdc533e33486f909
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940412"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="016aa-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="016aa-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="016aa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="016aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="016aa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="016aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="016aa-106">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="016aa-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="016aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="016aa-107">Properties</span></span>
|<span data-ttu-id="016aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="016aa-108">Property</span></span>|<span data-ttu-id="016aa-109">类型</span><span class="sxs-lookup"><span data-stu-id="016aa-109">Type</span></span>|<span data-ttu-id="016aa-110">说明</span><span class="sxs-lookup"><span data-stu-id="016aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="016aa-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="016aa-111">platformBlocked</span></span>|<span data-ttu-id="016aa-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="016aa-112">Boolean</span></span>|<span data-ttu-id="016aa-113">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="016aa-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="016aa-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="016aa-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="016aa-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="016aa-115">Boolean</span></span>|<span data-ttu-id="016aa-116">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="016aa-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="016aa-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="016aa-117">osMinimumVersion</span></span>|<span data-ttu-id="016aa-118">String</span><span class="sxs-lookup"><span data-stu-id="016aa-118">String</span></span>|<span data-ttu-id="016aa-119">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="016aa-119">Min OS version supported</span></span>|
|<span data-ttu-id="016aa-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="016aa-120">osMaximumVersion</span></span>|<span data-ttu-id="016aa-121">String</span><span class="sxs-lookup"><span data-stu-id="016aa-121">String</span></span>|<span data-ttu-id="016aa-122">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="016aa-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="016aa-123">关系</span><span class="sxs-lookup"><span data-stu-id="016aa-123">Relationships</span></span>
<span data-ttu-id="016aa-124">无</span><span class="sxs-lookup"><span data-stu-id="016aa-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="016aa-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="016aa-125">JSON Representation</span></span>
<span data-ttu-id="016aa-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="016aa-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```




