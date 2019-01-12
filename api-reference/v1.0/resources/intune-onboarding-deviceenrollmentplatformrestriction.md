---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7879b7f6585908aa760c3169e950cc5257bf49a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929065"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4b798-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b798-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4b798-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4b798-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b798-105">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="4b798-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="4b798-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b798-106">Properties</span></span>
|<span data-ttu-id="4b798-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b798-107">Property</span></span>|<span data-ttu-id="4b798-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b798-108">Type</span></span>|<span data-ttu-id="4b798-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b798-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b798-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4b798-110">platformBlocked</span></span>|<span data-ttu-id="4b798-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b798-111">Boolean</span></span>|<span data-ttu-id="4b798-112">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="4b798-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4b798-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4b798-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4b798-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b798-114">Boolean</span></span>|<span data-ttu-id="4b798-115">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="4b798-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4b798-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4b798-116">osMinimumVersion</span></span>|<span data-ttu-id="4b798-117">String</span><span class="sxs-lookup"><span data-stu-id="4b798-117">String</span></span>|<span data-ttu-id="4b798-118">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="4b798-118">Min OS version supported</span></span>|
|<span data-ttu-id="4b798-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4b798-119">osMaximumVersion</span></span>|<span data-ttu-id="4b798-120">String</span><span class="sxs-lookup"><span data-stu-id="4b798-120">String</span></span>|<span data-ttu-id="4b798-121">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="4b798-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b798-122">关系</span><span class="sxs-lookup"><span data-stu-id="4b798-122">Relationships</span></span>
<span data-ttu-id="4b798-123">无</span><span class="sxs-lookup"><span data-stu-id="4b798-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b798-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b798-124">JSON Representation</span></span>
<span data-ttu-id="4b798-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b798-125">Here is a JSON representation of the resource.</span></span>
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



