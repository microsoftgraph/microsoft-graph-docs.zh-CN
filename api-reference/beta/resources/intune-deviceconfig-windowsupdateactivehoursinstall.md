---
title: windowsUpdateActiveHoursInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9deab255749e70cfd165f28c27c09182b298e00a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144091"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="bc87b-103">windowsUpdateActiveHoursInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc87b-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="bc87b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc87b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc87b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc87b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc87b-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc87b-106">Not yet documented</span></span>


<span data-ttu-id="bc87b-107">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="bc87b-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc87b-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc87b-108">Properties</span></span>
|<span data-ttu-id="bc87b-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc87b-109">Property</span></span>|<span data-ttu-id="bc87b-110">类型</span><span class="sxs-lookup"><span data-stu-id="bc87b-110">Type</span></span>|<span data-ttu-id="bc87b-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc87b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc87b-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="bc87b-112">activeHoursStart</span></span>|<span data-ttu-id="bc87b-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bc87b-113">TimeOfDay</span></span>|<span data-ttu-id="bc87b-114">开始活动时间</span><span class="sxs-lookup"><span data-stu-id="bc87b-114">Active Hours Start</span></span>|
|<span data-ttu-id="bc87b-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="bc87b-115">activeHoursEnd</span></span>|<span data-ttu-id="bc87b-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bc87b-116">TimeOfDay</span></span>|<span data-ttu-id="bc87b-117">结束活动时间</span><span class="sxs-lookup"><span data-stu-id="bc87b-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc87b-118">关系</span><span class="sxs-lookup"><span data-stu-id="bc87b-118">Relationships</span></span>
<span data-ttu-id="bc87b-119">无</span><span class="sxs-lookup"><span data-stu-id="bc87b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc87b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc87b-120">JSON Representation</span></span>
<span data-ttu-id="bc87b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc87b-121">Here is a JSON representation of the resource.</span></span>
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




