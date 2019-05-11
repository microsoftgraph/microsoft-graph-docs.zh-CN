---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9fbad683f193ffc6bce00fc29aa694422d2f494
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939810"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="07064-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="07064-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="07064-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07064-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07064-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07064-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07064-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="07064-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="07064-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="07064-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07064-108">属性</span><span class="sxs-lookup"><span data-stu-id="07064-108">Properties</span></span>
|<span data-ttu-id="07064-109">属性</span><span class="sxs-lookup"><span data-stu-id="07064-109">Property</span></span>|<span data-ttu-id="07064-110">类型</span><span class="sxs-lookup"><span data-stu-id="07064-110">Type</span></span>|<span data-ttu-id="07064-111">说明</span><span class="sxs-lookup"><span data-stu-id="07064-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07064-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="07064-112">occurrenceDateTime</span></span>|<span data-ttu-id="07064-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07064-113">DateTimeOffset</span></span>|<span data-ttu-id="07064-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="07064-114">Time when the history item occurred.</span></span> <span data-ttu-id="07064-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="07064-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="07064-116">关系</span><span class="sxs-lookup"><span data-stu-id="07064-116">Relationships</span></span>
<span data-ttu-id="07064-117">无</span><span class="sxs-lookup"><span data-stu-id="07064-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07064-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07064-118">JSON Representation</span></span>
<span data-ttu-id="07064-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07064-119">Here is a JSON representation of the resource.</span></span>
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




