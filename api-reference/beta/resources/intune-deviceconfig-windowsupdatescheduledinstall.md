---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93866da8e1dff5b53303dfd6cbd358fc0280ee30
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337683"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="e9db3-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9db3-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="e9db3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9db3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9db3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9db3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9db3-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9db3-106">Not yet documented</span></span>


<span data-ttu-id="e9db3-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="e9db3-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9db3-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9db3-108">Properties</span></span>
|<span data-ttu-id="e9db3-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9db3-109">Property</span></span>|<span data-ttu-id="e9db3-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9db3-110">Type</span></span>|<span data-ttu-id="e9db3-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9db3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9db3-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="e9db3-112">scheduledInstallDay</span></span>|[<span data-ttu-id="e9db3-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="e9db3-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="e9db3-114">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="e9db3-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="e9db3-115">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="e9db3-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="e9db3-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="e9db3-116">scheduledInstallTime</span></span>|<span data-ttu-id="e9db3-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e9db3-117">TimeOfDay</span></span>|<span data-ttu-id="e9db3-118">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="e9db3-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9db3-119">关系</span><span class="sxs-lookup"><span data-stu-id="e9db3-119">Relationships</span></span>
<span data-ttu-id="e9db3-120">无</span><span class="sxs-lookup"><span data-stu-id="e9db3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9db3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9db3-121">JSON Representation</span></span>
<span data-ttu-id="e9db3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9db3-122">Here is a JSON representation of the resource.</span></span>
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



