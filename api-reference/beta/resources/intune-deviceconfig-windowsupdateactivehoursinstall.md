---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5e9b8f4f55f2709fe5db513e801937e05e0f38a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453424"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="906d8-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="906d8-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="906d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="906d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="906d8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="906d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="906d8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="906d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="906d8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="906d8-107">Not yet documented</span></span>


<span data-ttu-id="906d8-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="906d8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="906d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="906d8-109">Properties</span></span>
|<span data-ttu-id="906d8-110">属性</span><span class="sxs-lookup"><span data-stu-id="906d8-110">Property</span></span>|<span data-ttu-id="906d8-111">类型</span><span class="sxs-lookup"><span data-stu-id="906d8-111">Type</span></span>|<span data-ttu-id="906d8-112">说明</span><span class="sxs-lookup"><span data-stu-id="906d8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="906d8-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="906d8-113">activeHoursStart</span></span>|<span data-ttu-id="906d8-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="906d8-114">TimeOfDay</span></span>|<span data-ttu-id="906d8-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="906d8-115">Active Hours Start</span></span>|
|<span data-ttu-id="906d8-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="906d8-116">activeHoursEnd</span></span>|<span data-ttu-id="906d8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="906d8-117">TimeOfDay</span></span>|<span data-ttu-id="906d8-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="906d8-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="906d8-119">关系</span><span class="sxs-lookup"><span data-stu-id="906d8-119">Relationships</span></span>
<span data-ttu-id="906d8-120">无</span><span class="sxs-lookup"><span data-stu-id="906d8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="906d8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="906d8-121">JSON Representation</span></span>
<span data-ttu-id="906d8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="906d8-122">Here is a JSON representation of the resource.</span></span>
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



