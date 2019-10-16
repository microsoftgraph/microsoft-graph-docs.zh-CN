---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用程序安装后重启协调的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84e4b231c189f02cf1e19401933ae517d8955263
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538761"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="b0f48-103">win32LobAppRestartSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0f48-103">win32LobAppRestartSettings resource type</span></span>

> <span data-ttu-id="b0f48-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0f48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0f48-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0f48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0f48-106">包含描述应用程序安装后重启协调的属性。</span><span class="sxs-lookup"><span data-stu-id="b0f48-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="b0f48-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0f48-107">Properties</span></span>
|<span data-ttu-id="b0f48-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0f48-108">Property</span></span>|<span data-ttu-id="b0f48-109">类型</span><span class="sxs-lookup"><span data-stu-id="b0f48-109">Type</span></span>|<span data-ttu-id="b0f48-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0f48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f48-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0f48-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="b0f48-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b0f48-112">Int32</span></span>|<span data-ttu-id="b0f48-113">在应用程序安装后重新启动设备之前要等待的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b0f48-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="b0f48-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0f48-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="b0f48-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b0f48-115">Int32</span></span>|<span data-ttu-id="b0f48-116">为等待重新启动而显示倒计时对话框之前的重新启动时间的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b0f48-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="b0f48-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0f48-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="b0f48-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b0f48-118">Int32</span></span>|<span data-ttu-id="b0f48-119">选择 "暂停" 按钮时暂停 "重新启动通知" 对话框的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b0f48-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0f48-120">关系</span><span class="sxs-lookup"><span data-stu-id="b0f48-120">Relationships</span></span>
<span data-ttu-id="b0f48-121">无</span><span class="sxs-lookup"><span data-stu-id="b0f48-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0f48-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0f48-122">JSON Representation</span></span>
<span data-ttu-id="b0f48-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0f48-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



