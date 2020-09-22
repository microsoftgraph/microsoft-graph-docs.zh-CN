---
title: macOsVppAppRevokeLicensesActionResult 资源类型
description: 定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acaa10168696dc81e012fb9f18f01efd6262bd7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019619"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="7f242-103">macOsVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f242-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="7f242-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f242-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f242-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f242-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f242-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f242-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f242-107">定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="7f242-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="7f242-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f242-108">Properties</span></span>
|<span data-ttu-id="7f242-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f242-109">Property</span></span>|<span data-ttu-id="7f242-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f242-110">Type</span></span>|<span data-ttu-id="7f242-111">描述</span><span class="sxs-lookup"><span data-stu-id="7f242-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f242-112">userId</span><span class="sxs-lookup"><span data-stu-id="7f242-112">userId</span></span>|<span data-ttu-id="7f242-113">String</span><span class="sxs-lookup"><span data-stu-id="7f242-113">String</span></span>|<span data-ttu-id="7f242-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="7f242-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="7f242-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7f242-115">managedDeviceId</span></span>|<span data-ttu-id="7f242-116">String</span><span class="sxs-lookup"><span data-stu-id="7f242-116">String</span></span>|<span data-ttu-id="7f242-117">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="7f242-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="7f242-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="7f242-118">totalLicensesCount</span></span>|<span data-ttu-id="7f242-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7f242-119">Int32</span></span>|<span data-ttu-id="7f242-120">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="7f242-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="7f242-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="7f242-121">failedLicensesCount</span></span>|<span data-ttu-id="7f242-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7f242-122">Int32</span></span>|<span data-ttu-id="7f242-123">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="7f242-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="7f242-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="7f242-124">actionFailureReason</span></span>|[<span data-ttu-id="7f242-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="7f242-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="7f242-126">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="7f242-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="7f242-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="7f242-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="7f242-128">actionName</span><span class="sxs-lookup"><span data-stu-id="7f242-128">actionName</span></span>|<span data-ttu-id="7f242-129">String</span><span class="sxs-lookup"><span data-stu-id="7f242-129">String</span></span>|<span data-ttu-id="7f242-130">操作名</span><span class="sxs-lookup"><span data-stu-id="7f242-130">Action name</span></span>|
|<span data-ttu-id="7f242-131">actionState</span><span class="sxs-lookup"><span data-stu-id="7f242-131">actionState</span></span>|[<span data-ttu-id="7f242-132">actionState</span><span class="sxs-lookup"><span data-stu-id="7f242-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7f242-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7f242-133">State of the action.</span></span> <span data-ttu-id="7f242-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7f242-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7f242-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f242-135">startDateTime</span></span>|<span data-ttu-id="7f242-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f242-136">DateTimeOffset</span></span>|<span data-ttu-id="7f242-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="7f242-137">Time the action was initiated</span></span>|
|<span data-ttu-id="7f242-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f242-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="7f242-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f242-139">DateTimeOffset</span></span>|<span data-ttu-id="7f242-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="7f242-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f242-141">关系</span><span class="sxs-lookup"><span data-stu-id="7f242-141">Relationships</span></span>
<span data-ttu-id="7f242-142">无</span><span class="sxs-lookup"><span data-stu-id="7f242-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f242-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f242-143">JSON Representation</span></span>
<span data-ttu-id="7f242-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f242-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```






