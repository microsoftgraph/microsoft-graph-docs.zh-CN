---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5189b286de61375715944c5ac979d847392a18c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917760"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="52d61-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="52d61-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="52d61-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="52d61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52d61-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="52d61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52d61-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="52d61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52d61-107">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="52d61-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="52d61-108">属性</span><span class="sxs-lookup"><span data-stu-id="52d61-108">Properties</span></span>
|<span data-ttu-id="52d61-109">属性</span><span class="sxs-lookup"><span data-stu-id="52d61-109">Property</span></span>|<span data-ttu-id="52d61-110">类型</span><span class="sxs-lookup"><span data-stu-id="52d61-110">Type</span></span>|<span data-ttu-id="52d61-111">说明</span><span class="sxs-lookup"><span data-stu-id="52d61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d61-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="52d61-112">platformBlocked</span></span>|<span data-ttu-id="52d61-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="52d61-113">Boolean</span></span>|<span data-ttu-id="52d61-114">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="52d61-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="52d61-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="52d61-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="52d61-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="52d61-116">Boolean</span></span>|<span data-ttu-id="52d61-117">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="52d61-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="52d61-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="52d61-118">osMinimumVersion</span></span>|<span data-ttu-id="52d61-119">String</span><span class="sxs-lookup"><span data-stu-id="52d61-119">String</span></span>|<span data-ttu-id="52d61-120">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="52d61-120">Min OS version supported</span></span>|
|<span data-ttu-id="52d61-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="52d61-121">osMaximumVersion</span></span>|<span data-ttu-id="52d61-122">String</span><span class="sxs-lookup"><span data-stu-id="52d61-122">String</span></span>|<span data-ttu-id="52d61-123">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="52d61-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d61-124">关系</span><span class="sxs-lookup"><span data-stu-id="52d61-124">Relationships</span></span>
<span data-ttu-id="52d61-125">无</span><span class="sxs-lookup"><span data-stu-id="52d61-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52d61-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52d61-126">JSON Representation</span></span>
<span data-ttu-id="52d61-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52d61-127">Here is a JSON representation of the resource.</span></span>
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





