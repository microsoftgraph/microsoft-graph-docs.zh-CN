---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed4f909db5dd31195ace7d98151b226b03849c81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967180"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="fd4a2-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd4a2-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="fd4a2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fd4a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd4a2-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fd4a2-105">Not yet documented</span></span>

<span data-ttu-id="fd4a2-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="fd4a2-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd4a2-107">属性</span><span class="sxs-lookup"><span data-stu-id="fd4a2-107">Properties</span></span>
|<span data-ttu-id="fd4a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd4a2-108">Property</span></span>|<span data-ttu-id="fd4a2-109">类型</span><span class="sxs-lookup"><span data-stu-id="fd4a2-109">Type</span></span>|<span data-ttu-id="fd4a2-110">说明</span><span class="sxs-lookup"><span data-stu-id="fd4a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd4a2-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="fd4a2-111">activeHoursStart</span></span>|<span data-ttu-id="fd4a2-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fd4a2-112">TimeOfDay</span></span>|<span data-ttu-id="fd4a2-113">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="fd4a2-113">Active Hours Start</span></span>|
|<span data-ttu-id="fd4a2-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="fd4a2-114">activeHoursEnd</span></span>|<span data-ttu-id="fd4a2-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fd4a2-115">TimeOfDay</span></span>|<span data-ttu-id="fd4a2-116">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="fd4a2-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd4a2-117">关系</span><span class="sxs-lookup"><span data-stu-id="fd4a2-117">Relationships</span></span>
<span data-ttu-id="fd4a2-118">无</span><span class="sxs-lookup"><span data-stu-id="fd4a2-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd4a2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd4a2-119">JSON Representation</span></span>
<span data-ttu-id="fd4a2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd4a2-120">Here is a JSON representation of the resource.</span></span>
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



