---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
ms.openlocfilehash: b8050a6d99eeca008477059c9d39a40dbda906a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047577"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="beeb4-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="beeb4-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="beeb4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="beeb4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beeb4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="beeb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beeb4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="beeb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beeb4-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="beeb4-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="beeb4-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeb4-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="beeb4-109">属性</span><span class="sxs-lookup"><span data-stu-id="beeb4-109">Properties</span></span>
|<span data-ttu-id="beeb4-110">属性</span><span class="sxs-lookup"><span data-stu-id="beeb4-110">Property</span></span>|<span data-ttu-id="beeb4-111">类型</span><span class="sxs-lookup"><span data-stu-id="beeb4-111">Type</span></span>|<span data-ttu-id="beeb4-112">说明</span><span class="sxs-lookup"><span data-stu-id="beeb4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beeb4-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="beeb4-113">occurrenceDateTime</span></span>|<span data-ttu-id="beeb4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beeb4-114">DateTimeOffset</span></span>|<span data-ttu-id="beeb4-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="beeb4-115">Time when the history item occurred.</span></span> <span data-ttu-id="beeb4-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="beeb4-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="beeb4-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="beeb4-117">Relationships</span></span>
<span data-ttu-id="beeb4-118">无</span><span class="sxs-lookup"><span data-stu-id="beeb4-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="beeb4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="beeb4-119">JSON Representation</span></span>
<span data-ttu-id="beeb4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="beeb4-120">Here is a JSON representation of the resource.</span></span>
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





