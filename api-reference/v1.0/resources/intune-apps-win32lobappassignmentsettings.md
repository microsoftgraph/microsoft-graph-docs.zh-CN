---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76e189d684999e3922b625def26d4d0cfcb6a3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752208"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="49e80-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="49e80-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="49e80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49e80-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49e80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49e80-106">包含用于将 Win32 LOB 移动应用分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="49e80-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="49e80-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="49e80-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49e80-108">属性</span><span class="sxs-lookup"><span data-stu-id="49e80-108">Properties</span></span>
|<span data-ttu-id="49e80-109">属性</span><span class="sxs-lookup"><span data-stu-id="49e80-109">Property</span></span>|<span data-ttu-id="49e80-110">类型</span><span class="sxs-lookup"><span data-stu-id="49e80-110">Type</span></span>|<span data-ttu-id="49e80-111">Description</span><span class="sxs-lookup"><span data-stu-id="49e80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e80-112">通知</span><span class="sxs-lookup"><span data-stu-id="49e80-112">notifications</span></span>|[<span data-ttu-id="49e80-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="49e80-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="49e80-114">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="49e80-114">The notification status for this app assignment.</span></span> <span data-ttu-id="49e80-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="49e80-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="49e80-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="49e80-116">restartSettings</span></span>|[<span data-ttu-id="49e80-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="49e80-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="49e80-118">要应用于此应用分配的重启设置。</span><span class="sxs-lookup"><span data-stu-id="49e80-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="49e80-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="49e80-119">installTimeSettings</span></span>|[<span data-ttu-id="49e80-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="49e80-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="49e80-121">要应用于此应用分配的安装时间设置。</span><span class="sxs-lookup"><span data-stu-id="49e80-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="49e80-122">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="49e80-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="49e80-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="49e80-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="49e80-124">此应用分配的传递优化优先级。</span><span class="sxs-lookup"><span data-stu-id="49e80-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="49e80-125">国家云环境不支持此设置。</span><span class="sxs-lookup"><span data-stu-id="49e80-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="49e80-126">可取值为：`notConfigured`、`foreground`。</span><span class="sxs-lookup"><span data-stu-id="49e80-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49e80-127">关系</span><span class="sxs-lookup"><span data-stu-id="49e80-127">Relationships</span></span>
<span data-ttu-id="49e80-128">无</span><span class="sxs-lookup"><span data-stu-id="49e80-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49e80-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49e80-129">JSON Representation</span></span>
<span data-ttu-id="49e80-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49e80-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```




