---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d017c6b1bba7552bc2524f21cf5c102254b4dfcc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271476"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="1296c-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1296c-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

<span data-ttu-id="1296c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1296c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1296c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1296c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1296c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1296c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1296c-107">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="1296c-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="1296c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1296c-108">Properties</span></span>
|<span data-ttu-id="1296c-109">属性</span><span class="sxs-lookup"><span data-stu-id="1296c-109">Property</span></span>|<span data-ttu-id="1296c-110">类型</span><span class="sxs-lookup"><span data-stu-id="1296c-110">Type</span></span>|<span data-ttu-id="1296c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1296c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1296c-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="1296c-112">occurrenceDateTime</span></span>|<span data-ttu-id="1296c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1296c-113">DateTimeOffset</span></span>|<span data-ttu-id="1296c-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="1296c-114">Time when the history item occurred.</span></span>|
|<span data-ttu-id="1296c-115">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1296c-115">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="1296c-116">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1296c-116">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="1296c-117">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="1296c-117">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1296c-118">关系</span><span class="sxs-lookup"><span data-stu-id="1296c-118">Relationships</span></span>
<span data-ttu-id="1296c-119">无</span><span class="sxs-lookup"><span data-stu-id="1296c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1296c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1296c-120">JSON Representation</span></span>
<span data-ttu-id="1296c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1296c-121">Here is a JSON representation of the resource.</span></span>
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




