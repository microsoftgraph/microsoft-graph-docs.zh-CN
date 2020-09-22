---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e84a740a45cb57417c81b5c99a892642097413b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020252"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="1cca1-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cca1-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="1cca1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cca1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cca1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1cca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cca1-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="1cca1-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="1cca1-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1cca1-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1cca1-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cca1-108">Properties</span></span>
|<span data-ttu-id="1cca1-109">属性</span><span class="sxs-lookup"><span data-stu-id="1cca1-109">Property</span></span>|<span data-ttu-id="1cca1-110">类型</span><span class="sxs-lookup"><span data-stu-id="1cca1-110">Type</span></span>|<span data-ttu-id="1cca1-111">说明</span><span class="sxs-lookup"><span data-stu-id="1cca1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cca1-112">通知</span><span class="sxs-lookup"><span data-stu-id="1cca1-112">notifications</span></span>|[<span data-ttu-id="1cca1-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="1cca1-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="1cca1-114">此应用分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="1cca1-114">The notification status for this app assignment.</span></span> <span data-ttu-id="1cca1-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="1cca1-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="1cca1-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="1cca1-116">restartSettings</span></span>|[<span data-ttu-id="1cca1-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="1cca1-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="1cca1-118">要应用于此应用程序分配的重新启动设置。</span><span class="sxs-lookup"><span data-stu-id="1cca1-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="1cca1-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="1cca1-119">installTimeSettings</span></span>|[<span data-ttu-id="1cca1-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="1cca1-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="1cca1-121">要应用于此应用程序分配的安装时设置。</span><span class="sxs-lookup"><span data-stu-id="1cca1-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cca1-122">关系</span><span class="sxs-lookup"><span data-stu-id="1cca1-122">Relationships</span></span>
<span data-ttu-id="1cca1-123">无</span><span class="sxs-lookup"><span data-stu-id="1cca1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cca1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cca1-124">JSON Representation</span></span>
<span data-ttu-id="1cca1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cca1-125">Here is a JSON representation of the resource.</span></span>
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





