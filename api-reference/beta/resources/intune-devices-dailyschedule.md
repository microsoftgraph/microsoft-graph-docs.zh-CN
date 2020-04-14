---
title: dailySchedule 资源类型
description: 定期设备管理脚本的每日运行计划。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b921b13fd87d3a500ca543ca6601a9ad368456ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464998"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="c563c-103">dailySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c563c-103">dailySchedule resource type</span></span>

<span data-ttu-id="c563c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c563c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c563c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c563c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c563c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c563c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c563c-107">定期设备管理脚本的每日运行计划。</span><span class="sxs-lookup"><span data-stu-id="c563c-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="c563c-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c563c-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c563c-109">属性</span><span class="sxs-lookup"><span data-stu-id="c563c-109">Properties</span></span>
|<span data-ttu-id="c563c-110">属性</span><span class="sxs-lookup"><span data-stu-id="c563c-110">Property</span></span>|<span data-ttu-id="c563c-111">类型</span><span class="sxs-lookup"><span data-stu-id="c563c-111">Type</span></span>|<span data-ttu-id="c563c-112">说明</span><span class="sxs-lookup"><span data-stu-id="c563c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c563c-113">interval</span><span class="sxs-lookup"><span data-stu-id="c563c-113">interval</span></span>|<span data-ttu-id="c563c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c563c-114">Int32</span></span>|<span data-ttu-id="c563c-115">以天为单位的时间间隔</span><span class="sxs-lookup"><span data-stu-id="c563c-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="c563c-116">关系</span><span class="sxs-lookup"><span data-stu-id="c563c-116">Relationships</span></span>
<span data-ttu-id="c563c-117">无</span><span class="sxs-lookup"><span data-stu-id="c563c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c563c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c563c-118">JSON Representation</span></span>
<span data-ttu-id="c563c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c563c-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```



