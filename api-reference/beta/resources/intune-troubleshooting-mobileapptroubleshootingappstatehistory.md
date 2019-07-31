---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d145212645283738d1248bd05c50b1f6658460f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967215"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="74f56-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="74f56-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="74f56-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74f56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f56-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74f56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f56-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="74f56-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="74f56-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="74f56-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74f56-108">属性</span><span class="sxs-lookup"><span data-stu-id="74f56-108">Properties</span></span>
|<span data-ttu-id="74f56-109">属性</span><span class="sxs-lookup"><span data-stu-id="74f56-109">Property</span></span>|<span data-ttu-id="74f56-110">类型</span><span class="sxs-lookup"><span data-stu-id="74f56-110">Type</span></span>|<span data-ttu-id="74f56-111">说明</span><span class="sxs-lookup"><span data-stu-id="74f56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f56-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="74f56-112">occurrenceDateTime</span></span>|<span data-ttu-id="74f56-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f56-113">DateTimeOffset</span></span>|<span data-ttu-id="74f56-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="74f56-114">Time when the history item occurred.</span></span> <span data-ttu-id="74f56-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="74f56-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="74f56-116">actionType</span><span class="sxs-lookup"><span data-stu-id="74f56-116">actionType</span></span>|[<span data-ttu-id="74f56-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="74f56-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="74f56-118">Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="74f56-118">Action type for Intune Application.</span></span> <span data-ttu-id="74f56-119">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="74f56-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="74f56-120">runState</span><span class="sxs-lookup"><span data-stu-id="74f56-120">runState</span></span>|[<span data-ttu-id="74f56-121">runState</span><span class="sxs-lookup"><span data-stu-id="74f56-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="74f56-122">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="74f56-122">Status of the item.</span></span> <span data-ttu-id="74f56-123">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="74f56-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="74f56-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="74f56-124">errorCode</span></span>|<span data-ttu-id="74f56-125">String</span><span class="sxs-lookup"><span data-stu-id="74f56-125">String</span></span>|<span data-ttu-id="74f56-126">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="74f56-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74f56-127">关系</span><span class="sxs-lookup"><span data-stu-id="74f56-127">Relationships</span></span>
<span data-ttu-id="74f56-128">无</span><span class="sxs-lookup"><span data-stu-id="74f56-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74f56-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74f56-129">JSON Representation</span></span>
<span data-ttu-id="74f56-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74f56-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```





