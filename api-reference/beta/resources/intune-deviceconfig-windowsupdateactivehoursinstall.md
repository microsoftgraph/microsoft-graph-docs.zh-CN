---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49238831005d579baba2dd55e431f1ac684e67d3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943653"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="03d79-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="03d79-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="03d79-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03d79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03d79-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03d79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03d79-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="03d79-106">Not yet documented</span></span>


<span data-ttu-id="03d79-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="03d79-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03d79-108">属性</span><span class="sxs-lookup"><span data-stu-id="03d79-108">Properties</span></span>
|<span data-ttu-id="03d79-109">属性</span><span class="sxs-lookup"><span data-stu-id="03d79-109">Property</span></span>|<span data-ttu-id="03d79-110">类型</span><span class="sxs-lookup"><span data-stu-id="03d79-110">Type</span></span>|<span data-ttu-id="03d79-111">说明</span><span class="sxs-lookup"><span data-stu-id="03d79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d79-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="03d79-112">activeHoursStart</span></span>|<span data-ttu-id="03d79-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="03d79-113">TimeOfDay</span></span>|<span data-ttu-id="03d79-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="03d79-114">Active Hours Start</span></span>|
|<span data-ttu-id="03d79-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="03d79-115">activeHoursEnd</span></span>|<span data-ttu-id="03d79-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="03d79-116">TimeOfDay</span></span>|<span data-ttu-id="03d79-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="03d79-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="03d79-118">关系</span><span class="sxs-lookup"><span data-stu-id="03d79-118">Relationships</span></span>
<span data-ttu-id="03d79-119">无</span><span class="sxs-lookup"><span data-stu-id="03d79-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03d79-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03d79-120">JSON Representation</span></span>
<span data-ttu-id="03d79-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03d79-121">Here is a JSON representation of the resource.</span></span>
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




