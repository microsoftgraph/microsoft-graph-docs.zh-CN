---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71a5786bb5c2a89d6a4397e999155a31cc0f9369
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729099"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="9f837-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f837-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="9f837-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f837-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f837-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f837-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f837-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="9f837-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9f837-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f837-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f837-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f837-108">Properties</span></span>
|<span data-ttu-id="9f837-109">属性</span><span class="sxs-lookup"><span data-stu-id="9f837-109">Property</span></span>|<span data-ttu-id="9f837-110">类型</span><span class="sxs-lookup"><span data-stu-id="9f837-110">Type</span></span>|<span data-ttu-id="9f837-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f837-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f837-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9f837-112">occurrenceDateTime</span></span>|<span data-ttu-id="9f837-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f837-113">DateTimeOffset</span></span>|<span data-ttu-id="9f837-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="9f837-114">Time when the history item occurred.</span></span> <span data-ttu-id="9f837-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f837-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9f837-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9f837-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="9f837-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9f837-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="9f837-118">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="9f837-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="9f837-119">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f837-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9f837-120">actionType</span><span class="sxs-lookup"><span data-stu-id="9f837-120">actionType</span></span>|[<span data-ttu-id="9f837-121">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="9f837-121">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="9f837-122">Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="9f837-122">Action type for Intune Application.</span></span> <span data-ttu-id="9f837-123">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="9f837-123">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="9f837-124">runState</span><span class="sxs-lookup"><span data-stu-id="9f837-124">runState</span></span>|[<span data-ttu-id="9f837-125">runState</span><span class="sxs-lookup"><span data-stu-id="9f837-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="9f837-126">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="9f837-126">Status of the item.</span></span> <span data-ttu-id="9f837-127">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="9f837-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="9f837-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="9f837-128">errorCode</span></span>|<span data-ttu-id="9f837-129">String</span><span class="sxs-lookup"><span data-stu-id="9f837-129">String</span></span>|<span data-ttu-id="9f837-130">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="9f837-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f837-131">关系</span><span class="sxs-lookup"><span data-stu-id="9f837-131">Relationships</span></span>
<span data-ttu-id="9f837-132">无</span><span class="sxs-lookup"><span data-stu-id="9f837-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f837-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f837-133">JSON Representation</span></span>
<span data-ttu-id="9f837-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f837-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```



