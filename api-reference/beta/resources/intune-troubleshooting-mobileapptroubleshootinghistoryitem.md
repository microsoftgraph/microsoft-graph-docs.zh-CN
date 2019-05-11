---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e63de7a150f36529237aac6f5f0794c8407e13e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938672"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="6ff43-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ff43-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="6ff43-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ff43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff43-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ff43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff43-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="6ff43-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="6ff43-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ff43-107">Properties</span></span>
|<span data-ttu-id="6ff43-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ff43-108">Property</span></span>|<span data-ttu-id="6ff43-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ff43-109">Type</span></span>|<span data-ttu-id="6ff43-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ff43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff43-111">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="6ff43-111">occurrenceDateTime</span></span>|<span data-ttu-id="6ff43-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ff43-112">DateTimeOffset</span></span>|<span data-ttu-id="6ff43-113">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="6ff43-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff43-114">关系</span><span class="sxs-lookup"><span data-stu-id="6ff43-114">Relationships</span></span>
<span data-ttu-id="6ff43-115">无</span><span class="sxs-lookup"><span data-stu-id="6ff43-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff43-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ff43-116">JSON Representation</span></span>
<span data-ttu-id="6ff43-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ff43-117">Here is a JSON representation of the resource.</span></span>
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




