---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 606fe9dcf282dd75992f5a936aa5f49dfbb61dc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414205"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="e4c52-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4c52-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="e4c52-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e4c52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4c52-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4c52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4c52-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4c52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4c52-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e4c52-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e4c52-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e4c52-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e4c52-109">属性</span><span class="sxs-lookup"><span data-stu-id="e4c52-109">Properties</span></span>
|<span data-ttu-id="e4c52-110">属性</span><span class="sxs-lookup"><span data-stu-id="e4c52-110">Property</span></span>|<span data-ttu-id="e4c52-111">类型</span><span class="sxs-lookup"><span data-stu-id="e4c52-111">Type</span></span>|<span data-ttu-id="e4c52-112">说明</span><span class="sxs-lookup"><span data-stu-id="e4c52-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4c52-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e4c52-113">occurrenceDateTime</span></span>|<span data-ttu-id="e4c52-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4c52-114">DateTimeOffset</span></span>|<span data-ttu-id="e4c52-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e4c52-115">Time when the history item occurred.</span></span> <span data-ttu-id="e4c52-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e4c52-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4c52-117">关系</span><span class="sxs-lookup"><span data-stu-id="e4c52-117">Relationships</span></span>
<span data-ttu-id="e4c52-118">无</span><span class="sxs-lookup"><span data-stu-id="e4c52-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4c52-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4c52-119">JSON Representation</span></span>
<span data-ttu-id="e4c52-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4c52-120">Here is a JSON representation of the resource.</span></span>
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




