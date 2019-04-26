---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571196"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="f7ae1-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7ae1-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="f7ae1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7ae1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ae1-105">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="f7ae1-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="f7ae1-106">属性</span><span class="sxs-lookup"><span data-stu-id="f7ae1-106">Properties</span></span>
|<span data-ttu-id="f7ae1-107">属性</span><span class="sxs-lookup"><span data-stu-id="f7ae1-107">Property</span></span>|<span data-ttu-id="f7ae1-108">类型</span><span class="sxs-lookup"><span data-stu-id="f7ae1-108">Type</span></span>|<span data-ttu-id="f7ae1-109">说明</span><span class="sxs-lookup"><span data-stu-id="f7ae1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ae1-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="f7ae1-110">platformBlocked</span></span>|<span data-ttu-id="f7ae1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7ae1-111">Boolean</span></span>|<span data-ttu-id="f7ae1-112">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="f7ae1-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="f7ae1-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="f7ae1-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="f7ae1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7ae1-114">Boolean</span></span>|<span data-ttu-id="f7ae1-115">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="f7ae1-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="f7ae1-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f7ae1-116">osMinimumVersion</span></span>|<span data-ttu-id="f7ae1-117">String</span><span class="sxs-lookup"><span data-stu-id="f7ae1-117">String</span></span>|<span data-ttu-id="f7ae1-118">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="f7ae1-118">Min OS version supported</span></span>|
|<span data-ttu-id="f7ae1-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f7ae1-119">osMaximumVersion</span></span>|<span data-ttu-id="f7ae1-120">String</span><span class="sxs-lookup"><span data-stu-id="f7ae1-120">String</span></span>|<span data-ttu-id="f7ae1-121">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="f7ae1-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7ae1-122">关系</span><span class="sxs-lookup"><span data-stu-id="f7ae1-122">Relationships</span></span>
<span data-ttu-id="f7ae1-123">无</span><span class="sxs-lookup"><span data-stu-id="f7ae1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7ae1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7ae1-124">JSON Representation</span></span>
<span data-ttu-id="f7ae1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7ae1-125">Here is a JSON representation of the resource.</span></span>
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



