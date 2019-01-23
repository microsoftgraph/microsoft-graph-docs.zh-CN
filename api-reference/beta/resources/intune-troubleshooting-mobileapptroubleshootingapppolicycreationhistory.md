---
title: mobileAppTroubleshootingAppPolicyCreationHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e81f7f39cac934a89cf06d77fbcb80581267097b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394556"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="5e2c7-103">mobileAppTroubleshootingAppPolicyCreationHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e2c7-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="5e2c7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e2c7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e2c7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e2c7-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5e2c7-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5e2c7-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e2c7-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e2c7-109">Properties</span></span>
|<span data-ttu-id="5e2c7-110">属性</span><span class="sxs-lookup"><span data-stu-id="5e2c7-110">Property</span></span>|<span data-ttu-id="5e2c7-111">类型</span><span class="sxs-lookup"><span data-stu-id="5e2c7-111">Type</span></span>|<span data-ttu-id="5e2c7-112">说明</span><span class="sxs-lookup"><span data-stu-id="5e2c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2c7-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5e2c7-113">occurrenceDateTime</span></span>|<span data-ttu-id="5e2c7-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e2c7-114">DateTimeOffset</span></span>|<span data-ttu-id="5e2c7-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-115">Time when the history item occurred.</span></span> <span data-ttu-id="5e2c7-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5e2c7-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5e2c7-117">runState</span><span class="sxs-lookup"><span data-stu-id="5e2c7-117">runState</span></span>|[<span data-ttu-id="5e2c7-118">runState</span><span class="sxs-lookup"><span data-stu-id="5e2c7-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5e2c7-119">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-119">Status of the item.</span></span> <span data-ttu-id="5e2c7-120">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5e2c7-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="5e2c7-121">errorCode</span></span>|<span data-ttu-id="5e2c7-122">String</span><span class="sxs-lookup"><span data-stu-id="5e2c7-122">String</span></span>|<span data-ttu-id="5e2c7-123">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e2c7-124">关系</span><span class="sxs-lookup"><span data-stu-id="5e2c7-124">Relationships</span></span>
<span data-ttu-id="5e2c7-125">无</span><span class="sxs-lookup"><span data-stu-id="5e2c7-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e2c7-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e2c7-126">JSON Representation</span></span>
<span data-ttu-id="5e2c7-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e2c7-127">Here is a JSON representation of the resource.</span></span>
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




