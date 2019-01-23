---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402963"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="05102-103">mobileAppTroubleshootingAppTargetHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="05102-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="05102-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="05102-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05102-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05102-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05102-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05102-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05102-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="05102-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="05102-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="05102-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05102-109">属性</span><span class="sxs-lookup"><span data-stu-id="05102-109">Properties</span></span>
|<span data-ttu-id="05102-110">属性</span><span class="sxs-lookup"><span data-stu-id="05102-110">Property</span></span>|<span data-ttu-id="05102-111">类型</span><span class="sxs-lookup"><span data-stu-id="05102-111">Type</span></span>|<span data-ttu-id="05102-112">说明</span><span class="sxs-lookup"><span data-stu-id="05102-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05102-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="05102-113">occurrenceDateTime</span></span>|<span data-ttu-id="05102-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05102-114">DateTimeOffset</span></span>|<span data-ttu-id="05102-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="05102-115">Time when the history item occurred.</span></span> <span data-ttu-id="05102-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="05102-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="05102-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="05102-117">securityGroupId</span></span>|<span data-ttu-id="05102-118">String</span><span class="sxs-lookup"><span data-stu-id="05102-118">String</span></span>|<span data-ttu-id="05102-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="05102-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="05102-120">runState</span><span class="sxs-lookup"><span data-stu-id="05102-120">runState</span></span>|[<span data-ttu-id="05102-121">runState</span><span class="sxs-lookup"><span data-stu-id="05102-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="05102-122">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="05102-122">Status of the item.</span></span> <span data-ttu-id="05102-123">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="05102-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="05102-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="05102-124">errorCode</span></span>|<span data-ttu-id="05102-125">String</span><span class="sxs-lookup"><span data-stu-id="05102-125">String</span></span>|<span data-ttu-id="05102-126">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="05102-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05102-127">关系</span><span class="sxs-lookup"><span data-stu-id="05102-127">Relationships</span></span>
<span data-ttu-id="05102-128">无</span><span class="sxs-lookup"><span data-stu-id="05102-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05102-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05102-129">JSON Representation</span></span>
<span data-ttu-id="05102-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05102-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




