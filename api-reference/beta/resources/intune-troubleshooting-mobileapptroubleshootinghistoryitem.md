---
title: mobileAppTroubleshootingHistoryItem 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
ms.openlocfilehash: 132039a0b6e457ebd2ca3e545f6f15dd4ad7ac58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329524"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="4ad43-103">mobileAppTroubleshootingHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ad43-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="4ad43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ad43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ad43-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ad43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ad43-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ad43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ad43-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="4ad43-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="4ad43-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ad43-108">Properties</span></span>
|<span data-ttu-id="4ad43-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ad43-109">Property</span></span>|<span data-ttu-id="4ad43-110">类型</span><span class="sxs-lookup"><span data-stu-id="4ad43-110">Type</span></span>|<span data-ttu-id="4ad43-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ad43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad43-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="4ad43-112">occurrenceDateTime</span></span>|<span data-ttu-id="4ad43-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ad43-113">DateTimeOffset</span></span>|<span data-ttu-id="4ad43-114">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4ad43-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ad43-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="4ad43-115">Relationships</span></span>
<span data-ttu-id="4ad43-116">无</span><span class="sxs-lookup"><span data-stu-id="4ad43-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ad43-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ad43-117">JSON Representation</span></span>
<span data-ttu-id="4ad43-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ad43-118">Here is a JSON representation of the resource.</span></span>
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





