---
title: dailySchedule 资源类型
description: 运行的每日计划的定期设备管理脚本。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d0f4f258afe1de65bd8fecf32d9df387716a2c6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987711"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="6ed40-103">dailySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed40-103">dailySchedule resource type</span></span>

> <span data-ttu-id="6ed40-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ed40-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ed40-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ed40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ed40-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ed40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ed40-107">运行的每日计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="6ed40-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="6ed40-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="6ed40-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ed40-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ed40-109">Properties</span></span>
|<span data-ttu-id="6ed40-110">属性</span><span class="sxs-lookup"><span data-stu-id="6ed40-110">Property</span></span>|<span data-ttu-id="6ed40-111">类型</span><span class="sxs-lookup"><span data-stu-id="6ed40-111">Type</span></span>|<span data-ttu-id="6ed40-112">说明</span><span class="sxs-lookup"><span data-stu-id="6ed40-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ed40-113">interval</span><span class="sxs-lookup"><span data-stu-id="6ed40-113">interval</span></span>|<span data-ttu-id="6ed40-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6ed40-114">Int32</span></span>|<span data-ttu-id="6ed40-115">间隔的天数</span><span class="sxs-lookup"><span data-stu-id="6ed40-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ed40-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="6ed40-116">Relationships</span></span>
<span data-ttu-id="6ed40-117">无</span><span class="sxs-lookup"><span data-stu-id="6ed40-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ed40-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed40-118">JSON Representation</span></span>
<span data-ttu-id="6ed40-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed40-119">Here is a JSON representation of the resource.</span></span>
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





