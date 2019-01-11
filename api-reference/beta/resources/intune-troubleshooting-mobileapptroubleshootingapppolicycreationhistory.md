---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd7880a6d931fafda46ab4adf0668835438ddcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870103"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="a67f1-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="a67f1-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="a67f1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a67f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a67f1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a67f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a67f1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a67f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a67f1-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="a67f1-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="a67f1-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a67f1-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a67f1-109">属性</span><span class="sxs-lookup"><span data-stu-id="a67f1-109">Properties</span></span>
|<span data-ttu-id="a67f1-110">属性</span><span class="sxs-lookup"><span data-stu-id="a67f1-110">Property</span></span>|<span data-ttu-id="a67f1-111">类型</span><span class="sxs-lookup"><span data-stu-id="a67f1-111">Type</span></span>|<span data-ttu-id="a67f1-112">Description</span><span class="sxs-lookup"><span data-stu-id="a67f1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a67f1-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="a67f1-113">occurrenceDateTime</span></span>|<span data-ttu-id="a67f1-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a67f1-114">DateTimeOffset</span></span>|<span data-ttu-id="a67f1-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a67f1-115">Time when the history item occurred.</span></span> <span data-ttu-id="a67f1-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a67f1-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="a67f1-117">runState</span><span class="sxs-lookup"><span data-stu-id="a67f1-117">runState</span></span>|[<span data-ttu-id="a67f1-118">runState</span><span class="sxs-lookup"><span data-stu-id="a67f1-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a67f1-119">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="a67f1-119">Status of the item.</span></span> <span data-ttu-id="a67f1-120">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="a67f1-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="a67f1-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="a67f1-121">errorCode</span></span>|<span data-ttu-id="a67f1-122">String</span><span class="sxs-lookup"><span data-stu-id="a67f1-122">String</span></span>|<span data-ttu-id="a67f1-123">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="a67f1-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a67f1-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="a67f1-124">Relationships</span></span>
<span data-ttu-id="a67f1-125">无</span><span class="sxs-lookup"><span data-stu-id="a67f1-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a67f1-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a67f1-126">JSON Representation</span></span>
<span data-ttu-id="a67f1-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a67f1-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```





