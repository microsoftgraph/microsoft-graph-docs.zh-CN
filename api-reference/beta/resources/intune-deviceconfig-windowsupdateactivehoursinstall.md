---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28f40501123f465d8fcbfa05c3febb8ffab6f27a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409466"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="533cd-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="533cd-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="533cd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="533cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="533cd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="533cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="533cd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="533cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="533cd-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="533cd-107">Not yet documented</span></span>


<span data-ttu-id="533cd-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="533cd-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="533cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="533cd-109">Properties</span></span>
|<span data-ttu-id="533cd-110">属性</span><span class="sxs-lookup"><span data-stu-id="533cd-110">Property</span></span>|<span data-ttu-id="533cd-111">类型</span><span class="sxs-lookup"><span data-stu-id="533cd-111">Type</span></span>|<span data-ttu-id="533cd-112">说明</span><span class="sxs-lookup"><span data-stu-id="533cd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="533cd-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="533cd-113">activeHoursStart</span></span>|<span data-ttu-id="533cd-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="533cd-114">TimeOfDay</span></span>|<span data-ttu-id="533cd-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="533cd-115">Active Hours Start</span></span>|
|<span data-ttu-id="533cd-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="533cd-116">activeHoursEnd</span></span>|<span data-ttu-id="533cd-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="533cd-117">TimeOfDay</span></span>|<span data-ttu-id="533cd-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="533cd-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="533cd-119">关系</span><span class="sxs-lookup"><span data-stu-id="533cd-119">Relationships</span></span>
<span data-ttu-id="533cd-120">无</span><span class="sxs-lookup"><span data-stu-id="533cd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="533cd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="533cd-121">JSON Representation</span></span>
<span data-ttu-id="533cd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="533cd-122">Here is a JSON representation of the resource.</span></span>
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




