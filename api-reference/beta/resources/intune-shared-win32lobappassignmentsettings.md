---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e1f650919e3e7cd9fa55d7e05d3fc706b18f95db
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538691"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="5b624-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b624-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5b624-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b624-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b624-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b624-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b624-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="5b624-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="5b624-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5b624-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b624-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b624-108">Properties</span></span>
|<span data-ttu-id="5b624-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b624-109">Property</span></span>|<span data-ttu-id="5b624-110">类型</span><span class="sxs-lookup"><span data-stu-id="5b624-110">Type</span></span>|<span data-ttu-id="5b624-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b624-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b624-112">通知</span><span class="sxs-lookup"><span data-stu-id="5b624-112">notifications</span></span>|[<span data-ttu-id="5b624-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="5b624-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="5b624-114">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="5b624-114">The notification status for this app assignment.</span></span> <span data-ttu-id="5b624-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="5b624-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="5b624-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="5b624-116">restartSettings</span></span>|[<span data-ttu-id="5b624-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="5b624-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="5b624-118">要应用于此应用程序分配的重新启动设置。</span><span class="sxs-lookup"><span data-stu-id="5b624-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="5b624-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="5b624-119">installTimeSettings</span></span>|[<span data-ttu-id="5b624-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="5b624-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="5b624-121">要应用于此应用程序分配的安装时设置。</span><span class="sxs-lookup"><span data-stu-id="5b624-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b624-122">关系</span><span class="sxs-lookup"><span data-stu-id="5b624-122">Relationships</span></span>
<span data-ttu-id="5b624-123">无</span><span class="sxs-lookup"><span data-stu-id="5b624-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b624-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b624-124">JSON Representation</span></span>
<span data-ttu-id="5b624-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b624-125">Here is a JSON representation of the resource.</span></span>
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



