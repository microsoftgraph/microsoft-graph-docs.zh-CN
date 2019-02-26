---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264055"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d9fa6-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9fa6-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="d9fa6-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9fa6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9fa6-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9fa6-105">Not yet documented</span></span>


<span data-ttu-id="d9fa6-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d9fa6-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9fa6-107">属性</span><span class="sxs-lookup"><span data-stu-id="d9fa6-107">Properties</span></span>
|<span data-ttu-id="d9fa6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9fa6-108">Property</span></span>|<span data-ttu-id="d9fa6-109">类型</span><span class="sxs-lookup"><span data-stu-id="d9fa6-109">Type</span></span>|<span data-ttu-id="d9fa6-110">说明</span><span class="sxs-lookup"><span data-stu-id="d9fa6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9fa6-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d9fa6-111">activeHoursStart</span></span>|<span data-ttu-id="d9fa6-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d9fa6-112">TimeOfDay</span></span>|<span data-ttu-id="d9fa6-113">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="d9fa6-113">Active Hours Start</span></span>|
|<span data-ttu-id="d9fa6-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d9fa6-114">activeHoursEnd</span></span>|<span data-ttu-id="d9fa6-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d9fa6-115">TimeOfDay</span></span>|<span data-ttu-id="d9fa6-116">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="d9fa6-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9fa6-117">关系</span><span class="sxs-lookup"><span data-stu-id="d9fa6-117">Relationships</span></span>
<span data-ttu-id="d9fa6-118">无</span><span class="sxs-lookup"><span data-stu-id="d9fa6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9fa6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9fa6-119">JSON Representation</span></span>
<span data-ttu-id="d9fa6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9fa6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



