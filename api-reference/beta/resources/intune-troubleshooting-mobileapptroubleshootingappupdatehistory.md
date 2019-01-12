---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c938aa30667f28e65285cfdb365f4b0eab55104a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922268"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="ec550-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec550-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="ec550-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ec550-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec550-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ec550-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec550-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ec550-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec550-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="ec550-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="ec550-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ec550-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec550-109">属性</span><span class="sxs-lookup"><span data-stu-id="ec550-109">Properties</span></span>
|<span data-ttu-id="ec550-110">属性</span><span class="sxs-lookup"><span data-stu-id="ec550-110">Property</span></span>|<span data-ttu-id="ec550-111">类型</span><span class="sxs-lookup"><span data-stu-id="ec550-111">Type</span></span>|<span data-ttu-id="ec550-112">说明</span><span class="sxs-lookup"><span data-stu-id="ec550-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec550-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ec550-113">occurrenceDateTime</span></span>|<span data-ttu-id="ec550-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec550-114">DateTimeOffset</span></span>|<span data-ttu-id="ec550-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="ec550-115">Time when the history item occurred.</span></span> <span data-ttu-id="ec550-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ec550-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec550-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="ec550-117">Relationships</span></span>
<span data-ttu-id="ec550-118">无</span><span class="sxs-lookup"><span data-stu-id="ec550-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ec550-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec550-119">JSON Representation</span></span>
<span data-ttu-id="ec550-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec550-120">Here is a JSON representation of the resource.</span></span>
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





