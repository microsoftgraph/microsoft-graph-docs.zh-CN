---
title: dailySchedule 资源类型
description: 运行的每日计划的定期设备管理脚本。
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047143"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="3fae2-103">dailySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3fae2-103">dailySchedule resource type</span></span>

> <span data-ttu-id="3fae2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3fae2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fae2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3fae2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fae2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3fae2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fae2-107">运行的每日计划的定期设备管理脚本。</span><span class="sxs-lookup"><span data-stu-id="3fae2-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="3fae2-108">继承自[runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="3fae2-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3fae2-109">属性</span><span class="sxs-lookup"><span data-stu-id="3fae2-109">Properties</span></span>
|<span data-ttu-id="3fae2-110">属性</span><span class="sxs-lookup"><span data-stu-id="3fae2-110">Property</span></span>|<span data-ttu-id="3fae2-111">类型</span><span class="sxs-lookup"><span data-stu-id="3fae2-111">Type</span></span>|<span data-ttu-id="3fae2-112">说明</span><span class="sxs-lookup"><span data-stu-id="3fae2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fae2-113">interval</span><span class="sxs-lookup"><span data-stu-id="3fae2-113">interval</span></span>|<span data-ttu-id="3fae2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3fae2-114">Int32</span></span>|<span data-ttu-id="3fae2-115">间隔的天数</span><span class="sxs-lookup"><span data-stu-id="3fae2-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fae2-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="3fae2-116">Relationships</span></span>
<span data-ttu-id="3fae2-117">无</span><span class="sxs-lookup"><span data-stu-id="3fae2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3fae2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3fae2-118">JSON Representation</span></span>
<span data-ttu-id="3fae2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fae2-119">Here is a JSON representation of the resource.</span></span>
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





