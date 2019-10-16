---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2993967e1340ebb29e0a794f8204f75c5d431de0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525215"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="aee07-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="aee07-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="aee07-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aee07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aee07-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aee07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee07-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="aee07-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="aee07-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aee07-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aee07-108">属性</span><span class="sxs-lookup"><span data-stu-id="aee07-108">Properties</span></span>
|<span data-ttu-id="aee07-109">属性</span><span class="sxs-lookup"><span data-stu-id="aee07-109">Property</span></span>|<span data-ttu-id="aee07-110">类型</span><span class="sxs-lookup"><span data-stu-id="aee07-110">Type</span></span>|<span data-ttu-id="aee07-111">说明</span><span class="sxs-lookup"><span data-stu-id="aee07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee07-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="aee07-112">occurrenceDateTime</span></span>|<span data-ttu-id="aee07-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee07-113">DateTimeOffset</span></span>|<span data-ttu-id="aee07-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="aee07-114">Time when the history item occurred.</span></span> <span data-ttu-id="aee07-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="aee07-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="aee07-116">runState</span><span class="sxs-lookup"><span data-stu-id="aee07-116">runState</span></span>|[<span data-ttu-id="aee07-117">runState</span><span class="sxs-lookup"><span data-stu-id="aee07-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="aee07-118">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="aee07-118">Status of the item.</span></span> <span data-ttu-id="aee07-119">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="aee07-119">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="aee07-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="aee07-120">errorCode</span></span>|<span data-ttu-id="aee07-121">String</span><span class="sxs-lookup"><span data-stu-id="aee07-121">String</span></span>|<span data-ttu-id="aee07-122">失败的错误代码，如果没有失败，则为空。</span><span class="sxs-lookup"><span data-stu-id="aee07-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aee07-123">关系</span><span class="sxs-lookup"><span data-stu-id="aee07-123">Relationships</span></span>
<span data-ttu-id="aee07-124">无</span><span class="sxs-lookup"><span data-stu-id="aee07-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aee07-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aee07-125">JSON Representation</span></span>
<span data-ttu-id="aee07-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aee07-126">Here is a JSON representation of the resource.</span></span>
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



