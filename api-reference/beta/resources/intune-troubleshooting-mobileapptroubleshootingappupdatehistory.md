---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8260479d17dfc2e0769cb6980158bdfe54b808d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993215"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="34d9a-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="34d9a-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="34d9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34d9a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34d9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34d9a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34d9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34d9a-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="34d9a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="34d9a-108">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="34d9a-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34d9a-109">属性</span><span class="sxs-lookup"><span data-stu-id="34d9a-109">Properties</span></span>
|<span data-ttu-id="34d9a-110">属性</span><span class="sxs-lookup"><span data-stu-id="34d9a-110">Property</span></span>|<span data-ttu-id="34d9a-111">类型</span><span class="sxs-lookup"><span data-stu-id="34d9a-111">Type</span></span>|<span data-ttu-id="34d9a-112">说明</span><span class="sxs-lookup"><span data-stu-id="34d9a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d9a-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="34d9a-113">occurrenceDateTime</span></span>|<span data-ttu-id="34d9a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34d9a-114">DateTimeOffset</span></span>|<span data-ttu-id="34d9a-115">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="34d9a-115">Time when the history item occurred.</span></span> <span data-ttu-id="34d9a-116">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="34d9a-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="34d9a-117">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="34d9a-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="34d9a-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="34d9a-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="34d9a-119">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="34d9a-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="34d9a-120">继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="34d9a-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="34d9a-121">关系</span><span class="sxs-lookup"><span data-stu-id="34d9a-121">Relationships</span></span>
<span data-ttu-id="34d9a-122">无</span><span class="sxs-lookup"><span data-stu-id="34d9a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34d9a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34d9a-123">JSON Representation</span></span>
<span data-ttu-id="34d9a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34d9a-124">Here is a JSON representation of the resource.</span></span>
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






