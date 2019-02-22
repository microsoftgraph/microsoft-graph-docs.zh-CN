---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 646fb576e8590d9f5c58b2b67c6fd3612cf689f0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171216"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="25533-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="25533-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="25533-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25533-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25533-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25533-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25533-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="25533-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="25533-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25533-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25533-108">属性</span><span class="sxs-lookup"><span data-stu-id="25533-108">Properties</span></span>
|<span data-ttu-id="25533-109">属性</span><span class="sxs-lookup"><span data-stu-id="25533-109">Property</span></span>|<span data-ttu-id="25533-110">类型</span><span class="sxs-lookup"><span data-stu-id="25533-110">Type</span></span>|<span data-ttu-id="25533-111">说明</span><span class="sxs-lookup"><span data-stu-id="25533-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25533-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="25533-112">occurrenceDateTime</span></span>|<span data-ttu-id="25533-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25533-113">DateTimeOffset</span></span>|<span data-ttu-id="25533-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="25533-114">Time when the history item occurred.</span></span> <span data-ttu-id="25533-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="25533-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="25533-116">关系</span><span class="sxs-lookup"><span data-stu-id="25533-116">Relationships</span></span>
<span data-ttu-id="25533-117">无</span><span class="sxs-lookup"><span data-stu-id="25533-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25533-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25533-118">JSON Representation</span></span>
<span data-ttu-id="25533-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25533-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```




