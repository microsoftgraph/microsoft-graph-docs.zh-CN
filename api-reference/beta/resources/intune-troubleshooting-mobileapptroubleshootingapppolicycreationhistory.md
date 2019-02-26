---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a93b88f850e2fa220903362375774d8a6dded59c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160499"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="66fd5-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="66fd5-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="66fd5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66fd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66fd5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66fd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66fd5-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="66fd5-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="66fd5-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="66fd5-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66fd5-108">属性</span><span class="sxs-lookup"><span data-stu-id="66fd5-108">Properties</span></span>
|<span data-ttu-id="66fd5-109">属性</span><span class="sxs-lookup"><span data-stu-id="66fd5-109">Property</span></span>|<span data-ttu-id="66fd5-110">类型</span><span class="sxs-lookup"><span data-stu-id="66fd5-110">Type</span></span>|<span data-ttu-id="66fd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="66fd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fd5-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="66fd5-112">occurrenceDateTime</span></span>|<span data-ttu-id="66fd5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66fd5-113">DateTimeOffset</span></span>|<span data-ttu-id="66fd5-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="66fd5-114">Time when the history item occurred.</span></span> <span data-ttu-id="66fd5-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="66fd5-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="66fd5-116">runState</span><span class="sxs-lookup"><span data-stu-id="66fd5-116">runState</span></span>|[<span data-ttu-id="66fd5-117">runState</span><span class="sxs-lookup"><span data-stu-id="66fd5-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="66fd5-118">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="66fd5-118">Status of the item.</span></span> <span data-ttu-id="66fd5-119">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="66fd5-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="66fd5-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="66fd5-120">errorCode</span></span>|<span data-ttu-id="66fd5-121">String</span><span class="sxs-lookup"><span data-stu-id="66fd5-121">String</span></span>|<span data-ttu-id="66fd5-122">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="66fd5-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66fd5-123">关系</span><span class="sxs-lookup"><span data-stu-id="66fd5-123">Relationships</span></span>
<span data-ttu-id="66fd5-124">无</span><span class="sxs-lookup"><span data-stu-id="66fd5-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66fd5-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66fd5-125">JSON Representation</span></span>
<span data-ttu-id="66fd5-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66fd5-126">Here is a JSON representation of the resource.</span></span>
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




