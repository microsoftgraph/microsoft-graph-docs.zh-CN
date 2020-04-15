---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 124ac24616ee8662bd0224fd2a063e523dfdb260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451397"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="d6bff-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6bff-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="d6bff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6bff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6bff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6bff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bff-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d6bff-106">Not yet documented</span></span>


<span data-ttu-id="d6bff-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d6bff-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6bff-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6bff-108">Properties</span></span>
|<span data-ttu-id="d6bff-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6bff-109">Property</span></span>|<span data-ttu-id="d6bff-110">类型</span><span class="sxs-lookup"><span data-stu-id="d6bff-110">Type</span></span>|<span data-ttu-id="d6bff-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6bff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bff-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="d6bff-112">activeHoursStart</span></span>|<span data-ttu-id="d6bff-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d6bff-113">TimeOfDay</span></span>|<span data-ttu-id="d6bff-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="d6bff-114">Active Hours Start</span></span>|
|<span data-ttu-id="d6bff-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="d6bff-115">activeHoursEnd</span></span>|<span data-ttu-id="d6bff-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d6bff-116">TimeOfDay</span></span>|<span data-ttu-id="d6bff-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="d6bff-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6bff-118">关系</span><span class="sxs-lookup"><span data-stu-id="d6bff-118">Relationships</span></span>
<span data-ttu-id="d6bff-119">无</span><span class="sxs-lookup"><span data-stu-id="d6bff-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6bff-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6bff-120">JSON Representation</span></span>
<span data-ttu-id="d6bff-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6bff-121">Here is a JSON representation of the resource.</span></span>
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







