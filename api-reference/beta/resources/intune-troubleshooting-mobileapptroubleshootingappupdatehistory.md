---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eadbec77e95dd90fd9ef819e468241bf8ef5c9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153639"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="89f69-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="89f69-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="89f69-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89f69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89f69-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f69-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="89f69-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="89f69-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="89f69-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89f69-108">属性</span><span class="sxs-lookup"><span data-stu-id="89f69-108">Properties</span></span>
|<span data-ttu-id="89f69-109">属性</span><span class="sxs-lookup"><span data-stu-id="89f69-109">Property</span></span>|<span data-ttu-id="89f69-110">类型</span><span class="sxs-lookup"><span data-stu-id="89f69-110">Type</span></span>|<span data-ttu-id="89f69-111">说明</span><span class="sxs-lookup"><span data-stu-id="89f69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f69-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="89f69-112">occurrenceDateTime</span></span>|<span data-ttu-id="89f69-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f69-113">DateTimeOffset</span></span>|<span data-ttu-id="89f69-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="89f69-114">Time when the history item occurred.</span></span> <span data-ttu-id="89f69-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="89f69-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f69-116">关系</span><span class="sxs-lookup"><span data-stu-id="89f69-116">Relationships</span></span>
<span data-ttu-id="89f69-117">无</span><span class="sxs-lookup"><span data-stu-id="89f69-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f69-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89f69-118">JSON Representation</span></span>
<span data-ttu-id="89f69-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89f69-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




