---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c30f3cb1f6eb4375da4112ca51c0b8298245a6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764416"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="c709e-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c709e-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="c709e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c709e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c709e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c709e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c709e-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="c709e-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="c709e-107">属性</span><span class="sxs-lookup"><span data-stu-id="c709e-107">Properties</span></span>
|<span data-ttu-id="c709e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c709e-108">Property</span></span>|<span data-ttu-id="c709e-109">类型</span><span class="sxs-lookup"><span data-stu-id="c709e-109">Type</span></span>|<span data-ttu-id="c709e-110">说明</span><span class="sxs-lookup"><span data-stu-id="c709e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c709e-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c709e-111">occurrenceDateTime</span></span>|<span data-ttu-id="c709e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c709e-112">DateTimeOffset</span></span>|<span data-ttu-id="c709e-113">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c709e-113">Time when the history item occurred.</span></span>|
|<span data-ttu-id="c709e-114">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c709e-114">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c709e-115">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c709e-115">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c709e-116">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="c709e-116">Object containing detailed information about the error and its remediation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c709e-117">关系</span><span class="sxs-lookup"><span data-stu-id="c709e-117">Relationships</span></span>
<span data-ttu-id="c709e-118">无</span><span class="sxs-lookup"><span data-stu-id="c709e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c709e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c709e-119">JSON Representation</span></span>
<span data-ttu-id="c709e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c709e-120">Here is a JSON representation of the resource.</span></span>
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



