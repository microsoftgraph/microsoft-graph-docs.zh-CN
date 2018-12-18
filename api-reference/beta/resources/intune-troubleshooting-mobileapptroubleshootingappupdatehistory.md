---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
ms.openlocfilehash: 5f5775ac25c6bfce283bc67a195393f0cbe9ab75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312101"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="e704a-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="e704a-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="e704a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e704a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e704a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e704a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e704a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e704a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e704a-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="e704a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="e704a-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e704a-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e704a-109">属性</span><span class="sxs-lookup"><span data-stu-id="e704a-109">Properties</span></span>
|<span data-ttu-id="e704a-110">属性</span><span class="sxs-lookup"><span data-stu-id="e704a-110">Property</span></span>|<span data-ttu-id="e704a-111">类型</span><span class="sxs-lookup"><span data-stu-id="e704a-111">Type</span></span>|<span data-ttu-id="e704a-112">说明</span><span class="sxs-lookup"><span data-stu-id="e704a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e704a-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e704a-113">occurrenceDateTime</span></span>|<span data-ttu-id="e704a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e704a-114">DateTimeOffset</span></span>|<span data-ttu-id="e704a-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e704a-115">Time when the history item occurred.</span></span> <span data-ttu-id="e704a-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e704a-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e704a-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="e704a-117">Relationships</span></span>
<span data-ttu-id="e704a-118">无</span><span class="sxs-lookup"><span data-stu-id="e704a-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e704a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e704a-119">JSON Representation</span></span>
<span data-ttu-id="e704a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e704a-120">Here is a JSON representation of the resource.</span></span>
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





