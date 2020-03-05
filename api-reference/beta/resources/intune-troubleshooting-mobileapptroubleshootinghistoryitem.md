---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23760e335db70d011043647a0d5fd81354b0025e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523280"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="57aa0-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="57aa0-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="57aa0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="57aa0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57aa0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57aa0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57aa0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57aa0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57aa0-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="57aa0-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="57aa0-108">属性</span><span class="sxs-lookup"><span data-stu-id="57aa0-108">Properties</span></span>
|<span data-ttu-id="57aa0-109">属性</span><span class="sxs-lookup"><span data-stu-id="57aa0-109">Property</span></span>|<span data-ttu-id="57aa0-110">类型</span><span class="sxs-lookup"><span data-stu-id="57aa0-110">Type</span></span>|<span data-ttu-id="57aa0-111">说明</span><span class="sxs-lookup"><span data-stu-id="57aa0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57aa0-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="57aa0-112">occurrenceDateTime</span></span>|<span data-ttu-id="57aa0-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57aa0-113">DateTimeOffset</span></span>|<span data-ttu-id="57aa0-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="57aa0-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="57aa0-115">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="57aa0-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="57aa0-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="57aa0-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="57aa0-117">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="57aa0-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57aa0-118">关系</span><span class="sxs-lookup"><span data-stu-id="57aa0-118">Relationships</span></span>
<span data-ttu-id="57aa0-119">无</span><span class="sxs-lookup"><span data-stu-id="57aa0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57aa0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57aa0-120">JSON Representation</span></span>
<span data-ttu-id="57aa0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57aa0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
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



