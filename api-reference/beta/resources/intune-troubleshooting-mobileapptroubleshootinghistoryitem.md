---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 713bf06c65bd8d651e1d885d41876822d62eade1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947237"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="a8327-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8327-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="a8327-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8327-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8327-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8327-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8327-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8327-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="a8327-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="a8327-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8327-108">Properties</span></span>
|<span data-ttu-id="a8327-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8327-109">Property</span></span>|<span data-ttu-id="a8327-110">类型</span><span class="sxs-lookup"><span data-stu-id="a8327-110">Type</span></span>|<span data-ttu-id="a8327-111">Description</span><span class="sxs-lookup"><span data-stu-id="a8327-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8327-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="a8327-112">occurrenceDateTime</span></span>|<span data-ttu-id="a8327-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8327-113">DateTimeOffset</span></span>|<span data-ttu-id="a8327-114">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a8327-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8327-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="a8327-115">Relationships</span></span>
<span data-ttu-id="a8327-116">无</span><span class="sxs-lookup"><span data-stu-id="a8327-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8327-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8327-117">JSON Representation</span></span>
<span data-ttu-id="a8327-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8327-118">Here is a JSON representation of the resource.</span></span>
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





