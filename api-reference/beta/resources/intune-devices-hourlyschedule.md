---
title: hourlySchedule 资源类型
description: 定期设备管理脚本的每小时运行计划。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2eae0d244eb78e006f74c127a81df1786bc9bd8f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470611"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="ccb04-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccb04-103">hourlySchedule resource type</span></span>

<span data-ttu-id="ccb04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccb04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccb04-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ccb04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccb04-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccb04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccb04-107">定期设备管理脚本的每小时运行计划。</span><span class="sxs-lookup"><span data-stu-id="ccb04-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="ccb04-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="ccb04-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ccb04-109">属性</span><span class="sxs-lookup"><span data-stu-id="ccb04-109">Properties</span></span>
|<span data-ttu-id="ccb04-110">属性</span><span class="sxs-lookup"><span data-stu-id="ccb04-110">Property</span></span>|<span data-ttu-id="ccb04-111">类型</span><span class="sxs-lookup"><span data-stu-id="ccb04-111">Type</span></span>|<span data-ttu-id="ccb04-112">说明</span><span class="sxs-lookup"><span data-stu-id="ccb04-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb04-113">interval</span><span class="sxs-lookup"><span data-stu-id="ccb04-113">interval</span></span>|<span data-ttu-id="ccb04-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb04-114">Int32</span></span>|<span data-ttu-id="ccb04-115">时间间隔（小时数）</span><span class="sxs-lookup"><span data-stu-id="ccb04-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccb04-116">关系</span><span class="sxs-lookup"><span data-stu-id="ccb04-116">Relationships</span></span>
<span data-ttu-id="ccb04-117">无</span><span class="sxs-lookup"><span data-stu-id="ccb04-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccb04-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccb04-118">JSON Representation</span></span>
<span data-ttu-id="ccb04-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccb04-119">Here is a JSON representation of the resource.</span></span>
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



