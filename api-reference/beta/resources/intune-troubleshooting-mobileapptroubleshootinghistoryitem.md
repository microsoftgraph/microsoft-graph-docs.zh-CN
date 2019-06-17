---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7158855510df58b56fc63b467ec721250ca502d3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983580"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="44adb-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="44adb-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="44adb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44adb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44adb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44adb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44adb-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="44adb-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="44adb-107">属性</span><span class="sxs-lookup"><span data-stu-id="44adb-107">Properties</span></span>
|<span data-ttu-id="44adb-108">属性</span><span class="sxs-lookup"><span data-stu-id="44adb-108">Property</span></span>|<span data-ttu-id="44adb-109">类型</span><span class="sxs-lookup"><span data-stu-id="44adb-109">Type</span></span>|<span data-ttu-id="44adb-110">说明</span><span class="sxs-lookup"><span data-stu-id="44adb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44adb-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="44adb-111">occurrenceDateTime</span></span>|<span data-ttu-id="44adb-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44adb-112">DateTimeOffset</span></span>|<span data-ttu-id="44adb-113">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="44adb-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44adb-114">关系</span><span class="sxs-lookup"><span data-stu-id="44adb-114">Relationships</span></span>
<span data-ttu-id="44adb-115">无</span><span class="sxs-lookup"><span data-stu-id="44adb-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44adb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44adb-116">JSON Representation</span></span>
<span data-ttu-id="44adb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44adb-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





