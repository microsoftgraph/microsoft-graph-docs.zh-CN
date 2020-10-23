---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 23470828293f7655c6779d369bb24055b4966c4e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736000"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="7d548-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d548-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="7d548-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d548-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d548-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d548-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d548-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d548-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d548-107">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="7d548-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="7d548-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7d548-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d548-109">属性</span><span class="sxs-lookup"><span data-stu-id="7d548-109">Properties</span></span>
|<span data-ttu-id="7d548-110">属性</span><span class="sxs-lookup"><span data-stu-id="7d548-110">Property</span></span>|<span data-ttu-id="7d548-111">类型</span><span class="sxs-lookup"><span data-stu-id="7d548-111">Type</span></span>|<span data-ttu-id="7d548-112">说明</span><span class="sxs-lookup"><span data-stu-id="7d548-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d548-113">通知</span><span class="sxs-lookup"><span data-stu-id="7d548-113">notifications</span></span>|[<span data-ttu-id="7d548-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="7d548-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="7d548-115">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="7d548-115">The notification status for this app assignment.</span></span> <span data-ttu-id="7d548-116">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="7d548-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="7d548-117">restartSettings</span><span class="sxs-lookup"><span data-stu-id="7d548-117">restartSettings</span></span>|[<span data-ttu-id="7d548-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="7d548-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="7d548-119">要应用于此应用程序分配的重新启动设置。</span><span class="sxs-lookup"><span data-stu-id="7d548-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="7d548-120">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="7d548-120">installTimeSettings</span></span>|[<span data-ttu-id="7d548-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="7d548-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="7d548-122">要应用于此应用程序分配的安装时设置。</span><span class="sxs-lookup"><span data-stu-id="7d548-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="7d548-123">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="7d548-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="7d548-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="7d548-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="7d548-125">此应用分配的传递优化优先级。</span><span class="sxs-lookup"><span data-stu-id="7d548-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="7d548-126">在国家/地区云环境中不支持此设置。</span><span class="sxs-lookup"><span data-stu-id="7d548-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="7d548-127">可取值为：`notConfigured`、`foreground`。</span><span class="sxs-lookup"><span data-stu-id="7d548-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d548-128">关系</span><span class="sxs-lookup"><span data-stu-id="7d548-128">Relationships</span></span>
<span data-ttu-id="7d548-129">无</span><span class="sxs-lookup"><span data-stu-id="7d548-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d548-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d548-130">JSON Representation</span></span>
<span data-ttu-id="7d548-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d548-131">Here is a JSON representation of the resource.</span></span>
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





