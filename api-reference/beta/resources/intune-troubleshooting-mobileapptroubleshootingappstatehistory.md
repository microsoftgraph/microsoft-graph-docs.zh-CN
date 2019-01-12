---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a7cd7a67790dca8824b7e446b5add5304c6f0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917739"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="d5413-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5413-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="d5413-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5413-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5413-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5413-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5413-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5413-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5413-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="d5413-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="d5413-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5413-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5413-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5413-109">Properties</span></span>
|<span data-ttu-id="d5413-110">属性</span><span class="sxs-lookup"><span data-stu-id="d5413-110">Property</span></span>|<span data-ttu-id="d5413-111">类型</span><span class="sxs-lookup"><span data-stu-id="d5413-111">Type</span></span>|<span data-ttu-id="d5413-112">Description</span><span class="sxs-lookup"><span data-stu-id="d5413-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5413-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d5413-113">occurrenceDateTime</span></span>|<span data-ttu-id="d5413-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5413-114">DateTimeOffset</span></span>|<span data-ttu-id="d5413-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="d5413-115">Time when the history item occurred.</span></span> <span data-ttu-id="d5413-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5413-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d5413-117">actionType</span><span class="sxs-lookup"><span data-stu-id="d5413-117">actionType</span></span>|[<span data-ttu-id="d5413-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="d5413-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="d5413-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="d5413-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="d5413-120">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="d5413-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="d5413-121">runState</span><span class="sxs-lookup"><span data-stu-id="d5413-121">runState</span></span>|[<span data-ttu-id="d5413-122">runState</span><span class="sxs-lookup"><span data-stu-id="d5413-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d5413-123">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="d5413-123">Status of the item.</span></span> <span data-ttu-id="d5413-124">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="d5413-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="d5413-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5413-125">errorCode</span></span>|<span data-ttu-id="d5413-126">String</span><span class="sxs-lookup"><span data-stu-id="d5413-126">String</span></span>|<span data-ttu-id="d5413-127">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="d5413-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5413-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="d5413-128">Relationships</span></span>
<span data-ttu-id="d5413-129">无</span><span class="sxs-lookup"><span data-stu-id="d5413-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5413-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5413-130">JSON Representation</span></span>
<span data-ttu-id="d5413-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5413-131">Here is a JSON representation of the resource.</span></span>
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





