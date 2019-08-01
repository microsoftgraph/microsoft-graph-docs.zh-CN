---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b3c6d5fa7e517713d1904d33c94bcd8dccec5d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030896"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6094f-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="6094f-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="6094f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6094f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6094f-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6094f-105">Not yet documented</span></span>


<span data-ttu-id="6094f-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6094f-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6094f-107">属性</span><span class="sxs-lookup"><span data-stu-id="6094f-107">Properties</span></span>
|<span data-ttu-id="6094f-108">属性</span><span class="sxs-lookup"><span data-stu-id="6094f-108">Property</span></span>|<span data-ttu-id="6094f-109">类型</span><span class="sxs-lookup"><span data-stu-id="6094f-109">Type</span></span>|<span data-ttu-id="6094f-110">说明</span><span class="sxs-lookup"><span data-stu-id="6094f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6094f-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6094f-111">scheduledInstallDay</span></span>|[<span data-ttu-id="6094f-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="6094f-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6094f-113">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="6094f-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="6094f-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="6094f-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6094f-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6094f-115">scheduledInstallTime</span></span>|<span data-ttu-id="6094f-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6094f-116">TimeOfDay</span></span>|<span data-ttu-id="6094f-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="6094f-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6094f-118">关系</span><span class="sxs-lookup"><span data-stu-id="6094f-118">Relationships</span></span>
<span data-ttu-id="6094f-119">无</span><span class="sxs-lookup"><span data-stu-id="6094f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6094f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6094f-120">JSON Representation</span></span>
<span data-ttu-id="6094f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6094f-121">Here is a JSON representation of the resource.</span></span>
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



