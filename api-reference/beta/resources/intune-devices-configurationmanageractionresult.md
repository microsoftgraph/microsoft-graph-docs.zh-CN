---
title: configurationManagerActionResult 资源类型
description: ConfigurationManager 操作的结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de187585e7e8dd74f4495d7143030e30acf46c4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785082"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="063f5-103">configurationManagerActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="063f5-103">configurationManagerActionResult resource type</span></span>

> <span data-ttu-id="063f5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="063f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="063f5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="063f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="063f5-106">ConfigurationManager 操作的结果</span><span class="sxs-lookup"><span data-stu-id="063f5-106">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="063f5-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="063f5-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="063f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="063f5-108">Properties</span></span>
|<span data-ttu-id="063f5-109">属性</span><span class="sxs-lookup"><span data-stu-id="063f5-109">Property</span></span>|<span data-ttu-id="063f5-110">类型</span><span class="sxs-lookup"><span data-stu-id="063f5-110">Type</span></span>|<span data-ttu-id="063f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="063f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="063f5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="063f5-112">actionName</span></span>|<span data-ttu-id="063f5-113">String</span><span class="sxs-lookup"><span data-stu-id="063f5-113">String</span></span>|<span data-ttu-id="063f5-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="063f5-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="063f5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="063f5-115">actionState</span></span>|[<span data-ttu-id="063f5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="063f5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="063f5-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="063f5-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="063f5-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="063f5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="063f5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="063f5-119">startDateTime</span></span>|<span data-ttu-id="063f5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="063f5-120">DateTimeOffset</span></span>|<span data-ttu-id="063f5-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="063f5-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="063f5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="063f5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="063f5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="063f5-123">DateTimeOffset</span></span>|<span data-ttu-id="063f5-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="063f5-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="063f5-125">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="063f5-125">actionDeliveryStatus</span></span>|[<span data-ttu-id="063f5-126">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="063f5-126">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="063f5-127">传递到本地服务器的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="063f5-127">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="063f5-128">可取值为：`unknown`、`pendingDelivery`、`deliveredToConnectorService`、`failedToDeliverToConnectorService`、`deliveredToOnPremisesServer`。</span><span class="sxs-lookup"><span data-stu-id="063f5-128">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="063f5-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="063f5-129">errorCode</span></span>|<span data-ttu-id="063f5-130">Int32</span><span class="sxs-lookup"><span data-stu-id="063f5-130">Int32</span></span>|<span data-ttu-id="063f5-131">来自客户端的 Configuration Manager 操作的错误代码</span><span class="sxs-lookup"><span data-stu-id="063f5-131">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="063f5-132">关系</span><span class="sxs-lookup"><span data-stu-id="063f5-132">Relationships</span></span>
<span data-ttu-id="063f5-133">无</span><span class="sxs-lookup"><span data-stu-id="063f5-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="063f5-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="063f5-134">JSON Representation</span></span>
<span data-ttu-id="063f5-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="063f5-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "actionDeliveryStatus": "String",
  "errorCode": 1024
}
```



