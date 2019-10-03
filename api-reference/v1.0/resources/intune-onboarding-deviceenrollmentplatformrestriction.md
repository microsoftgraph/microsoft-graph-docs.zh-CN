---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: edf64c6aaa2a9745b28543bd3dc3a458b7d8869e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367236"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8e73f-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e73f-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="8e73f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e73f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e73f-105">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="8e73f-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="8e73f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8e73f-106">Properties</span></span>
|<span data-ttu-id="8e73f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8e73f-107">Property</span></span>|<span data-ttu-id="8e73f-108">类型</span><span class="sxs-lookup"><span data-stu-id="8e73f-108">Type</span></span>|<span data-ttu-id="8e73f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8e73f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e73f-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8e73f-110">platformBlocked</span></span>|<span data-ttu-id="8e73f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e73f-111">Boolean</span></span>|<span data-ttu-id="8e73f-112">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="8e73f-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8e73f-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8e73f-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8e73f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e73f-114">Boolean</span></span>|<span data-ttu-id="8e73f-115">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="8e73f-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8e73f-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8e73f-116">osMinimumVersion</span></span>|<span data-ttu-id="8e73f-117">String</span><span class="sxs-lookup"><span data-stu-id="8e73f-117">String</span></span>|<span data-ttu-id="8e73f-118">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="8e73f-118">Min OS version supported</span></span>|
|<span data-ttu-id="8e73f-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8e73f-119">osMaximumVersion</span></span>|<span data-ttu-id="8e73f-120">String</span><span class="sxs-lookup"><span data-stu-id="8e73f-120">String</span></span>|<span data-ttu-id="8e73f-121">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="8e73f-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e73f-122">关系</span><span class="sxs-lookup"><span data-stu-id="8e73f-122">Relationships</span></span>
<span data-ttu-id="8e73f-123">无</span><span class="sxs-lookup"><span data-stu-id="8e73f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e73f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e73f-124">JSON Representation</span></span>
<span data-ttu-id="8e73f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e73f-125">Here is a JSON representation of the resource.</span></span>
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




