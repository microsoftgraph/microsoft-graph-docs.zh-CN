---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26f29427dfe863ed1b89eaef5025655dc07430fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636593"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="693ec-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="693ec-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="693ec-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="693ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="693ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="693ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="693ec-106">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="693ec-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="693ec-107">属性</span><span class="sxs-lookup"><span data-stu-id="693ec-107">Properties</span></span>
|<span data-ttu-id="693ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="693ec-108">Property</span></span>|<span data-ttu-id="693ec-109">类型</span><span class="sxs-lookup"><span data-stu-id="693ec-109">Type</span></span>|<span data-ttu-id="693ec-110">Description</span><span class="sxs-lookup"><span data-stu-id="693ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693ec-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="693ec-111">platformBlocked</span></span>|<span data-ttu-id="693ec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="693ec-112">Boolean</span></span>|<span data-ttu-id="693ec-113">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="693ec-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="693ec-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="693ec-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="693ec-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="693ec-115">Boolean</span></span>|<span data-ttu-id="693ec-116">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="693ec-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="693ec-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="693ec-117">osMinimumVersion</span></span>|<span data-ttu-id="693ec-118">字符串</span><span class="sxs-lookup"><span data-stu-id="693ec-118">String</span></span>|<span data-ttu-id="693ec-119">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="693ec-119">Min OS version supported</span></span>|
|<span data-ttu-id="693ec-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="693ec-120">osMaximumVersion</span></span>|<span data-ttu-id="693ec-121">String</span><span class="sxs-lookup"><span data-stu-id="693ec-121">String</span></span>|<span data-ttu-id="693ec-122">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="693ec-122">Max OS version supported</span></span>|
|<span data-ttu-id="693ec-123">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="693ec-123">blockedManufacturers</span></span>|<span data-ttu-id="693ec-124">String 集合</span><span class="sxs-lookup"><span data-stu-id="693ec-124">String collection</span></span>|<span data-ttu-id="693ec-125">被阻止的制造商的集合。</span><span class="sxs-lookup"><span data-stu-id="693ec-125">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="693ec-126">关系</span><span class="sxs-lookup"><span data-stu-id="693ec-126">Relationships</span></span>
<span data-ttu-id="693ec-127">无</span><span class="sxs-lookup"><span data-stu-id="693ec-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="693ec-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="693ec-128">JSON Representation</span></span>
<span data-ttu-id="693ec-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="693ec-129">Here is a JSON representation of the resource.</span></span>
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
  "osMaximumVersion": "String",
  "blockedManufacturers": [
    "String"
  ]
}
```



