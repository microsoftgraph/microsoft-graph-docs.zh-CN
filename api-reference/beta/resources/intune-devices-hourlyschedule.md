---
title: hourlySchedule 资源类型
description: 定期设备管理脚本的每小时运行计划。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb3eacf4e17ed1137ce78d21112c394a45423c6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173414"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="cdd33-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdd33-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="cdd33-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdd33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdd33-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdd33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdd33-106">定期设备管理脚本的每小时运行计划。</span><span class="sxs-lookup"><span data-stu-id="cdd33-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="cdd33-107">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="cdd33-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdd33-108">属性</span><span class="sxs-lookup"><span data-stu-id="cdd33-108">Properties</span></span>
|<span data-ttu-id="cdd33-109">属性</span><span class="sxs-lookup"><span data-stu-id="cdd33-109">Property</span></span>|<span data-ttu-id="cdd33-110">类型</span><span class="sxs-lookup"><span data-stu-id="cdd33-110">Type</span></span>|<span data-ttu-id="cdd33-111">说明</span><span class="sxs-lookup"><span data-stu-id="cdd33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdd33-112">interval</span><span class="sxs-lookup"><span data-stu-id="cdd33-112">interval</span></span>|<span data-ttu-id="cdd33-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cdd33-113">Int32</span></span>|<span data-ttu-id="cdd33-114">时间间隔 (小时数)</span><span class="sxs-lookup"><span data-stu-id="cdd33-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdd33-115">关系</span><span class="sxs-lookup"><span data-stu-id="cdd33-115">Relationships</span></span>
<span data-ttu-id="cdd33-116">无</span><span class="sxs-lookup"><span data-stu-id="cdd33-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdd33-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdd33-117">JSON Representation</span></span>
<span data-ttu-id="cdd33-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdd33-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




