---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3fb483a0a500673c607344d35d38fa651711579e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764444"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="c5ea7-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5ea7-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="c5ea7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5ea7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5ea7-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c5ea7-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5ea7-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5ea7-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5ea7-108">Properties</span></span>
|<span data-ttu-id="c5ea7-109">属性</span><span class="sxs-lookup"><span data-stu-id="c5ea7-109">Property</span></span>|<span data-ttu-id="c5ea7-110">类型</span><span class="sxs-lookup"><span data-stu-id="c5ea7-110">Type</span></span>|<span data-ttu-id="c5ea7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5ea7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ea7-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ea7-112">occurrenceDateTime</span></span>|<span data-ttu-id="c5ea7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ea7-113">DateTimeOffset</span></span>|<span data-ttu-id="c5ea7-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-114">Time when the history item occurred.</span></span> <span data-ttu-id="c5ea7-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5ea7-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c5ea7-116">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c5ea7-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c5ea7-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c5ea7-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c5ea7-118">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c5ea7-119">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5ea7-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5ea7-120">关系</span><span class="sxs-lookup"><span data-stu-id="c5ea7-120">Relationships</span></span>
<span data-ttu-id="c5ea7-121">无</span><span class="sxs-lookup"><span data-stu-id="c5ea7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5ea7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5ea7-122">JSON Representation</span></span>
<span data-ttu-id="c5ea7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5ea7-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
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



