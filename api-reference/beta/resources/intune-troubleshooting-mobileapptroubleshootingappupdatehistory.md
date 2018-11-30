---
title: mobileAppTroubleshootingAppUpdateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
ms.openlocfilehash: d546475f568c279137e411d546765fe828c43975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045903"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="b5a17-103">mobileAppTroubleshootingAppUpdateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5a17-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="b5a17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5a17-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5a17-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5a17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5a17-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5a17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5a17-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="b5a17-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="b5a17-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5a17-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5a17-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5a17-109">Properties</span></span>
|<span data-ttu-id="b5a17-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5a17-110">Property</span></span>|<span data-ttu-id="b5a17-111">类型</span><span class="sxs-lookup"><span data-stu-id="b5a17-111">Type</span></span>|<span data-ttu-id="b5a17-112">说明</span><span class="sxs-lookup"><span data-stu-id="b5a17-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a17-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="b5a17-113">occurrenceDateTime</span></span>|<span data-ttu-id="b5a17-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5a17-114">DateTimeOffset</span></span>|<span data-ttu-id="b5a17-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b5a17-115">Time when the history item occurred.</span></span> <span data-ttu-id="b5a17-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5a17-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5a17-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="b5a17-117">Relationships</span></span>
<span data-ttu-id="b5a17-118">无</span><span class="sxs-lookup"><span data-stu-id="b5a17-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5a17-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5a17-119">JSON Representation</span></span>
<span data-ttu-id="b5a17-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5a17-120">Here is a JSON representation of the resource.</span></span>
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





