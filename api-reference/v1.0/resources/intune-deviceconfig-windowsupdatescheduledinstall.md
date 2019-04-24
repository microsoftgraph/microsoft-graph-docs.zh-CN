---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503574"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4ab57-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ab57-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4ab57-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ab57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ab57-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4ab57-105">Not yet documented</span></span>


<span data-ttu-id="4ab57-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4ab57-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ab57-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ab57-107">Properties</span></span>
|<span data-ttu-id="4ab57-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ab57-108">Property</span></span>|<span data-ttu-id="4ab57-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ab57-109">Type</span></span>|<span data-ttu-id="4ab57-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ab57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ab57-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4ab57-111">scheduledInstallDay</span></span>|[<span data-ttu-id="4ab57-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4ab57-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4ab57-113">每周的计划安装日期。</span><span class="sxs-lookup"><span data-stu-id="4ab57-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="4ab57-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="4ab57-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4ab57-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4ab57-115">scheduledInstallTime</span></span>|<span data-ttu-id="4ab57-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4ab57-116">TimeOfDay</span></span>|<span data-ttu-id="4ab57-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="4ab57-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ab57-118">关系</span><span class="sxs-lookup"><span data-stu-id="4ab57-118">Relationships</span></span>
<span data-ttu-id="4ab57-119">无</span><span class="sxs-lookup"><span data-stu-id="4ab57-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ab57-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ab57-120">JSON Representation</span></span>
<span data-ttu-id="4ab57-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ab57-121">Here is a JSON representation of the resource.</span></span>
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



