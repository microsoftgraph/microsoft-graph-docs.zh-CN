---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad931dc531cea8212309abca74e4dae6b6105cdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074991"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="c32d1-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c32d1-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="c32d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c32d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c32d1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c32d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c32d1-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c32d1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c32d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="c32d1-107">Properties</span></span>
|<span data-ttu-id="c32d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="c32d1-108">Property</span></span>|<span data-ttu-id="c32d1-109">类型</span><span class="sxs-lookup"><span data-stu-id="c32d1-109">Type</span></span>|<span data-ttu-id="c32d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="c32d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c32d1-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="c32d1-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="c32d1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c32d1-112">Int32</span></span>|<span data-ttu-id="c32d1-113">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="c32d1-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="c32d1-114">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="c32d1-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="c32d1-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="c32d1-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="c32d1-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c32d1-116">Boolean</span></span>|<span data-ttu-id="c32d1-117">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="c32d1-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="c32d1-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="c32d1-118">secureByDefault</span></span>|<span data-ttu-id="c32d1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c32d1-119">Boolean</span></span>|<span data-ttu-id="c32d1-120">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="c32d1-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="c32d1-121">关系</span><span class="sxs-lookup"><span data-stu-id="c32d1-121">Relationships</span></span>
<span data-ttu-id="c32d1-122">无</span><span class="sxs-lookup"><span data-stu-id="c32d1-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c32d1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c32d1-123">JSON Representation</span></span>
<span data-ttu-id="c32d1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c32d1-124">Here is a JSON representation of the resource.</span></span>
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
  "secureByDefault": true
}
```









