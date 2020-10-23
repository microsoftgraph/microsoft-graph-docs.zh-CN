---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67c6ec798df120f9c7c14fbf2392450d05bb8afb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695010"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="4757f-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="4757f-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="4757f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4757f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4757f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4757f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4757f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4757f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4757f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4757f-107">Not yet documented</span></span>


<span data-ttu-id="4757f-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4757f-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4757f-109">属性</span><span class="sxs-lookup"><span data-stu-id="4757f-109">Properties</span></span>
|<span data-ttu-id="4757f-110">属性</span><span class="sxs-lookup"><span data-stu-id="4757f-110">Property</span></span>|<span data-ttu-id="4757f-111">类型</span><span class="sxs-lookup"><span data-stu-id="4757f-111">Type</span></span>|<span data-ttu-id="4757f-112">说明</span><span class="sxs-lookup"><span data-stu-id="4757f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4757f-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="4757f-113">activeHoursStart</span></span>|<span data-ttu-id="4757f-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4757f-114">TimeOfDay</span></span>|<span data-ttu-id="4757f-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="4757f-115">Active Hours Start</span></span>|
|<span data-ttu-id="4757f-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="4757f-116">activeHoursEnd</span></span>|<span data-ttu-id="4757f-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4757f-117">TimeOfDay</span></span>|<span data-ttu-id="4757f-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="4757f-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="4757f-119">关系</span><span class="sxs-lookup"><span data-stu-id="4757f-119">Relationships</span></span>
<span data-ttu-id="4757f-120">无</span><span class="sxs-lookup"><span data-stu-id="4757f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4757f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4757f-121">JSON Representation</span></span>
<span data-ttu-id="4757f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4757f-122">Here is a JSON representation of the resource.</span></span>
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





