---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca4c658c9fa9837deb56868a84ff0bddefeb6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272414"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c7bf7-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7bf7-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="c7bf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7bf7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7bf7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7bf7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7bf7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7bf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7bf7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7bf7-107">Not yet documented</span></span>


<span data-ttu-id="c7bf7-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c7bf7-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7bf7-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7bf7-109">Properties</span></span>
|<span data-ttu-id="c7bf7-110">属性</span><span class="sxs-lookup"><span data-stu-id="c7bf7-110">Property</span></span>|<span data-ttu-id="c7bf7-111">类型</span><span class="sxs-lookup"><span data-stu-id="c7bf7-111">Type</span></span>|<span data-ttu-id="c7bf7-112">说明</span><span class="sxs-lookup"><span data-stu-id="c7bf7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7bf7-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c7bf7-113">scheduledInstallDay</span></span>|[<span data-ttu-id="c7bf7-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c7bf7-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="c7bf7-115">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="c7bf7-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="c7bf7-116">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="c7bf7-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="c7bf7-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c7bf7-117">scheduledInstallTime</span></span>|<span data-ttu-id="c7bf7-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c7bf7-118">TimeOfDay</span></span>|<span data-ttu-id="c7bf7-119">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c7bf7-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7bf7-120">关系</span><span class="sxs-lookup"><span data-stu-id="c7bf7-120">Relationships</span></span>
<span data-ttu-id="c7bf7-121">无</span><span class="sxs-lookup"><span data-stu-id="c7bf7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7bf7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7bf7-122">JSON Representation</span></span>
<span data-ttu-id="c7bf7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7bf7-123">Here is a JSON representation of the resource.</span></span>
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




