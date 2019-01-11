---
title: hourlySchedule 资源类型
description: 每小时运行计划的定期设备管理脚本。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f22cc44fdd9017ef6db6f014e4a9b756d46d034
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811289"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="5af10-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="5af10-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="5af10-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5af10-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af10-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5af10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af10-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5af10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af10-107">每小时运行计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="5af10-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="5af10-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="5af10-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5af10-109">属性</span><span class="sxs-lookup"><span data-stu-id="5af10-109">Properties</span></span>
|<span data-ttu-id="5af10-110">属性</span><span class="sxs-lookup"><span data-stu-id="5af10-110">Property</span></span>|<span data-ttu-id="5af10-111">类型</span><span class="sxs-lookup"><span data-stu-id="5af10-111">Type</span></span>|<span data-ttu-id="5af10-112">Description</span><span class="sxs-lookup"><span data-stu-id="5af10-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af10-113">interval</span><span class="sxs-lookup"><span data-stu-id="5af10-113">interval</span></span>|<span data-ttu-id="5af10-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5af10-114">Int32</span></span>|<span data-ttu-id="5af10-115">间隔中的小时数</span><span class="sxs-lookup"><span data-stu-id="5af10-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="5af10-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="5af10-116">Relationships</span></span>
<span data-ttu-id="5af10-117">无</span><span class="sxs-lookup"><span data-stu-id="5af10-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5af10-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5af10-118">JSON Representation</span></span>
<span data-ttu-id="5af10-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5af10-119">Here is a JSON representation of the resource.</span></span>
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





