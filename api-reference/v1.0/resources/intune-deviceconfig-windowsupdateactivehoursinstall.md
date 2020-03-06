---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d66aae6ed12abe546b5a7776e864015e20896ee7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530337"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="acc6e-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="acc6e-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="acc6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acc6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acc6e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acc6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acc6e-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="acc6e-106">Not yet documented</span></span>


<span data-ttu-id="acc6e-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="acc6e-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="acc6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="acc6e-108">Properties</span></span>
|<span data-ttu-id="acc6e-109">属性</span><span class="sxs-lookup"><span data-stu-id="acc6e-109">Property</span></span>|<span data-ttu-id="acc6e-110">类型</span><span class="sxs-lookup"><span data-stu-id="acc6e-110">Type</span></span>|<span data-ttu-id="acc6e-111">说明</span><span class="sxs-lookup"><span data-stu-id="acc6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc6e-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="acc6e-112">activeHoursStart</span></span>|<span data-ttu-id="acc6e-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="acc6e-113">TimeOfDay</span></span>|<span data-ttu-id="acc6e-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="acc6e-114">Active Hours Start</span></span>|
|<span data-ttu-id="acc6e-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="acc6e-115">activeHoursEnd</span></span>|<span data-ttu-id="acc6e-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="acc6e-116">TimeOfDay</span></span>|<span data-ttu-id="acc6e-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="acc6e-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="acc6e-118">关系</span><span class="sxs-lookup"><span data-stu-id="acc6e-118">Relationships</span></span>
<span data-ttu-id="acc6e-119">无</span><span class="sxs-lookup"><span data-stu-id="acc6e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acc6e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acc6e-120">JSON Representation</span></span>
<span data-ttu-id="acc6e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acc6e-121">Here is a JSON representation of the resource.</span></span>
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




