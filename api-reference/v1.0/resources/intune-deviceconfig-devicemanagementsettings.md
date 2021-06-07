---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17856c01f006206298e1efa1ed01fdcac6045557
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755096"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="d21c6-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d21c6-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="d21c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d21c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d21c6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d21c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d21c6-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d21c6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d21c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="d21c6-107">Properties</span></span>
|<span data-ttu-id="d21c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d21c6-108">Property</span></span>|<span data-ttu-id="d21c6-109">类型</span><span class="sxs-lookup"><span data-stu-id="d21c6-109">Type</span></span>|<span data-ttu-id="d21c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="d21c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d21c6-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d21c6-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="d21c6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d21c6-112">Int32</span></span>|<span data-ttu-id="d21c6-113">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="d21c6-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="d21c6-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="d21c6-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="d21c6-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d21c6-115">Boolean</span></span>|<span data-ttu-id="d21c6-116">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="d21c6-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="d21c6-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="d21c6-117">secureByDefault</span></span>|<span data-ttu-id="d21c6-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d21c6-118">Boolean</span></span>|<span data-ttu-id="d21c6-119">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="d21c6-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="d21c6-120">关系</span><span class="sxs-lookup"><span data-stu-id="d21c6-120">Relationships</span></span>
<span data-ttu-id="d21c6-121">无</span><span class="sxs-lookup"><span data-stu-id="d21c6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d21c6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d21c6-122">JSON Representation</span></span>
<span data-ttu-id="d21c6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d21c6-123">Here is a JSON representation of the resource.</span></span>
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




