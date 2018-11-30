---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
ms.openlocfilehash: 7a40a791a9a00d7cfd60287bade1759592e1bcf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048016"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b7e4f-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7e4f-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b7e4f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b7e4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7e4f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7e4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7e4f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b7e4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7e4f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b7e4f-107">Not yet documented</span></span>

<span data-ttu-id="b7e4f-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b7e4f-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7e4f-109">属性</span><span class="sxs-lookup"><span data-stu-id="b7e4f-109">Properties</span></span>
|<span data-ttu-id="b7e4f-110">属性</span><span class="sxs-lookup"><span data-stu-id="b7e4f-110">Property</span></span>|<span data-ttu-id="b7e4f-111">类型</span><span class="sxs-lookup"><span data-stu-id="b7e4f-111">Type</span></span>|<span data-ttu-id="b7e4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="b7e4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7e4f-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b7e4f-113">activeHoursStart</span></span>|<span data-ttu-id="b7e4f-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7e4f-114">TimeOfDay</span></span>|<span data-ttu-id="b7e4f-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="b7e4f-115">Active Hours Start</span></span>|
|<span data-ttu-id="b7e4f-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b7e4f-116">activeHoursEnd</span></span>|<span data-ttu-id="b7e4f-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7e4f-117">TimeOfDay</span></span>|<span data-ttu-id="b7e4f-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="b7e4f-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7e4f-119">关系</span><span class="sxs-lookup"><span data-stu-id="b7e4f-119">Relationships</span></span>
<span data-ttu-id="b7e4f-120">无</span><span class="sxs-lookup"><span data-stu-id="b7e4f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7e4f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7e4f-121">JSON Representation</span></span>
<span data-ttu-id="b7e4f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7e4f-122">Here is a JSON representation of the resource.</span></span>
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





