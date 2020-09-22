---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c621eb9fc0b90e752d46b8ab1a3d75a927c16051
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086542"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="9db80-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db80-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="9db80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9db80-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9db80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9db80-106">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="9db80-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="9db80-107">属性</span><span class="sxs-lookup"><span data-stu-id="9db80-107">Properties</span></span>
|<span data-ttu-id="9db80-108">属性</span><span class="sxs-lookup"><span data-stu-id="9db80-108">Property</span></span>|<span data-ttu-id="9db80-109">类型</span><span class="sxs-lookup"><span data-stu-id="9db80-109">Type</span></span>|<span data-ttu-id="9db80-110">说明</span><span class="sxs-lookup"><span data-stu-id="9db80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db80-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="9db80-111">platformBlocked</span></span>|<span data-ttu-id="9db80-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="9db80-112">Boolean</span></span>|<span data-ttu-id="9db80-113">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="9db80-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="9db80-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="9db80-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="9db80-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9db80-115">Boolean</span></span>|<span data-ttu-id="9db80-116">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="9db80-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="9db80-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9db80-117">osMinimumVersion</span></span>|<span data-ttu-id="9db80-118">String</span><span class="sxs-lookup"><span data-stu-id="9db80-118">String</span></span>|<span data-ttu-id="9db80-119">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="9db80-119">Min OS version supported</span></span>|
|<span data-ttu-id="9db80-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9db80-120">osMaximumVersion</span></span>|<span data-ttu-id="9db80-121">String</span><span class="sxs-lookup"><span data-stu-id="9db80-121">String</span></span>|<span data-ttu-id="9db80-122">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="9db80-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="9db80-123">关系</span><span class="sxs-lookup"><span data-stu-id="9db80-123">Relationships</span></span>
<span data-ttu-id="9db80-124">无</span><span class="sxs-lookup"><span data-stu-id="9db80-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9db80-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9db80-125">JSON Representation</span></span>
<span data-ttu-id="9db80-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db80-126">Here is a JSON representation of the resource.</span></span>
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









