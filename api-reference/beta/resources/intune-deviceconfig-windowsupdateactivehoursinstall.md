---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad513d4022b991917a7afe8ce9bdf012095621de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931242"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="24b74-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="24b74-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="24b74-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="24b74-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24b74-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24b74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24b74-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24b74-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24b74-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24b74-107">Not yet documented</span></span>

<span data-ttu-id="24b74-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="24b74-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24b74-109">属性</span><span class="sxs-lookup"><span data-stu-id="24b74-109">Properties</span></span>
|<span data-ttu-id="24b74-110">属性</span><span class="sxs-lookup"><span data-stu-id="24b74-110">Property</span></span>|<span data-ttu-id="24b74-111">类型</span><span class="sxs-lookup"><span data-stu-id="24b74-111">Type</span></span>|<span data-ttu-id="24b74-112">说明</span><span class="sxs-lookup"><span data-stu-id="24b74-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b74-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="24b74-113">activeHoursStart</span></span>|<span data-ttu-id="24b74-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="24b74-114">TimeOfDay</span></span>|<span data-ttu-id="24b74-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="24b74-115">Active Hours Start</span></span>|
|<span data-ttu-id="24b74-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="24b74-116">activeHoursEnd</span></span>|<span data-ttu-id="24b74-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="24b74-117">TimeOfDay</span></span>|<span data-ttu-id="24b74-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="24b74-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="24b74-119">关系</span><span class="sxs-lookup"><span data-stu-id="24b74-119">Relationships</span></span>
<span data-ttu-id="24b74-120">无</span><span class="sxs-lookup"><span data-stu-id="24b74-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24b74-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24b74-121">JSON Representation</span></span>
<span data-ttu-id="24b74-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24b74-122">Here is a JSON representation of the resource.</span></span>
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





