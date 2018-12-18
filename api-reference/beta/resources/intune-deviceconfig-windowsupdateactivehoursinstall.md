---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 6d1328723f546f553bc31903d36ada2242d8cda3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307103"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="5deb7-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="5deb7-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="5deb7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5deb7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5deb7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5deb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5deb7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5deb7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5deb7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5deb7-107">Not yet documented</span></span>

<span data-ttu-id="5deb7-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="5deb7-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5deb7-109">属性</span><span class="sxs-lookup"><span data-stu-id="5deb7-109">Properties</span></span>
|<span data-ttu-id="5deb7-110">属性</span><span class="sxs-lookup"><span data-stu-id="5deb7-110">Property</span></span>|<span data-ttu-id="5deb7-111">类型</span><span class="sxs-lookup"><span data-stu-id="5deb7-111">Type</span></span>|<span data-ttu-id="5deb7-112">说明</span><span class="sxs-lookup"><span data-stu-id="5deb7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5deb7-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="5deb7-113">activeHoursStart</span></span>|<span data-ttu-id="5deb7-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5deb7-114">TimeOfDay</span></span>|<span data-ttu-id="5deb7-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="5deb7-115">Active Hours Start</span></span>|
|<span data-ttu-id="5deb7-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="5deb7-116">activeHoursEnd</span></span>|<span data-ttu-id="5deb7-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5deb7-117">TimeOfDay</span></span>|<span data-ttu-id="5deb7-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="5deb7-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="5deb7-119">关系</span><span class="sxs-lookup"><span data-stu-id="5deb7-119">Relationships</span></span>
<span data-ttu-id="5deb7-120">无</span><span class="sxs-lookup"><span data-stu-id="5deb7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5deb7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5deb7-121">JSON Representation</span></span>
<span data-ttu-id="5deb7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5deb7-122">Here is a JSON representation of the resource.</span></span>
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





