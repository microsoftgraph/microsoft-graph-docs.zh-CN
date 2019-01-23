---
title: mobileAppTroubleshootingDeviceCheckinHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43816929fd01be56b7487e3c0101ca08c928ac85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410166"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="5462b-103">mobileAppTroubleshootingDeviceCheckinHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5462b-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="5462b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5462b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5462b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5462b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5462b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5462b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5462b-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="5462b-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5462b-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5462b-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5462b-109">属性</span><span class="sxs-lookup"><span data-stu-id="5462b-109">Properties</span></span>
|<span data-ttu-id="5462b-110">属性</span><span class="sxs-lookup"><span data-stu-id="5462b-110">Property</span></span>|<span data-ttu-id="5462b-111">类型</span><span class="sxs-lookup"><span data-stu-id="5462b-111">Type</span></span>|<span data-ttu-id="5462b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5462b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5462b-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5462b-113">occurrenceDateTime</span></span>|<span data-ttu-id="5462b-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5462b-114">DateTimeOffset</span></span>|<span data-ttu-id="5462b-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="5462b-115">Time when the history item occurred.</span></span> <span data-ttu-id="5462b-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5462b-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5462b-117">关系</span><span class="sxs-lookup"><span data-stu-id="5462b-117">Relationships</span></span>
<span data-ttu-id="5462b-118">无</span><span class="sxs-lookup"><span data-stu-id="5462b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5462b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5462b-119">JSON Representation</span></span>
<span data-ttu-id="5462b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5462b-120">Here is a JSON representation of the resource.</span></span>
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




