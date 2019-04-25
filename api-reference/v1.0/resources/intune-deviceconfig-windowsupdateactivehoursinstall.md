---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573457"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="fc81b-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc81b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="fc81b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc81b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc81b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fc81b-105">Not yet documented</span></span>


<span data-ttu-id="fc81b-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="fc81b-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc81b-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc81b-107">Properties</span></span>
|<span data-ttu-id="fc81b-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc81b-108">Property</span></span>|<span data-ttu-id="fc81b-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc81b-109">Type</span></span>|<span data-ttu-id="fc81b-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc81b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc81b-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="fc81b-111">activeHoursStart</span></span>|<span data-ttu-id="fc81b-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fc81b-112">TimeOfDay</span></span>|<span data-ttu-id="fc81b-113">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="fc81b-113">Active Hours Start</span></span>|
|<span data-ttu-id="fc81b-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="fc81b-114">activeHoursEnd</span></span>|<span data-ttu-id="fc81b-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fc81b-115">TimeOfDay</span></span>|<span data-ttu-id="fc81b-116">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="fc81b-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc81b-117">关系</span><span class="sxs-lookup"><span data-stu-id="fc81b-117">Relationships</span></span>
<span data-ttu-id="fc81b-118">无</span><span class="sxs-lookup"><span data-stu-id="fc81b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc81b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc81b-119">JSON Representation</span></span>
<span data-ttu-id="fc81b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc81b-120">Here is a JSON representation of the resource.</span></span>
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



