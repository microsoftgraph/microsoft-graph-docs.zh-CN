---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a3164a11c940538bc6ffc67ac4b1911df85f27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525388"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="14743-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="14743-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="14743-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14743-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14743-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14743-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14743-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14743-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14743-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14743-107">Not yet documented</span></span>


<span data-ttu-id="14743-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="14743-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14743-109">属性</span><span class="sxs-lookup"><span data-stu-id="14743-109">Properties</span></span>
|<span data-ttu-id="14743-110">属性</span><span class="sxs-lookup"><span data-stu-id="14743-110">Property</span></span>|<span data-ttu-id="14743-111">类型</span><span class="sxs-lookup"><span data-stu-id="14743-111">Type</span></span>|<span data-ttu-id="14743-112">说明</span><span class="sxs-lookup"><span data-stu-id="14743-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14743-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="14743-113">activeHoursStart</span></span>|<span data-ttu-id="14743-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="14743-114">TimeOfDay</span></span>|<span data-ttu-id="14743-115">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="14743-115">Active Hours Start</span></span>|
|<span data-ttu-id="14743-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="14743-116">activeHoursEnd</span></span>|<span data-ttu-id="14743-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="14743-117">TimeOfDay</span></span>|<span data-ttu-id="14743-118">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="14743-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="14743-119">关系</span><span class="sxs-lookup"><span data-stu-id="14743-119">Relationships</span></span>
<span data-ttu-id="14743-120">无</span><span class="sxs-lookup"><span data-stu-id="14743-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14743-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14743-121">JSON Representation</span></span>
<span data-ttu-id="14743-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14743-122">Here is a JSON representation of the resource.</span></span>
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



