---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fd5958e5b8e853f07c715cd1ecf8c03a9a49a15
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357134"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="1782d-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="1782d-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="1782d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1782d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1782d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1782d-105">Not yet documented</span></span>


<span data-ttu-id="1782d-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="1782d-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1782d-107">属性</span><span class="sxs-lookup"><span data-stu-id="1782d-107">Properties</span></span>
|<span data-ttu-id="1782d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1782d-108">Property</span></span>|<span data-ttu-id="1782d-109">类型</span><span class="sxs-lookup"><span data-stu-id="1782d-109">Type</span></span>|<span data-ttu-id="1782d-110">说明</span><span class="sxs-lookup"><span data-stu-id="1782d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1782d-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="1782d-111">scheduledInstallDay</span></span>|[<span data-ttu-id="1782d-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="1782d-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="1782d-113">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="1782d-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="1782d-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="1782d-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1782d-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="1782d-115">scheduledInstallTime</span></span>|<span data-ttu-id="1782d-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1782d-116">TimeOfDay</span></span>|<span data-ttu-id="1782d-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="1782d-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="1782d-118">关系</span><span class="sxs-lookup"><span data-stu-id="1782d-118">Relationships</span></span>
<span data-ttu-id="1782d-119">无</span><span class="sxs-lookup"><span data-stu-id="1782d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1782d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1782d-120">JSON Representation</span></span>
<span data-ttu-id="1782d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1782d-121">Here is a JSON representation of the resource.</span></span>
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




