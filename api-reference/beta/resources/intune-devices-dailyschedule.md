---
title: dailySchedule 资源类型
description: 定期设备管理脚本的每日运行计划。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd2b226255f433b4f82d042b6389830143515033
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788070"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="ede01-103">dailySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="ede01-103">dailySchedule resource type</span></span>

> <span data-ttu-id="ede01-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ede01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ede01-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ede01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede01-106">定期设备管理脚本的每日运行计划。</span><span class="sxs-lookup"><span data-stu-id="ede01-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="ede01-107">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="ede01-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ede01-108">属性</span><span class="sxs-lookup"><span data-stu-id="ede01-108">Properties</span></span>
|<span data-ttu-id="ede01-109">属性</span><span class="sxs-lookup"><span data-stu-id="ede01-109">Property</span></span>|<span data-ttu-id="ede01-110">类型</span><span class="sxs-lookup"><span data-stu-id="ede01-110">Type</span></span>|<span data-ttu-id="ede01-111">说明</span><span class="sxs-lookup"><span data-stu-id="ede01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede01-112">interval</span><span class="sxs-lookup"><span data-stu-id="ede01-112">interval</span></span>|<span data-ttu-id="ede01-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ede01-113">Int32</span></span>|<span data-ttu-id="ede01-114">以天为单位的时间间隔</span><span class="sxs-lookup"><span data-stu-id="ede01-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="ede01-115">关系</span><span class="sxs-lookup"><span data-stu-id="ede01-115">Relationships</span></span>
<span data-ttu-id="ede01-116">无</span><span class="sxs-lookup"><span data-stu-id="ede01-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ede01-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ede01-117">JSON Representation</span></span>
<span data-ttu-id="ede01-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ede01-118">Here is a JSON representation of the resource.</span></span>
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





