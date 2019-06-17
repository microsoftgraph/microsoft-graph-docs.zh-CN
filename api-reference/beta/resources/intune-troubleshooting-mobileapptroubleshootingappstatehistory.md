---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c3f3b466d234c1f49a44cab8170366d8203bd26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988081"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="aec1d-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="aec1d-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="aec1d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aec1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec1d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aec1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec1d-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="aec1d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="aec1d-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aec1d-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aec1d-108">属性</span><span class="sxs-lookup"><span data-stu-id="aec1d-108">Properties</span></span>
|<span data-ttu-id="aec1d-109">属性</span><span class="sxs-lookup"><span data-stu-id="aec1d-109">Property</span></span>|<span data-ttu-id="aec1d-110">类型</span><span class="sxs-lookup"><span data-stu-id="aec1d-110">Type</span></span>|<span data-ttu-id="aec1d-111">说明</span><span class="sxs-lookup"><span data-stu-id="aec1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec1d-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="aec1d-112">occurrenceDateTime</span></span>|<span data-ttu-id="aec1d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aec1d-113">DateTimeOffset</span></span>|<span data-ttu-id="aec1d-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="aec1d-114">Time when the history item occurred.</span></span> <span data-ttu-id="aec1d-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aec1d-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="aec1d-116">actionType</span><span class="sxs-lookup"><span data-stu-id="aec1d-116">actionType</span></span>|[<span data-ttu-id="aec1d-117">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="aec1d-117">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="aec1d-118">目标为的 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="aec1d-118">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="aec1d-119">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="aec1d-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="aec1d-120">runState</span><span class="sxs-lookup"><span data-stu-id="aec1d-120">runState</span></span>|[<span data-ttu-id="aec1d-121">runState</span><span class="sxs-lookup"><span data-stu-id="aec1d-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="aec1d-122">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="aec1d-122">Status of the item.</span></span> <span data-ttu-id="aec1d-123">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="aec1d-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="aec1d-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="aec1d-124">errorCode</span></span>|<span data-ttu-id="aec1d-125">String</span><span class="sxs-lookup"><span data-stu-id="aec1d-125">String</span></span>|<span data-ttu-id="aec1d-126">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="aec1d-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aec1d-127">关系</span><span class="sxs-lookup"><span data-stu-id="aec1d-127">Relationships</span></span>
<span data-ttu-id="aec1d-128">无</span><span class="sxs-lookup"><span data-stu-id="aec1d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aec1d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aec1d-129">JSON Representation</span></span>
<span data-ttu-id="aec1d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aec1d-130">Here is a JSON representation of the resource.</span></span>
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





