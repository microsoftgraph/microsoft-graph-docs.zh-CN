---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89794800d46f91221d6232f5219e57e5eb7db2c5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287569"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="95030-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="95030-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

<span data-ttu-id="95030-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95030-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95030-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95030-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95030-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95030-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95030-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="95030-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="95030-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="95030-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95030-109">属性</span><span class="sxs-lookup"><span data-stu-id="95030-109">Properties</span></span>
|<span data-ttu-id="95030-110">属性</span><span class="sxs-lookup"><span data-stu-id="95030-110">Property</span></span>|<span data-ttu-id="95030-111">类型</span><span class="sxs-lookup"><span data-stu-id="95030-111">Type</span></span>|<span data-ttu-id="95030-112">Description</span><span class="sxs-lookup"><span data-stu-id="95030-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95030-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="95030-113">occurrenceDateTime</span></span>|<span data-ttu-id="95030-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95030-114">DateTimeOffset</span></span>|<span data-ttu-id="95030-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="95030-115">Time when the history item occurred.</span></span> <span data-ttu-id="95030-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="95030-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="95030-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="95030-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="95030-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="95030-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="95030-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="95030-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="95030-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="95030-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="95030-121">关系</span><span class="sxs-lookup"><span data-stu-id="95030-121">Relationships</span></span>
<span data-ttu-id="95030-122">无</span><span class="sxs-lookup"><span data-stu-id="95030-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95030-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95030-123">JSON Representation</span></span>
<span data-ttu-id="95030-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95030-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
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
  }
}
```




