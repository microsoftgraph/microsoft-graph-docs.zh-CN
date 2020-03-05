---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 546d335fec5945703e790c6cf712f9c37d2394ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523308"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="90a5f-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="90a5f-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="90a5f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="90a5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90a5f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90a5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90a5f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90a5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90a5f-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="90a5f-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="90a5f-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90a5f-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90a5f-109">属性</span><span class="sxs-lookup"><span data-stu-id="90a5f-109">Properties</span></span>
|<span data-ttu-id="90a5f-110">属性</span><span class="sxs-lookup"><span data-stu-id="90a5f-110">Property</span></span>|<span data-ttu-id="90a5f-111">类型</span><span class="sxs-lookup"><span data-stu-id="90a5f-111">Type</span></span>|<span data-ttu-id="90a5f-112">说明</span><span class="sxs-lookup"><span data-stu-id="90a5f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90a5f-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="90a5f-113">occurrenceDateTime</span></span>|<span data-ttu-id="90a5f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a5f-114">DateTimeOffset</span></span>|<span data-ttu-id="90a5f-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="90a5f-115">Time when the history item occurred.</span></span> <span data-ttu-id="90a5f-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90a5f-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="90a5f-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="90a5f-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="90a5f-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="90a5f-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="90a5f-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="90a5f-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="90a5f-120">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90a5f-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="90a5f-121">actionType</span><span class="sxs-lookup"><span data-stu-id="90a5f-121">actionType</span></span>|[<span data-ttu-id="90a5f-122">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="90a5f-122">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="90a5f-123">Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="90a5f-123">Action type for Intune Application.</span></span> <span data-ttu-id="90a5f-124">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="90a5f-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="90a5f-125">runState</span><span class="sxs-lookup"><span data-stu-id="90a5f-125">runState</span></span>|[<span data-ttu-id="90a5f-126">runState</span><span class="sxs-lookup"><span data-stu-id="90a5f-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="90a5f-127">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="90a5f-127">Status of the item.</span></span> <span data-ttu-id="90a5f-128">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="90a5f-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="90a5f-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="90a5f-129">errorCode</span></span>|<span data-ttu-id="90a5f-130">String</span><span class="sxs-lookup"><span data-stu-id="90a5f-130">String</span></span>|<span data-ttu-id="90a5f-131">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="90a5f-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90a5f-132">关系</span><span class="sxs-lookup"><span data-stu-id="90a5f-132">Relationships</span></span>
<span data-ttu-id="90a5f-133">无</span><span class="sxs-lookup"><span data-stu-id="90a5f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90a5f-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90a5f-134">JSON Representation</span></span>
<span data-ttu-id="90a5f-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90a5f-135">Here is a JSON representation of the resource.</span></span>
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



