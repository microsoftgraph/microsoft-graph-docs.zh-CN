---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a61c81bd0d4080cbf8ae706ae100a9fb1332f9a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159057"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="5f23e-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f23e-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="5f23e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f23e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f23e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f23e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f23e-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="5f23e-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5f23e-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5f23e-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f23e-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f23e-108">Properties</span></span>
|<span data-ttu-id="5f23e-109">属性</span><span class="sxs-lookup"><span data-stu-id="5f23e-109">Property</span></span>|<span data-ttu-id="5f23e-110">类型</span><span class="sxs-lookup"><span data-stu-id="5f23e-110">Type</span></span>|<span data-ttu-id="5f23e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f23e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f23e-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5f23e-112">occurrenceDateTime</span></span>|<span data-ttu-id="5f23e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f23e-113">DateTimeOffset</span></span>|<span data-ttu-id="5f23e-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="5f23e-114">Time when the history item occurred.</span></span> <span data-ttu-id="5f23e-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5f23e-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5f23e-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5f23e-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="5f23e-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5f23e-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="5f23e-118">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="5f23e-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="5f23e-119">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5f23e-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5f23e-120">actionType</span><span class="sxs-lookup"><span data-stu-id="5f23e-120">actionType</span></span>|[<span data-ttu-id="5f23e-121">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="5f23e-121">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="5f23e-122">Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f23e-122">Action type for Intune Application.</span></span> <span data-ttu-id="5f23e-123">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="5f23e-123">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="5f23e-124">runState</span><span class="sxs-lookup"><span data-stu-id="5f23e-124">runState</span></span>|[<span data-ttu-id="5f23e-125">runState</span><span class="sxs-lookup"><span data-stu-id="5f23e-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5f23e-126">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="5f23e-126">Status of the item.</span></span> <span data-ttu-id="5f23e-127">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="5f23e-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="5f23e-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="5f23e-128">errorCode</span></span>|<span data-ttu-id="5f23e-129">String</span><span class="sxs-lookup"><span data-stu-id="5f23e-129">String</span></span>|<span data-ttu-id="5f23e-130">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="5f23e-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f23e-131">关系</span><span class="sxs-lookup"><span data-stu-id="5f23e-131">Relationships</span></span>
<span data-ttu-id="5f23e-132">无</span><span class="sxs-lookup"><span data-stu-id="5f23e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f23e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f23e-133">JSON Representation</span></span>
<span data-ttu-id="5f23e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f23e-134">Here is a JSON representation of the resource.</span></span>
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



