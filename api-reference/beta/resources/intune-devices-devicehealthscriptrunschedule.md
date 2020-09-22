---
title: deviceHealthScriptRunSchedule 资源类型
description: 设备运行状况脚本运行计划的基本类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b38c4fcafd6855dedd819ed61a2cc0b6276939d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060263"
---
# <a name="devicehealthscriptrunschedule-resource-type"></a><span data-ttu-id="421fd-103">deviceHealthScriptRunSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="421fd-103">deviceHealthScriptRunSchedule resource type</span></span>

<span data-ttu-id="421fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="421fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="421fd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="421fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="421fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421fd-107">设备运行状况脚本运行计划的基本类型。</span><span class="sxs-lookup"><span data-stu-id="421fd-107">Base type of Device health script run schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="421fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="421fd-108">Properties</span></span>
|<span data-ttu-id="421fd-109">属性</span><span class="sxs-lookup"><span data-stu-id="421fd-109">Property</span></span>|<span data-ttu-id="421fd-110">类型</span><span class="sxs-lookup"><span data-stu-id="421fd-110">Type</span></span>|<span data-ttu-id="421fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="421fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421fd-112">interval</span><span class="sxs-lookup"><span data-stu-id="421fd-112">interval</span></span>|<span data-ttu-id="421fd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="421fd-113">Int32</span></span>|<span data-ttu-id="421fd-114">每小时计划的 x 值，每隔 x 小时在每日计划的每 x 小时，每周计划的 x 周，每个 x 个月的日程安排。</span><span class="sxs-lookup"><span data-stu-id="421fd-114">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="421fd-115">有效值为1至23</span><span class="sxs-lookup"><span data-stu-id="421fd-115">Valid values 1 to 23</span></span>|

## <a name="relationships"></a><span data-ttu-id="421fd-116">关系</span><span class="sxs-lookup"><span data-stu-id="421fd-116">Relationships</span></span>
<span data-ttu-id="421fd-117">无</span><span class="sxs-lookup"><span data-stu-id="421fd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="421fd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="421fd-118">JSON Representation</span></span>
<span data-ttu-id="421fd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="421fd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": 1024
}
```






