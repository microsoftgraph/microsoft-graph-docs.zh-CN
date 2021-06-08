---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22c1c6e2ba205c705baabc6bc7643848f7f12686
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759950"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="ac6dc-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac6dc-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="ac6dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac6dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac6dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac6dc-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ac6dc-106">Not yet documented</span></span>


<span data-ttu-id="ac6dc-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="ac6dc-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac6dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac6dc-108">Properties</span></span>
|<span data-ttu-id="ac6dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="ac6dc-109">Property</span></span>|<span data-ttu-id="ac6dc-110">类型</span><span class="sxs-lookup"><span data-stu-id="ac6dc-110">Type</span></span>|<span data-ttu-id="ac6dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="ac6dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6dc-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="ac6dc-112">scheduledInstallDay</span></span>|[<span data-ttu-id="ac6dc-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="ac6dc-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="ac6dc-114">计划的安装日（按周）。</span><span class="sxs-lookup"><span data-stu-id="ac6dc-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="ac6dc-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="ac6dc-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ac6dc-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="ac6dc-116">scheduledInstallTime</span></span>|<span data-ttu-id="ac6dc-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ac6dc-117">TimeOfDay</span></span>|<span data-ttu-id="ac6dc-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="ac6dc-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6dc-119">关系</span><span class="sxs-lookup"><span data-stu-id="ac6dc-119">Relationships</span></span>
<span data-ttu-id="ac6dc-120">无</span><span class="sxs-lookup"><span data-stu-id="ac6dc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6dc-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac6dc-121">JSON Representation</span></span>
<span data-ttu-id="ac6dc-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac6dc-122">Here is a JSON representation of the resource.</span></span>
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




