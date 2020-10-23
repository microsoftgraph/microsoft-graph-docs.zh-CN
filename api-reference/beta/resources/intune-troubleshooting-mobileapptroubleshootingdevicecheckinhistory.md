---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad778bef1b6a5a5d25316af98c31e138577e2c70
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732437"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="9b0c3-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b0c3-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

<span data-ttu-id="9b0c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b0c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b0c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b0c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b0c3-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9b0c3-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b0c3-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b0c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b0c3-109">Properties</span></span>
|<span data-ttu-id="9b0c3-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b0c3-110">Property</span></span>|<span data-ttu-id="9b0c3-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b0c3-111">Type</span></span>|<span data-ttu-id="9b0c3-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b0c3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b0c3-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="9b0c3-113">occurrenceDateTime</span></span>|<span data-ttu-id="9b0c3-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b0c3-114">DateTimeOffset</span></span>|<span data-ttu-id="9b0c3-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-115">Time when the history item occurred.</span></span> <span data-ttu-id="9b0c3-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b0c3-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="9b0c3-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9b0c3-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="9b0c3-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9b0c3-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="9b0c3-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="9b0c3-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b0c3-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b0c3-121">关系</span><span class="sxs-lookup"><span data-stu-id="9b0c3-121">Relationships</span></span>
<span data-ttu-id="9b0c3-122">无</span><span class="sxs-lookup"><span data-stu-id="9b0c3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b0c3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b0c3-123">JSON Representation</span></span>
<span data-ttu-id="9b0c3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b0c3-124">Here is a JSON representation of the resource.</span></span>
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





