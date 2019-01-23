---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57e10fcabc0aa3def07872c0e520f09c6ee90fc3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411237"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="394a0-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="394a0-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="394a0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="394a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="394a0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="394a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="394a0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="394a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="394a0-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="394a0-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="394a0-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="394a0-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="394a0-109">属性</span><span class="sxs-lookup"><span data-stu-id="394a0-109">Properties</span></span>
|<span data-ttu-id="394a0-110">属性</span><span class="sxs-lookup"><span data-stu-id="394a0-110">Property</span></span>|<span data-ttu-id="394a0-111">类型</span><span class="sxs-lookup"><span data-stu-id="394a0-111">Type</span></span>|<span data-ttu-id="394a0-112">说明</span><span class="sxs-lookup"><span data-stu-id="394a0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="394a0-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="394a0-113">occurrenceDateTime</span></span>|<span data-ttu-id="394a0-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="394a0-114">DateTimeOffset</span></span>|<span data-ttu-id="394a0-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="394a0-115">Time when the history item occurred.</span></span> <span data-ttu-id="394a0-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="394a0-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="394a0-117">actionType</span><span class="sxs-lookup"><span data-stu-id="394a0-117">actionType</span></span>|[<span data-ttu-id="394a0-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="394a0-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="394a0-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="394a0-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="394a0-120">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="394a0-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="394a0-121">runState</span><span class="sxs-lookup"><span data-stu-id="394a0-121">runState</span></span>|[<span data-ttu-id="394a0-122">runState</span><span class="sxs-lookup"><span data-stu-id="394a0-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="394a0-123">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="394a0-123">Status of the item.</span></span> <span data-ttu-id="394a0-124">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="394a0-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="394a0-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="394a0-125">errorCode</span></span>|<span data-ttu-id="394a0-126">String</span><span class="sxs-lookup"><span data-stu-id="394a0-126">String</span></span>|<span data-ttu-id="394a0-127">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="394a0-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="394a0-128">关系</span><span class="sxs-lookup"><span data-stu-id="394a0-128">Relationships</span></span>
<span data-ttu-id="394a0-129">无</span><span class="sxs-lookup"><span data-stu-id="394a0-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="394a0-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="394a0-130">JSON Representation</span></span>
<span data-ttu-id="394a0-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="394a0-131">Here is a JSON representation of the resource.</span></span>
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




