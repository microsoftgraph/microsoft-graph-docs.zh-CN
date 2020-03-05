---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7712a9f75317709cd30a84e2730c8dca9466b111
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523294"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="b2a2d-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2a2d-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="b2a2d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b2a2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2a2d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2a2d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2a2d-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="b2a2d-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2a2d-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2a2d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2a2d-109">Properties</span></span>
|<span data-ttu-id="b2a2d-110">属性</span><span class="sxs-lookup"><span data-stu-id="b2a2d-110">Property</span></span>|<span data-ttu-id="b2a2d-111">类型</span><span class="sxs-lookup"><span data-stu-id="b2a2d-111">Type</span></span>|<span data-ttu-id="b2a2d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2a2d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a2d-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="b2a2d-113">occurrenceDateTime</span></span>|<span data-ttu-id="b2a2d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2a2d-114">DateTimeOffset</span></span>|<span data-ttu-id="b2a2d-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-115">Time when the history item occurred.</span></span> <span data-ttu-id="b2a2d-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2a2d-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="b2a2d-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b2a2d-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="b2a2d-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b2a2d-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="b2a2d-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="b2a2d-120">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2a2d-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2a2d-121">关系</span><span class="sxs-lookup"><span data-stu-id="b2a2d-121">Relationships</span></span>
<span data-ttu-id="b2a2d-122">无</span><span class="sxs-lookup"><span data-stu-id="b2a2d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2a2d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2a2d-123">JSON Representation</span></span>
<span data-ttu-id="b2a2d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2a2d-124">Here is a JSON representation of the resource.</span></span>
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



