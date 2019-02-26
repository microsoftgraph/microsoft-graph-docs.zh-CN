---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264314"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c182e-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c182e-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c182e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c182e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c182e-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c182e-105">Not yet documented</span></span>


<span data-ttu-id="c182e-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c182e-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c182e-107">属性</span><span class="sxs-lookup"><span data-stu-id="c182e-107">Properties</span></span>
|<span data-ttu-id="c182e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c182e-108">Property</span></span>|<span data-ttu-id="c182e-109">类型</span><span class="sxs-lookup"><span data-stu-id="c182e-109">Type</span></span>|<span data-ttu-id="c182e-110">说明</span><span class="sxs-lookup"><span data-stu-id="c182e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c182e-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c182e-111">scheduledInstallDay</span></span>|[<span data-ttu-id="c182e-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c182e-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="c182e-113">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="c182e-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="c182e-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c182e-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c182e-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c182e-115">scheduledInstallTime</span></span>|<span data-ttu-id="c182e-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c182e-116">TimeOfDay</span></span>|<span data-ttu-id="c182e-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c182e-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c182e-118">关系</span><span class="sxs-lookup"><span data-stu-id="c182e-118">Relationships</span></span>
<span data-ttu-id="c182e-119">无</span><span class="sxs-lookup"><span data-stu-id="c182e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c182e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c182e-120">JSON Representation</span></span>
<span data-ttu-id="c182e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c182e-121">Here is a JSON representation of the resource.</span></span>
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



