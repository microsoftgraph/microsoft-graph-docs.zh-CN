---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0af2edc973e18c6afde50d1fdc5d93c5db196bf3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978694"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c44cf-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c44cf-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c44cf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c44cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c44cf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c44cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c44cf-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c44cf-106">Not yet documented</span></span>


<span data-ttu-id="c44cf-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c44cf-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c44cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="c44cf-108">Properties</span></span>
|<span data-ttu-id="c44cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="c44cf-109">Property</span></span>|<span data-ttu-id="c44cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="c44cf-110">Type</span></span>|<span data-ttu-id="c44cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="c44cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c44cf-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c44cf-112">scheduledInstallDay</span></span>|[<span data-ttu-id="c44cf-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c44cf-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="c44cf-114">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="c44cf-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="c44cf-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c44cf-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c44cf-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c44cf-116">scheduledInstallTime</span></span>|<span data-ttu-id="c44cf-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c44cf-117">TimeOfDay</span></span>|<span data-ttu-id="c44cf-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c44cf-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c44cf-119">关系</span><span class="sxs-lookup"><span data-stu-id="c44cf-119">Relationships</span></span>
<span data-ttu-id="c44cf-120">无</span><span class="sxs-lookup"><span data-stu-id="c44cf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c44cf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c44cf-121">JSON Representation</span></span>
<span data-ttu-id="c44cf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c44cf-122">Here is a JSON representation of the resource.</span></span>
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





