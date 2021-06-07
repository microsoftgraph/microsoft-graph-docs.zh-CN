---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用安装后重启协调的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db011486f1ec26afcc7e045afd2e1be1b553ec7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757828"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="0a34d-103">win32LobAppRestartSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a34d-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="0a34d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a34d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a34d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a34d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a34d-106">包含描述应用安装后重启协调的属性。</span><span class="sxs-lookup"><span data-stu-id="0a34d-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="0a34d-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a34d-107">Properties</span></span>
|<span data-ttu-id="0a34d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a34d-108">Property</span></span>|<span data-ttu-id="0a34d-109">类型</span><span class="sxs-lookup"><span data-stu-id="0a34d-109">Type</span></span>|<span data-ttu-id="0a34d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0a34d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a34d-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="0a34d-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="0a34d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0a34d-112">Int32</span></span>|<span data-ttu-id="0a34d-113">应用安装后重启设备之前等待的分钟数。</span><span class="sxs-lookup"><span data-stu-id="0a34d-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="0a34d-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="0a34d-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="0a34d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0a34d-115">Int32</span></span>|<span data-ttu-id="0a34d-116">重启时间前显示挂起重启的倒计时器对话框的分钟数。</span><span class="sxs-lookup"><span data-stu-id="0a34d-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="0a34d-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="0a34d-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="0a34d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="0a34d-118">Int32</span></span>|<span data-ttu-id="0a34d-119">选择"暂停"按钮时暂停重新启动通知对话框的分钟数。</span><span class="sxs-lookup"><span data-stu-id="0a34d-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a34d-120">关系</span><span class="sxs-lookup"><span data-stu-id="0a34d-120">Relationships</span></span>
<span data-ttu-id="0a34d-121">无</span><span class="sxs-lookup"><span data-stu-id="0a34d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a34d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a34d-122">JSON Representation</span></span>
<span data-ttu-id="0a34d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a34d-123">Here is a JSON representation of the resource.</span></span>
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




