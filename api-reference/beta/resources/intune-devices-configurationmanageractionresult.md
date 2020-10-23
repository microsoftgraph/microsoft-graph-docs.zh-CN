---
title: configurationManagerActionResult 资源类型
description: ConfigurationManager 操作的结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c73775293385ecfcef8ef269a2f3e83c53b233f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691405"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="d0e89-103">configurationManagerActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0e89-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="d0e89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0e89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0e89-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0e89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0e89-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0e89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0e89-107">ConfigurationManager 操作的结果</span><span class="sxs-lookup"><span data-stu-id="d0e89-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="d0e89-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0e89-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0e89-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0e89-109">Properties</span></span>
|<span data-ttu-id="d0e89-110">属性</span><span class="sxs-lookup"><span data-stu-id="d0e89-110">Property</span></span>|<span data-ttu-id="d0e89-111">类型</span><span class="sxs-lookup"><span data-stu-id="d0e89-111">Type</span></span>|<span data-ttu-id="d0e89-112">说明</span><span class="sxs-lookup"><span data-stu-id="d0e89-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0e89-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d0e89-113">actionName</span></span>|<span data-ttu-id="d0e89-114">String</span><span class="sxs-lookup"><span data-stu-id="d0e89-114">String</span></span>|<span data-ttu-id="d0e89-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0e89-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0e89-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d0e89-116">actionState</span></span>|[<span data-ttu-id="d0e89-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d0e89-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d0e89-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d0e89-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d0e89-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d0e89-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d0e89-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e89-120">startDateTime</span></span>|<span data-ttu-id="d0e89-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e89-121">DateTimeOffset</span></span>|<span data-ttu-id="d0e89-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0e89-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0e89-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e89-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d0e89-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e89-124">DateTimeOffset</span></span>|<span data-ttu-id="d0e89-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0e89-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0e89-126">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="d0e89-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="d0e89-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="d0e89-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="d0e89-128">传递到本地服务器的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d0e89-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="d0e89-129">可取值为：`unknown`、`pendingDelivery`、`deliveredToConnectorService`、`failedToDeliverToConnectorService`、`deliveredToOnPremisesServer`。</span><span class="sxs-lookup"><span data-stu-id="d0e89-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="d0e89-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="d0e89-130">errorCode</span></span>|<span data-ttu-id="d0e89-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e89-131">Int32</span></span>|<span data-ttu-id="d0e89-132">来自客户端的 Configuration Manager 操作的错误代码</span><span class="sxs-lookup"><span data-stu-id="d0e89-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0e89-133">关系</span><span class="sxs-lookup"><span data-stu-id="d0e89-133">Relationships</span></span>
<span data-ttu-id="d0e89-134">无</span><span class="sxs-lookup"><span data-stu-id="d0e89-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0e89-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0e89-135">JSON Representation</span></span>
<span data-ttu-id="d0e89-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0e89-136">Here is a JSON representation of the resource.</span></span>
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





