---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bf4748d8dc083fe03b55b5ee88062ebb429f639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422857"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="173da-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="173da-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="173da-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="173da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="173da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="173da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="173da-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="173da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="173da-107">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="173da-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="173da-108">属性</span><span class="sxs-lookup"><span data-stu-id="173da-108">Properties</span></span>
|<span data-ttu-id="173da-109">属性</span><span class="sxs-lookup"><span data-stu-id="173da-109">Property</span></span>|<span data-ttu-id="173da-110">类型</span><span class="sxs-lookup"><span data-stu-id="173da-110">Type</span></span>|<span data-ttu-id="173da-111">说明</span><span class="sxs-lookup"><span data-stu-id="173da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173da-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="173da-112">platformBlocked</span></span>|<span data-ttu-id="173da-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="173da-113">Boolean</span></span>|<span data-ttu-id="173da-114">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="173da-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="173da-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="173da-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="173da-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="173da-116">Boolean</span></span>|<span data-ttu-id="173da-117">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="173da-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="173da-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="173da-118">osMinimumVersion</span></span>|<span data-ttu-id="173da-119">String</span><span class="sxs-lookup"><span data-stu-id="173da-119">String</span></span>|<span data-ttu-id="173da-120">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="173da-120">Min OS version supported</span></span>|
|<span data-ttu-id="173da-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="173da-121">osMaximumVersion</span></span>|<span data-ttu-id="173da-122">String</span><span class="sxs-lookup"><span data-stu-id="173da-122">String</span></span>|<span data-ttu-id="173da-123">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="173da-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="173da-124">关系</span><span class="sxs-lookup"><span data-stu-id="173da-124">Relationships</span></span>
<span data-ttu-id="173da-125">无</span><span class="sxs-lookup"><span data-stu-id="173da-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="173da-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="173da-126">JSON Representation</span></span>
<span data-ttu-id="173da-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="173da-127">Here is a JSON representation of the resource.</span></span>
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




