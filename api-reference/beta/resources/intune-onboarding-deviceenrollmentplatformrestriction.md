---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed769c1e6550584688324f4bfdf2db772feae19c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524186"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8a866-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a866-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="8a866-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8a866-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a866-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a866-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a866-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a866-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a866-107">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="8a866-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="8a866-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a866-108">Properties</span></span>
|<span data-ttu-id="8a866-109">属性</span><span class="sxs-lookup"><span data-stu-id="8a866-109">Property</span></span>|<span data-ttu-id="8a866-110">类型</span><span class="sxs-lookup"><span data-stu-id="8a866-110">Type</span></span>|<span data-ttu-id="8a866-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a866-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a866-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8a866-112">platformBlocked</span></span>|<span data-ttu-id="8a866-113">布尔</span><span class="sxs-lookup"><span data-stu-id="8a866-113">Boolean</span></span>|<span data-ttu-id="8a866-114">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="8a866-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8a866-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8a866-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8a866-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a866-116">Boolean</span></span>|<span data-ttu-id="8a866-117">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="8a866-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8a866-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8a866-118">osMinimumVersion</span></span>|<span data-ttu-id="8a866-119">String</span><span class="sxs-lookup"><span data-stu-id="8a866-119">String</span></span>|<span data-ttu-id="8a866-120">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="8a866-120">Min OS version supported</span></span>|
|<span data-ttu-id="8a866-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8a866-121">osMaximumVersion</span></span>|<span data-ttu-id="8a866-122">String</span><span class="sxs-lookup"><span data-stu-id="8a866-122">String</span></span>|<span data-ttu-id="8a866-123">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="8a866-123">Max OS version supported</span></span>|
|<span data-ttu-id="8a866-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="8a866-124">blockedManufacturers</span></span>|<span data-ttu-id="8a866-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a866-125">String collection</span></span>|<span data-ttu-id="8a866-126">被阻止的制造商的集合。</span><span class="sxs-lookup"><span data-stu-id="8a866-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a866-127">关系</span><span class="sxs-lookup"><span data-stu-id="8a866-127">Relationships</span></span>
<span data-ttu-id="8a866-128">无</span><span class="sxs-lookup"><span data-stu-id="8a866-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a866-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a866-129">JSON Representation</span></span>
<span data-ttu-id="8a866-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a866-130">Here is a JSON representation of the resource.</span></span>
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



