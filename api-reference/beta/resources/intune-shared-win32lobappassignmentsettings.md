---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c56d236c48918592394dc143bc6f2c45fb80401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523497"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="e0bcb-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0bcb-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="e0bcb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e0bcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0bcb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0bcb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0bcb-107">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="e0bcb-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e0bcb-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0bcb-109">属性</span><span class="sxs-lookup"><span data-stu-id="e0bcb-109">Properties</span></span>
|<span data-ttu-id="e0bcb-110">属性</span><span class="sxs-lookup"><span data-stu-id="e0bcb-110">Property</span></span>|<span data-ttu-id="e0bcb-111">类型</span><span class="sxs-lookup"><span data-stu-id="e0bcb-111">Type</span></span>|<span data-ttu-id="e0bcb-112">说明</span><span class="sxs-lookup"><span data-stu-id="e0bcb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0bcb-113">通知</span><span class="sxs-lookup"><span data-stu-id="e0bcb-113">notifications</span></span>|[<span data-ttu-id="e0bcb-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="e0bcb-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="e0bcb-115">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-115">The notification status for this app assignment.</span></span> <span data-ttu-id="e0bcb-116">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="e0bcb-117">restartSettings</span><span class="sxs-lookup"><span data-stu-id="e0bcb-117">restartSettings</span></span>|[<span data-ttu-id="e0bcb-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="e0bcb-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="e0bcb-119">要应用于此应用程序分配的重新启动设置。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="e0bcb-120">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="e0bcb-120">installTimeSettings</span></span>|[<span data-ttu-id="e0bcb-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="e0bcb-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="e0bcb-122">要应用于此应用程序分配的安装时设置。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-122">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0bcb-123">关系</span><span class="sxs-lookup"><span data-stu-id="e0bcb-123">Relationships</span></span>
<span data-ttu-id="e0bcb-124">无</span><span class="sxs-lookup"><span data-stu-id="e0bcb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0bcb-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0bcb-125">JSON Representation</span></span>
<span data-ttu-id="e0bcb-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0bcb-126">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



