---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce8cf0290830a22ae1f074f9b177535cd2b20e09
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939831"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="c1c64-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1c64-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="c1c64-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1c64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1c64-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1c64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c64-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="c1c64-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c1c64-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1c64-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1c64-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1c64-108">Properties</span></span>
|<span data-ttu-id="c1c64-109">属性</span><span class="sxs-lookup"><span data-stu-id="c1c64-109">Property</span></span>|<span data-ttu-id="c1c64-110">类型</span><span class="sxs-lookup"><span data-stu-id="c1c64-110">Type</span></span>|<span data-ttu-id="c1c64-111">说明</span><span class="sxs-lookup"><span data-stu-id="c1c64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c64-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c1c64-112">occurrenceDateTime</span></span>|<span data-ttu-id="c1c64-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1c64-113">DateTimeOffset</span></span>|<span data-ttu-id="c1c64-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="c1c64-114">Time when the history item occurred.</span></span> <span data-ttu-id="c1c64-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1c64-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c1c64-116">runState</span><span class="sxs-lookup"><span data-stu-id="c1c64-116">runState</span></span>|[<span data-ttu-id="c1c64-117">runState</span><span class="sxs-lookup"><span data-stu-id="c1c64-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c1c64-118">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="c1c64-118">Status of the item.</span></span> <span data-ttu-id="c1c64-119">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="c1c64-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="c1c64-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="c1c64-120">errorCode</span></span>|<span data-ttu-id="c1c64-121">String</span><span class="sxs-lookup"><span data-stu-id="c1c64-121">String</span></span>|<span data-ttu-id="c1c64-122">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="c1c64-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c64-123">关系</span><span class="sxs-lookup"><span data-stu-id="c1c64-123">Relationships</span></span>
<span data-ttu-id="c1c64-124">无</span><span class="sxs-lookup"><span data-stu-id="c1c64-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c64-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1c64-125">JSON Representation</span></span>
<span data-ttu-id="c1c64-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1c64-126">Here is a JSON representation of the resource.</span></span>
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




