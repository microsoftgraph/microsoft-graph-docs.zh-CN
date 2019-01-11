---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 797cfc0f9279f0ab232991a95714d31ce37211a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818422"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="5053b-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="5053b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="5053b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5053b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5053b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5053b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5053b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5053b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5053b-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5053b-107">Not yet documented</span></span>

<span data-ttu-id="5053b-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="5053b-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5053b-109">属性</span><span class="sxs-lookup"><span data-stu-id="5053b-109">Properties</span></span>
|<span data-ttu-id="5053b-110">属性</span><span class="sxs-lookup"><span data-stu-id="5053b-110">Property</span></span>|<span data-ttu-id="5053b-111">类型</span><span class="sxs-lookup"><span data-stu-id="5053b-111">Type</span></span>|<span data-ttu-id="5053b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5053b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5053b-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="5053b-113">activeHoursStart</span></span>|<span data-ttu-id="5053b-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5053b-114">TimeOfDay</span></span>|<span data-ttu-id="5053b-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="5053b-115">Active Hours Start</span></span>|
|<span data-ttu-id="5053b-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="5053b-116">activeHoursEnd</span></span>|<span data-ttu-id="5053b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5053b-117">TimeOfDay</span></span>|<span data-ttu-id="5053b-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="5053b-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="5053b-119">关系</span><span class="sxs-lookup"><span data-stu-id="5053b-119">Relationships</span></span>
<span data-ttu-id="5053b-120">无</span><span class="sxs-lookup"><span data-stu-id="5053b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5053b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5053b-121">JSON Representation</span></span>
<span data-ttu-id="5053b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5053b-122">Here is a JSON representation of the resource.</span></span>
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





