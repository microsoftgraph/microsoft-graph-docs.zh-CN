---
title: mobileAppTroubleshootingAppStateHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
ms.openlocfilehash: ebe38b852c6c6926b69e75379bc1a029ade0bb98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332156"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="38604-103">mobileAppTroubleshootingAppStateHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="38604-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="38604-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38604-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38604-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38604-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38604-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38604-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38604-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="38604-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="38604-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="38604-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38604-109">属性</span><span class="sxs-lookup"><span data-stu-id="38604-109">Properties</span></span>
|<span data-ttu-id="38604-110">属性</span><span class="sxs-lookup"><span data-stu-id="38604-110">Property</span></span>|<span data-ttu-id="38604-111">类型</span><span class="sxs-lookup"><span data-stu-id="38604-111">Type</span></span>|<span data-ttu-id="38604-112">说明</span><span class="sxs-lookup"><span data-stu-id="38604-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38604-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="38604-113">occurrenceDateTime</span></span>|<span data-ttu-id="38604-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38604-114">DateTimeOffset</span></span>|<span data-ttu-id="38604-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="38604-115">Time when the history item occurred.</span></span> <span data-ttu-id="38604-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="38604-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="38604-117">actionType</span><span class="sxs-lookup"><span data-stu-id="38604-117">actionType</span></span>|[<span data-ttu-id="38604-118">mobileAppActionType</span><span class="sxs-lookup"><span data-stu-id="38604-118">mobileAppActionType</span></span>](../resources/intune-troubleshooting-mobileappactiontype.md)|<span data-ttu-id="38604-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="38604-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="38604-120">可取值为：`unknown`、`installCommandSent`、`installed`、`uninstalled`、`userRequestedInstall`。</span><span class="sxs-lookup"><span data-stu-id="38604-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="38604-121">runState</span><span class="sxs-lookup"><span data-stu-id="38604-121">runState</span></span>|[<span data-ttu-id="38604-122">runState</span><span class="sxs-lookup"><span data-stu-id="38604-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="38604-123">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="38604-123">Status of the item.</span></span> <span data-ttu-id="38604-124">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="38604-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="38604-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="38604-125">errorCode</span></span>|<span data-ttu-id="38604-126">String</span><span class="sxs-lookup"><span data-stu-id="38604-126">String</span></span>|<span data-ttu-id="38604-127">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="38604-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38604-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="38604-128">Relationships</span></span>
<span data-ttu-id="38604-129">无</span><span class="sxs-lookup"><span data-stu-id="38604-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38604-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38604-130">JSON Representation</span></span>
<span data-ttu-id="38604-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38604-131">Here is a JSON representation of the resource.</span></span>
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





