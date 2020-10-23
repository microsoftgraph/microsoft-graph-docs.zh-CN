---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9d757b8b26995d30789c4af0753ed0e1fb5917c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696039"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="dfd31-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfd31-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="dfd31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfd31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfd31-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfd31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfd31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfd31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfd31-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="dfd31-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="dfd31-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfd31-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfd31-109">属性</span><span class="sxs-lookup"><span data-stu-id="dfd31-109">Properties</span></span>
|<span data-ttu-id="dfd31-110">属性</span><span class="sxs-lookup"><span data-stu-id="dfd31-110">Property</span></span>|<span data-ttu-id="dfd31-111">类型</span><span class="sxs-lookup"><span data-stu-id="dfd31-111">Type</span></span>|<span data-ttu-id="dfd31-112">说明</span><span class="sxs-lookup"><span data-stu-id="dfd31-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfd31-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="dfd31-113">occurrenceDateTime</span></span>|<span data-ttu-id="dfd31-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfd31-114">DateTimeOffset</span></span>|<span data-ttu-id="dfd31-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="dfd31-115">Time when the history item occurred.</span></span> <span data-ttu-id="dfd31-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfd31-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="dfd31-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dfd31-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="dfd31-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dfd31-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="dfd31-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="dfd31-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="dfd31-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfd31-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="dfd31-121">actionType</span><span class="sxs-lookup"><span data-stu-id="dfd31-121">actionType</span></span>|[<span data-ttu-id="dfd31-122">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="dfd31-122">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="dfd31-123">Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="dfd31-123">Action type for Intune Application.</span></span> <span data-ttu-id="dfd31-124">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="dfd31-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="dfd31-125">runState</span><span class="sxs-lookup"><span data-stu-id="dfd31-125">runState</span></span>|[<span data-ttu-id="dfd31-126">runState</span><span class="sxs-lookup"><span data-stu-id="dfd31-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="dfd31-127">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="dfd31-127">Status of the item.</span></span> <span data-ttu-id="dfd31-128">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="dfd31-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="dfd31-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="dfd31-129">errorCode</span></span>|<span data-ttu-id="dfd31-130">String</span><span class="sxs-lookup"><span data-stu-id="dfd31-130">String</span></span>|<span data-ttu-id="dfd31-131">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="dfd31-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfd31-132">关系</span><span class="sxs-lookup"><span data-stu-id="dfd31-132">Relationships</span></span>
<span data-ttu-id="dfd31-133">无</span><span class="sxs-lookup"><span data-stu-id="dfd31-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfd31-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfd31-134">JSON Representation</span></span>
<span data-ttu-id="dfd31-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfd31-135">Here is a JSON representation of the resource.</span></span>
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





