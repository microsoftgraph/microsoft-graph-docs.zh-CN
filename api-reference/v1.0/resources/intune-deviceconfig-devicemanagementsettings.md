---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d990271b611fdb088975e155637834dc9261580
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028413"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="22703-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="22703-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="22703-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22703-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22703-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="22703-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="22703-106">属性</span><span class="sxs-lookup"><span data-stu-id="22703-106">Properties</span></span>
|<span data-ttu-id="22703-107">属性</span><span class="sxs-lookup"><span data-stu-id="22703-107">Property</span></span>|<span data-ttu-id="22703-108">类型</span><span class="sxs-lookup"><span data-stu-id="22703-108">Type</span></span>|<span data-ttu-id="22703-109">说明</span><span class="sxs-lookup"><span data-stu-id="22703-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22703-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="22703-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="22703-111">Int32</span><span class="sxs-lookup"><span data-stu-id="22703-111">Int32</span></span>|<span data-ttu-id="22703-112">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="22703-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="22703-113">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="22703-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="22703-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="22703-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="22703-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="22703-115">Boolean</span></span>|<span data-ttu-id="22703-116">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="22703-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="22703-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="22703-117">secureByDefault</span></span>|<span data-ttu-id="22703-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="22703-118">Boolean</span></span>|<span data-ttu-id="22703-119">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="22703-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="22703-120">关系</span><span class="sxs-lookup"><span data-stu-id="22703-120">Relationships</span></span>
<span data-ttu-id="22703-121">无</span><span class="sxs-lookup"><span data-stu-id="22703-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22703-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22703-122">JSON Representation</span></span>
<span data-ttu-id="22703-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22703-123">Here is a JSON representation of the resource.</span></span>
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



