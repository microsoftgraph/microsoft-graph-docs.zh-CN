---
title: deviceEnrollmentPlatformRestriction 资源类型
description: 平台特定注册限制
ms.openlocfilehash: 823eecc37dc8ee4536d5cb63213f2bb80ca5138d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047605"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="bb059-103">deviceEnrollmentPlatformRestriction 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb059-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="bb059-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bb059-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb059-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb059-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bb059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb059-107">平台特定注册限制</span><span class="sxs-lookup"><span data-stu-id="bb059-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="bb059-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb059-108">Properties</span></span>
|<span data-ttu-id="bb059-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb059-109">Property</span></span>|<span data-ttu-id="bb059-110">类型</span><span class="sxs-lookup"><span data-stu-id="bb059-110">Type</span></span>|<span data-ttu-id="bb059-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb059-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb059-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="bb059-112">platformBlocked</span></span>|<span data-ttu-id="bb059-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb059-113">Boolean</span></span>|<span data-ttu-id="bb059-114">阻止平台注册</span><span class="sxs-lookup"><span data-stu-id="bb059-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="bb059-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="bb059-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="bb059-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb059-116">Boolean</span></span>|<span data-ttu-id="bb059-117">阻止个人拥有的设备注册</span><span class="sxs-lookup"><span data-stu-id="bb059-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="bb059-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bb059-118">osMinimumVersion</span></span>|<span data-ttu-id="bb059-119">String</span><span class="sxs-lookup"><span data-stu-id="bb059-119">String</span></span>|<span data-ttu-id="bb059-120">支持的最小 OS 版本</span><span class="sxs-lookup"><span data-stu-id="bb059-120">Min OS version supported</span></span>|
|<span data-ttu-id="bb059-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bb059-121">osMaximumVersion</span></span>|<span data-ttu-id="bb059-122">String</span><span class="sxs-lookup"><span data-stu-id="bb059-122">String</span></span>|<span data-ttu-id="bb059-123">支持的最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="bb059-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb059-124">关系</span><span class="sxs-lookup"><span data-stu-id="bb059-124">Relationships</span></span>
<span data-ttu-id="bb059-125">无</span><span class="sxs-lookup"><span data-stu-id="bb059-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb059-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb059-126">JSON Representation</span></span>
<span data-ttu-id="bb059-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb059-127">Here is a JSON representation of the resource.</span></span>
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





