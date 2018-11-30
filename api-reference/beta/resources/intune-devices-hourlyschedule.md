---
title: hourlySchedule 资源类型
description: 每小时运行计划的定期设备管理脚本。
ms.openlocfilehash: 1161f7dfc3d74224c22075db8eff83b7f412b9b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046299"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="1c8d6-103">hourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c8d6-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="1c8d6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c8d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c8d6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c8d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c8d6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c8d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c8d6-107">每小时运行计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="1c8d6-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="1c8d6-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="1c8d6-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c8d6-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c8d6-109">Properties</span></span>
|<span data-ttu-id="1c8d6-110">属性</span><span class="sxs-lookup"><span data-stu-id="1c8d6-110">Property</span></span>|<span data-ttu-id="1c8d6-111">类型</span><span class="sxs-lookup"><span data-stu-id="1c8d6-111">Type</span></span>|<span data-ttu-id="1c8d6-112">说明</span><span class="sxs-lookup"><span data-stu-id="1c8d6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c8d6-113">interval</span><span class="sxs-lookup"><span data-stu-id="1c8d6-113">interval</span></span>|<span data-ttu-id="1c8d6-114">Int32</span><span class="sxs-lookup"><span data-stu-id="1c8d6-114">Int32</span></span>|<span data-ttu-id="1c8d6-115">间隔中的小时数</span><span class="sxs-lookup"><span data-stu-id="1c8d6-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c8d6-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="1c8d6-116">Relationships</span></span>
<span data-ttu-id="1c8d6-117">无</span><span class="sxs-lookup"><span data-stu-id="1c8d6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c8d6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c8d6-118">JSON Representation</span></span>
<span data-ttu-id="1c8d6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c8d6-119">Here is a JSON representation of the resource.</span></span>
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





