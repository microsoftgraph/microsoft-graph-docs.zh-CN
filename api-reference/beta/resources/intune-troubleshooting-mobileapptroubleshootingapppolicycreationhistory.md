---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 416a5c7171a03db48d0b349a2a6415a940e5b798
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988067"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="f7d8a-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7d8a-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="f7d8a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7d8a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d8a-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="f7d8a-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f7d8a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7d8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7d8a-108">Properties</span></span>
|<span data-ttu-id="f7d8a-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7d8a-109">Property</span></span>|<span data-ttu-id="f7d8a-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7d8a-110">Type</span></span>|<span data-ttu-id="f7d8a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7d8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d8a-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="f7d8a-112">occurrenceDateTime</span></span>|<span data-ttu-id="f7d8a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7d8a-113">DateTimeOffset</span></span>|<span data-ttu-id="f7d8a-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-114">Time when the history item occurred.</span></span> <span data-ttu-id="f7d8a-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f7d8a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f7d8a-116">runState</span><span class="sxs-lookup"><span data-stu-id="f7d8a-116">runState</span></span>|[<span data-ttu-id="f7d8a-117">runState</span><span class="sxs-lookup"><span data-stu-id="f7d8a-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f7d8a-118">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-118">Status of the item.</span></span> <span data-ttu-id="f7d8a-119">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="f7d8a-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="f7d8a-120">errorCode</span></span>|<span data-ttu-id="f7d8a-121">String</span><span class="sxs-lookup"><span data-stu-id="f7d8a-121">String</span></span>|<span data-ttu-id="f7d8a-122">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d8a-123">关系</span><span class="sxs-lookup"><span data-stu-id="f7d8a-123">Relationships</span></span>
<span data-ttu-id="f7d8a-124">无</span><span class="sxs-lookup"><span data-stu-id="f7d8a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7d8a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7d8a-125">JSON Representation</span></span>
<span data-ttu-id="f7d8a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d8a-126">Here is a JSON representation of the resource.</span></span>
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





