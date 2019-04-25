---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8ba3306c5a4af4dfbb8b97e4d4794b917ebbf64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566649"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2a126-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a126-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2a126-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a126-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a126-106">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="2a126-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="2a126-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a126-107">Properties</span></span>
|<span data-ttu-id="2a126-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a126-108">Property</span></span>|<span data-ttu-id="2a126-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a126-109">Type</span></span>|<span data-ttu-id="2a126-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a126-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a126-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2a126-111">platformBlocked</span></span>|<span data-ttu-id="2a126-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a126-112">Boolean</span></span>|<span data-ttu-id="2a126-113">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="2a126-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2a126-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2a126-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2a126-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a126-115">Boolean</span></span>|<span data-ttu-id="2a126-116">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="2a126-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2a126-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2a126-117">osMinimumVersion</span></span>|<span data-ttu-id="2a126-118">String</span><span class="sxs-lookup"><span data-stu-id="2a126-118">String</span></span>|<span data-ttu-id="2a126-119">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="2a126-119">Min OS version supported</span></span>|
|<span data-ttu-id="2a126-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2a126-120">osMaximumVersion</span></span>|<span data-ttu-id="2a126-121">String</span><span class="sxs-lookup"><span data-stu-id="2a126-121">String</span></span>|<span data-ttu-id="2a126-122">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="2a126-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a126-123">关系</span><span class="sxs-lookup"><span data-stu-id="2a126-123">Relationships</span></span>
<span data-ttu-id="2a126-124">无</span><span class="sxs-lookup"><span data-stu-id="2a126-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a126-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a126-125">JSON Representation</span></span>
<span data-ttu-id="2a126-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a126-126">Here is a JSON representation of the resource.</span></span>
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





