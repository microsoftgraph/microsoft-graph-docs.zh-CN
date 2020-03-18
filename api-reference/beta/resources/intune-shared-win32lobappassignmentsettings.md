---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 340dc21cce7b52ebc55c13488f7340c7b66f9e26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767041"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="1e83e-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e83e-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1e83e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e83e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e83e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e83e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e83e-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="1e83e-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="1e83e-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1e83e-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e83e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e83e-108">Properties</span></span>
|<span data-ttu-id="1e83e-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e83e-109">Property</span></span>|<span data-ttu-id="1e83e-110">类型</span><span class="sxs-lookup"><span data-stu-id="1e83e-110">Type</span></span>|<span data-ttu-id="1e83e-111">说明</span><span class="sxs-lookup"><span data-stu-id="1e83e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e83e-112">通知</span><span class="sxs-lookup"><span data-stu-id="1e83e-112">notifications</span></span>|[<span data-ttu-id="1e83e-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="1e83e-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="1e83e-114">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="1e83e-114">The notification status for this app assignment.</span></span> <span data-ttu-id="1e83e-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="1e83e-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="1e83e-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="1e83e-116">restartSettings</span></span>|[<span data-ttu-id="1e83e-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="1e83e-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="1e83e-118">要应用于此应用程序分配的重新启动设置。</span><span class="sxs-lookup"><span data-stu-id="1e83e-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="1e83e-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="1e83e-119">installTimeSettings</span></span>|[<span data-ttu-id="1e83e-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="1e83e-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="1e83e-121">要应用于此应用程序分配的安装时设置。</span><span class="sxs-lookup"><span data-stu-id="1e83e-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="1e83e-122">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="1e83e-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="1e83e-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="1e83e-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="1e83e-124">此应用分配的传递优化优先级。</span><span class="sxs-lookup"><span data-stu-id="1e83e-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="1e83e-125">在国家/地区云环境中不支持此设置。</span><span class="sxs-lookup"><span data-stu-id="1e83e-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="1e83e-126">可取值为：`notConfigured`、`foreground`。</span><span class="sxs-lookup"><span data-stu-id="1e83e-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e83e-127">关系</span><span class="sxs-lookup"><span data-stu-id="1e83e-127">Relationships</span></span>
<span data-ttu-id="1e83e-128">无</span><span class="sxs-lookup"><span data-stu-id="1e83e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e83e-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e83e-129">JSON Representation</span></span>
<span data-ttu-id="1e83e-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e83e-130">Here is a JSON representation of the resource.</span></span>
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



