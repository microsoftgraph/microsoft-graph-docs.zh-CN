---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de36e3777518cf7c79a7590c19147d014e2aee7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172504"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="8b9dc-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b9dc-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="8b9dc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b9dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b9dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b9dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b9dc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8b9dc-106">Not yet documented</span></span>


<span data-ttu-id="8b9dc-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8b9dc-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8b9dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b9dc-108">Properties</span></span>
|<span data-ttu-id="8b9dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="8b9dc-109">Property</span></span>|<span data-ttu-id="8b9dc-110">类型</span><span class="sxs-lookup"><span data-stu-id="8b9dc-110">Type</span></span>|<span data-ttu-id="8b9dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b9dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b9dc-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="8b9dc-112">scheduledInstallDay</span></span>|[<span data-ttu-id="8b9dc-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8b9dc-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="8b9dc-114">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="8b9dc-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="8b9dc-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="8b9dc-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8b9dc-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="8b9dc-116">scheduledInstallTime</span></span>|<span data-ttu-id="8b9dc-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8b9dc-117">TimeOfDay</span></span>|<span data-ttu-id="8b9dc-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="8b9dc-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b9dc-119">关系</span><span class="sxs-lookup"><span data-stu-id="8b9dc-119">Relationships</span></span>
<span data-ttu-id="8b9dc-120">无</span><span class="sxs-lookup"><span data-stu-id="8b9dc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b9dc-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b9dc-121">JSON Representation</span></span>
<span data-ttu-id="8b9dc-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b9dc-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```




