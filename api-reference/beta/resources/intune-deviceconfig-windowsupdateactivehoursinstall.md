---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792718"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="8786f-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="8786f-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="8786f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8786f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8786f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8786f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8786f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8786f-106">Not yet documented</span></span>


<span data-ttu-id="8786f-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8786f-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8786f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8786f-108">Properties</span></span>
|<span data-ttu-id="8786f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8786f-109">Property</span></span>|<span data-ttu-id="8786f-110">类型</span><span class="sxs-lookup"><span data-stu-id="8786f-110">Type</span></span>|<span data-ttu-id="8786f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8786f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8786f-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="8786f-112">activeHoursStart</span></span>|<span data-ttu-id="8786f-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8786f-113">TimeOfDay</span></span>|<span data-ttu-id="8786f-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="8786f-114">Active Hours Start</span></span>|
|<span data-ttu-id="8786f-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="8786f-115">activeHoursEnd</span></span>|<span data-ttu-id="8786f-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8786f-116">TimeOfDay</span></span>|<span data-ttu-id="8786f-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="8786f-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="8786f-118">关系</span><span class="sxs-lookup"><span data-stu-id="8786f-118">Relationships</span></span>
<span data-ttu-id="8786f-119">无</span><span class="sxs-lookup"><span data-stu-id="8786f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8786f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8786f-120">JSON Representation</span></span>
<span data-ttu-id="8786f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8786f-121">Here is a JSON representation of the resource.</span></span>
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





