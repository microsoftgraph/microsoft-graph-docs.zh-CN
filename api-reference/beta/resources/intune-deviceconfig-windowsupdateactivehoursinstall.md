---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5d5c517e4b146c94b931caf09f354ed5a348080
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369568"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="7d9ec-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d9ec-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="7d9ec-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d9ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d9ec-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d9ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d9ec-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7d9ec-106">Not yet documented</span></span>


<span data-ttu-id="7d9ec-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="7d9ec-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d9ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d9ec-108">Properties</span></span>
|<span data-ttu-id="7d9ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="7d9ec-109">Property</span></span>|<span data-ttu-id="7d9ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="7d9ec-110">Type</span></span>|<span data-ttu-id="7d9ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d9ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d9ec-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7d9ec-112">activeHoursStart</span></span>|<span data-ttu-id="7d9ec-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d9ec-113">TimeOfDay</span></span>|<span data-ttu-id="7d9ec-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="7d9ec-114">Active Hours Start</span></span>|
|<span data-ttu-id="7d9ec-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7d9ec-115">activeHoursEnd</span></span>|<span data-ttu-id="7d9ec-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d9ec-116">TimeOfDay</span></span>|<span data-ttu-id="7d9ec-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="7d9ec-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d9ec-118">关系</span><span class="sxs-lookup"><span data-stu-id="7d9ec-118">Relationships</span></span>
<span data-ttu-id="7d9ec-119">无</span><span class="sxs-lookup"><span data-stu-id="7d9ec-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d9ec-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d9ec-120">JSON Representation</span></span>
<span data-ttu-id="7d9ec-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d9ec-121">Here is a JSON representation of the resource.</span></span>
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



