---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用程序安装后重启协调的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f9fefd725f59c9884e3fe4442a7154aaed4529
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255635"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="f0360-103">win32LobAppRestartSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0360-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="f0360-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0360-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0360-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0360-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0360-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0360-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0360-107">包含描述应用程序安装后重启协调的属性。</span><span class="sxs-lookup"><span data-stu-id="f0360-107">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="f0360-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0360-108">Properties</span></span>
|<span data-ttu-id="f0360-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0360-109">Property</span></span>|<span data-ttu-id="f0360-110">类型</span><span class="sxs-lookup"><span data-stu-id="f0360-110">Type</span></span>|<span data-ttu-id="f0360-111">描述</span><span class="sxs-lookup"><span data-stu-id="f0360-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0360-112">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="f0360-112">gracePeriodInMinutes</span></span>|<span data-ttu-id="f0360-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f0360-113">Int32</span></span>|<span data-ttu-id="f0360-114">在应用程序安装后重新启动设备之前要等待的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f0360-114">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="f0360-115">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="f0360-115">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="f0360-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f0360-116">Int32</span></span>|<span data-ttu-id="f0360-117">为等待重新启动而显示倒计时对话框之前的重新启动时间的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f0360-117">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="f0360-118">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="f0360-118">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="f0360-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f0360-119">Int32</span></span>|<span data-ttu-id="f0360-120">选择 "暂停" 按钮时暂停 "重新启动通知" 对话框的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f0360-120">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0360-121">关系</span><span class="sxs-lookup"><span data-stu-id="f0360-121">Relationships</span></span>
<span data-ttu-id="f0360-122">无</span><span class="sxs-lookup"><span data-stu-id="f0360-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0360-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0360-123">JSON Representation</span></span>
<span data-ttu-id="f0360-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0360-124">Here is a JSON representation of the resource.</span></span>
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




