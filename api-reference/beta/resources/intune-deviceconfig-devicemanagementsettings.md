---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f973f2645b37375641bc536b5ace0fa508fb0b0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854416"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="97e17-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="97e17-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="97e17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97e17-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97e17-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97e17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97e17-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97e17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97e17-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97e17-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="97e17-108">属性</span><span class="sxs-lookup"><span data-stu-id="97e17-108">Properties</span></span>
|<span data-ttu-id="97e17-109">属性</span><span class="sxs-lookup"><span data-stu-id="97e17-109">Property</span></span>|<span data-ttu-id="97e17-110">类型</span><span class="sxs-lookup"><span data-stu-id="97e17-110">Type</span></span>|<span data-ttu-id="97e17-111">说明</span><span class="sxs-lookup"><span data-stu-id="97e17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e17-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="97e17-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="97e17-113">Int32</span><span class="sxs-lookup"><span data-stu-id="97e17-113">Int32</span></span>|<span data-ttu-id="97e17-114">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="97e17-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="97e17-115">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="97e17-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="97e17-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="97e17-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="97e17-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="97e17-117">Boolean</span></span>|<span data-ttu-id="97e17-118">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="97e17-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="97e17-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="97e17-119">secureByDefault</span></span>|<span data-ttu-id="97e17-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="97e17-120">Boolean</span></span>|<span data-ttu-id="97e17-121">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="97e17-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="97e17-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="97e17-122">enhancedJailBreak</span></span>|<span data-ttu-id="97e17-123">布尔</span><span class="sxs-lookup"><span data-stu-id="97e17-123">Boolean</span></span>|<span data-ttu-id="97e17-124">功能启用或非增强 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="97e17-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="97e17-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="97e17-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="97e17-126">Int32</span><span class="sxs-lookup"><span data-stu-id="97e17-126">Int32</span></span>|<span data-ttu-id="97e17-127">当设备不检查指定天数，公司数据可能会删除，设备将不会在管理下。</span><span class="sxs-lookup"><span data-stu-id="97e17-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="97e17-128">有效值 30 到 270</span><span class="sxs-lookup"><span data-stu-id="97e17-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="97e17-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="97e17-129">Relationships</span></span>
<span data-ttu-id="97e17-130">无</span><span class="sxs-lookup"><span data-stu-id="97e17-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97e17-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97e17-131">JSON Representation</span></span>
<span data-ttu-id="97e17-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97e17-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





