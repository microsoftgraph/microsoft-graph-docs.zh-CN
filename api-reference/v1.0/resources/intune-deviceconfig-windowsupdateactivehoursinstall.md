---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 81ccc29bfe0eb9c3d0d943975807cbf5776051a9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758762"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b3c78-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3c78-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="b3c78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3c78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3c78-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3c78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3c78-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3c78-106">Not yet documented</span></span>


<span data-ttu-id="b3c78-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b3c78-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3c78-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3c78-108">Properties</span></span>
|<span data-ttu-id="b3c78-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3c78-109">Property</span></span>|<span data-ttu-id="b3c78-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3c78-110">Type</span></span>|<span data-ttu-id="b3c78-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3c78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3c78-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b3c78-112">activeHoursStart</span></span>|<span data-ttu-id="b3c78-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b3c78-113">TimeOfDay</span></span>|<span data-ttu-id="b3c78-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="b3c78-114">Active Hours Start</span></span>|
|<span data-ttu-id="b3c78-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b3c78-115">activeHoursEnd</span></span>|<span data-ttu-id="b3c78-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b3c78-116">TimeOfDay</span></span>|<span data-ttu-id="b3c78-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="b3c78-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3c78-118">关系</span><span class="sxs-lookup"><span data-stu-id="b3c78-118">Relationships</span></span>
<span data-ttu-id="b3c78-119">无</span><span class="sxs-lookup"><span data-stu-id="b3c78-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3c78-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3c78-120">JSON Representation</span></span>
<span data-ttu-id="b3c78-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c78-121">Here is a JSON representation of the resource.</span></span>
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




