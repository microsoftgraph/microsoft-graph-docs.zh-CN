---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd3a1aafe751bd5db334387cc3872c68e6de6637
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523634"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="1e874-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e874-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="1e874-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e874-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e874-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e874-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e874-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="1e874-106">Not yet documented</span></span>


<span data-ttu-id="1e874-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="1e874-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e874-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e874-108">Properties</span></span>
|<span data-ttu-id="1e874-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e874-109">Property</span></span>|<span data-ttu-id="1e874-110">类型</span><span class="sxs-lookup"><span data-stu-id="1e874-110">Type</span></span>|<span data-ttu-id="1e874-111">说明</span><span class="sxs-lookup"><span data-stu-id="1e874-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e874-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="1e874-112">scheduledInstallDay</span></span>|[<span data-ttu-id="1e874-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="1e874-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="1e874-114">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="1e874-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="1e874-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="1e874-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1e874-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="1e874-116">scheduledInstallTime</span></span>|<span data-ttu-id="1e874-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1e874-117">TimeOfDay</span></span>|<span data-ttu-id="1e874-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="1e874-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e874-119">关系</span><span class="sxs-lookup"><span data-stu-id="1e874-119">Relationships</span></span>
<span data-ttu-id="1e874-120">无</span><span class="sxs-lookup"><span data-stu-id="1e874-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e874-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e874-121">JSON Representation</span></span>
<span data-ttu-id="1e874-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e874-122">Here is a JSON representation of the resource.</span></span>
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





