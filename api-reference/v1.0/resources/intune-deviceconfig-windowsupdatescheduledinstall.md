---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f291fbb34f5fa412fb6da172dd196c766a7327a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091395"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="392e0-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="392e0-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="392e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="392e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="392e0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="392e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="392e0-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="392e0-106">Not yet documented</span></span>


<span data-ttu-id="392e0-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="392e0-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="392e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="392e0-108">Properties</span></span>
|<span data-ttu-id="392e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="392e0-109">Property</span></span>|<span data-ttu-id="392e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="392e0-110">Type</span></span>|<span data-ttu-id="392e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="392e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="392e0-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="392e0-112">scheduledInstallDay</span></span>|[<span data-ttu-id="392e0-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="392e0-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="392e0-114">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="392e0-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="392e0-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="392e0-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="392e0-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="392e0-116">scheduledInstallTime</span></span>|<span data-ttu-id="392e0-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="392e0-117">TimeOfDay</span></span>|<span data-ttu-id="392e0-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="392e0-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="392e0-119">关系</span><span class="sxs-lookup"><span data-stu-id="392e0-119">Relationships</span></span>
<span data-ttu-id="392e0-120">无</span><span class="sxs-lookup"><span data-stu-id="392e0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="392e0-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="392e0-121">JSON Representation</span></span>
<span data-ttu-id="392e0-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="392e0-122">Here is a JSON representation of the resource.</span></span>
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









