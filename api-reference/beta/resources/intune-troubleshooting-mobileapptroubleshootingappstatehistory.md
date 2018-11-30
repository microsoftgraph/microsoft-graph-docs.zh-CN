---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
ms.openlocfilehash: 415d018d3650819bce8defe651af8df77e3c6032
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043844"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="488fa-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="488fa-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="488fa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="488fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="488fa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="488fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="488fa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="488fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="488fa-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="488fa-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="488fa-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="488fa-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="488fa-109">属性</span><span class="sxs-lookup"><span data-stu-id="488fa-109">Properties</span></span>
|<span data-ttu-id="488fa-110">属性</span><span class="sxs-lookup"><span data-stu-id="488fa-110">Property</span></span>|<span data-ttu-id="488fa-111">类型</span><span class="sxs-lookup"><span data-stu-id="488fa-111">Type</span></span>|<span data-ttu-id="488fa-112">说明</span><span class="sxs-lookup"><span data-stu-id="488fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="488fa-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="488fa-113">occurrenceDateTime</span></span>|<span data-ttu-id="488fa-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="488fa-114">DateTimeOffset</span></span>|<span data-ttu-id="488fa-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="488fa-115">Time when the history item occurred.</span></span> <span data-ttu-id="488fa-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="488fa-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="488fa-117">actionType</span><span class="sxs-lookup"><span data-stu-id="488fa-117">actionType</span></span>|[<span data-ttu-id="488fa-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="488fa-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="488fa-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="488fa-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="488fa-120">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="488fa-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="488fa-121">runState</span><span class="sxs-lookup"><span data-stu-id="488fa-121">runState</span></span>|[<span data-ttu-id="488fa-122">runState</span><span class="sxs-lookup"><span data-stu-id="488fa-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="488fa-123">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="488fa-123">Status of the item.</span></span> <span data-ttu-id="488fa-124">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="488fa-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="488fa-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="488fa-125">errorCode</span></span>|<span data-ttu-id="488fa-126">String</span><span class="sxs-lookup"><span data-stu-id="488fa-126">String</span></span>|<span data-ttu-id="488fa-127">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="488fa-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="488fa-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="488fa-128">Relationships</span></span>
<span data-ttu-id="488fa-129">无</span><span class="sxs-lookup"><span data-stu-id="488fa-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="488fa-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="488fa-130">JSON Representation</span></span>
<span data-ttu-id="488fa-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="488fa-131">Here is a JSON representation of the resource.</span></span>
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





