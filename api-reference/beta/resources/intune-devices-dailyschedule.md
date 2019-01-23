---
title: dailySchedule 资源类型
description: 运行的每日计划的定期设备管理脚本。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4cbe48aecf3fe561becad4734f7de0b5f68ffa0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415248"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="f41d2-103">dailySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f41d2-103">dailySchedule resource type</span></span>

> <span data-ttu-id="f41d2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f41d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f41d2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f41d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f41d2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f41d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f41d2-107">运行的每日计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="f41d2-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="f41d2-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f41d2-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f41d2-109">属性</span><span class="sxs-lookup"><span data-stu-id="f41d2-109">Properties</span></span>
|<span data-ttu-id="f41d2-110">属性</span><span class="sxs-lookup"><span data-stu-id="f41d2-110">Property</span></span>|<span data-ttu-id="f41d2-111">类型</span><span class="sxs-lookup"><span data-stu-id="f41d2-111">Type</span></span>|<span data-ttu-id="f41d2-112">说明</span><span class="sxs-lookup"><span data-stu-id="f41d2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f41d2-113">interval</span><span class="sxs-lookup"><span data-stu-id="f41d2-113">interval</span></span>|<span data-ttu-id="f41d2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f41d2-114">Int32</span></span>|<span data-ttu-id="f41d2-115">间隔的天数</span><span class="sxs-lookup"><span data-stu-id="f41d2-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="f41d2-116">关系</span><span class="sxs-lookup"><span data-stu-id="f41d2-116">Relationships</span></span>
<span data-ttu-id="f41d2-117">无</span><span class="sxs-lookup"><span data-stu-id="f41d2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f41d2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f41d2-118">JSON Representation</span></span>
<span data-ttu-id="f41d2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f41d2-119">Here is a JSON representation of the resource.</span></span>
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




