---
title: hourlySchedule 资源类型
description: 定期设备管理脚本的每小时运行计划。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aadd9f6e53288087cea5ee75a5f7cab2b2decbde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995166"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="f308a-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f308a-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="f308a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f308a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f308a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f308a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f308a-106">定期设备管理脚本的每小时运行计划。</span><span class="sxs-lookup"><span data-stu-id="f308a-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="f308a-107">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f308a-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f308a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f308a-108">Properties</span></span>
|<span data-ttu-id="f308a-109">属性</span><span class="sxs-lookup"><span data-stu-id="f308a-109">Property</span></span>|<span data-ttu-id="f308a-110">类型</span><span class="sxs-lookup"><span data-stu-id="f308a-110">Type</span></span>|<span data-ttu-id="f308a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f308a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f308a-112">interval</span><span class="sxs-lookup"><span data-stu-id="f308a-112">interval</span></span>|<span data-ttu-id="f308a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f308a-113">Int32</span></span>|<span data-ttu-id="f308a-114">时间间隔 (小时数)</span><span class="sxs-lookup"><span data-stu-id="f308a-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="f308a-115">关系</span><span class="sxs-lookup"><span data-stu-id="f308a-115">Relationships</span></span>
<span data-ttu-id="f308a-116">无</span><span class="sxs-lookup"><span data-stu-id="f308a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f308a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f308a-117">JSON Representation</span></span>
<span data-ttu-id="f308a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f308a-118">Here is a JSON representation of the resource.</span></span>
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





