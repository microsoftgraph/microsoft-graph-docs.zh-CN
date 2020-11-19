---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05105eec5b3b870ee608d0b47861d1eaddae8965
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301275"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="1a7bd-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a7bd-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="1a7bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a7bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a7bd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a7bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a7bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a7bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a7bd-107">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="1a7bd-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="1a7bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a7bd-108">Properties</span></span>
|<span data-ttu-id="1a7bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="1a7bd-109">Property</span></span>|<span data-ttu-id="1a7bd-110">类型</span><span class="sxs-lookup"><span data-stu-id="1a7bd-110">Type</span></span>|<span data-ttu-id="1a7bd-111">Description</span><span class="sxs-lookup"><span data-stu-id="1a7bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7bd-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="1a7bd-112">platformBlocked</span></span>|<span data-ttu-id="1a7bd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a7bd-113">Boolean</span></span>|<span data-ttu-id="1a7bd-114">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="1a7bd-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="1a7bd-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="1a7bd-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="1a7bd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a7bd-116">Boolean</span></span>|<span data-ttu-id="1a7bd-117">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="1a7bd-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="1a7bd-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1a7bd-118">osMinimumVersion</span></span>|<span data-ttu-id="1a7bd-119">String</span><span class="sxs-lookup"><span data-stu-id="1a7bd-119">String</span></span>|<span data-ttu-id="1a7bd-120">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="1a7bd-120">Min OS version supported</span></span>|
|<span data-ttu-id="1a7bd-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1a7bd-121">osMaximumVersion</span></span>|<span data-ttu-id="1a7bd-122">String</span><span class="sxs-lookup"><span data-stu-id="1a7bd-122">String</span></span>|<span data-ttu-id="1a7bd-123">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="1a7bd-123">Max OS version supported</span></span>|
|<span data-ttu-id="1a7bd-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="1a7bd-124">blockedManufacturers</span></span>|<span data-ttu-id="1a7bd-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a7bd-125">String collection</span></span>|<span data-ttu-id="1a7bd-126">被阻止的制造商的集合。</span><span class="sxs-lookup"><span data-stu-id="1a7bd-126">Collection of blocked Manufacturers.</span></span>|
|<span data-ttu-id="1a7bd-127">blockedSkus</span><span class="sxs-lookup"><span data-stu-id="1a7bd-127">blockedSkus</span></span>|<span data-ttu-id="1a7bd-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a7bd-128">String collection</span></span>|<span data-ttu-id="1a7bd-129">阻止的 Sku 的集合。</span><span class="sxs-lookup"><span data-stu-id="1a7bd-129">Collection of blocked Skus.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a7bd-130">关系</span><span class="sxs-lookup"><span data-stu-id="1a7bd-130">Relationships</span></span>
<span data-ttu-id="1a7bd-131">无</span><span class="sxs-lookup"><span data-stu-id="1a7bd-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a7bd-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a7bd-132">JSON Representation</span></span>
<span data-ttu-id="1a7bd-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a7bd-133">Here is a JSON representation of the resource.</span></span>
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
  ],
  "blockedSkus": [
    "String"
  ]
}
```




