---
title: hourlySchedule 资源类型
description: 每小时运行计划的定期设备管理脚本。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396824"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="0c223-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c223-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="0c223-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0c223-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c223-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c223-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c223-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c223-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c223-107">每小时运行计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="0c223-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="0c223-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="0c223-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c223-109">属性</span><span class="sxs-lookup"><span data-stu-id="0c223-109">Properties</span></span>
|<span data-ttu-id="0c223-110">属性</span><span class="sxs-lookup"><span data-stu-id="0c223-110">Property</span></span>|<span data-ttu-id="0c223-111">类型</span><span class="sxs-lookup"><span data-stu-id="0c223-111">Type</span></span>|<span data-ttu-id="0c223-112">说明</span><span class="sxs-lookup"><span data-stu-id="0c223-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c223-113">interval</span><span class="sxs-lookup"><span data-stu-id="0c223-113">interval</span></span>|<span data-ttu-id="0c223-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0c223-114">Int32</span></span>|<span data-ttu-id="0c223-115">间隔中的小时数</span><span class="sxs-lookup"><span data-stu-id="0c223-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c223-116">关系</span><span class="sxs-lookup"><span data-stu-id="0c223-116">Relationships</span></span>
<span data-ttu-id="0c223-117">无</span><span class="sxs-lookup"><span data-stu-id="0c223-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c223-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c223-118">JSON Representation</span></span>
<span data-ttu-id="0c223-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c223-119">Here is a JSON representation of the resource.</span></span>
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




