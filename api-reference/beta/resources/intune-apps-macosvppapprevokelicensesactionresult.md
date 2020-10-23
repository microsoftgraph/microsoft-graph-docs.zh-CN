---
title: macOsVppAppRevokeLicensesActionResult 资源类型
description: 定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97daa2d7c156664f359bc454067981b71c5e4d5b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707204"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="5190f-103">macOsVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="5190f-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="5190f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5190f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5190f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5190f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5190f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5190f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5190f-107">定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="5190f-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="5190f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5190f-108">Properties</span></span>
|<span data-ttu-id="5190f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5190f-109">Property</span></span>|<span data-ttu-id="5190f-110">类型</span><span class="sxs-lookup"><span data-stu-id="5190f-110">Type</span></span>|<span data-ttu-id="5190f-111">描述</span><span class="sxs-lookup"><span data-stu-id="5190f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5190f-112">userId</span><span class="sxs-lookup"><span data-stu-id="5190f-112">userId</span></span>|<span data-ttu-id="5190f-113">String</span><span class="sxs-lookup"><span data-stu-id="5190f-113">String</span></span>|<span data-ttu-id="5190f-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="5190f-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="5190f-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5190f-115">managedDeviceId</span></span>|<span data-ttu-id="5190f-116">String</span><span class="sxs-lookup"><span data-stu-id="5190f-116">String</span></span>|<span data-ttu-id="5190f-117">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="5190f-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="5190f-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="5190f-118">totalLicensesCount</span></span>|<span data-ttu-id="5190f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="5190f-119">Int32</span></span>|<span data-ttu-id="5190f-120">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="5190f-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="5190f-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="5190f-121">failedLicensesCount</span></span>|<span data-ttu-id="5190f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5190f-122">Int32</span></span>|<span data-ttu-id="5190f-123">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="5190f-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="5190f-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="5190f-124">actionFailureReason</span></span>|[<span data-ttu-id="5190f-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="5190f-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="5190f-126">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="5190f-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="5190f-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="5190f-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="5190f-128">actionName</span><span class="sxs-lookup"><span data-stu-id="5190f-128">actionName</span></span>|<span data-ttu-id="5190f-129">String</span><span class="sxs-lookup"><span data-stu-id="5190f-129">String</span></span>|<span data-ttu-id="5190f-130">操作名</span><span class="sxs-lookup"><span data-stu-id="5190f-130">Action name</span></span>|
|<span data-ttu-id="5190f-131">actionState</span><span class="sxs-lookup"><span data-stu-id="5190f-131">actionState</span></span>|[<span data-ttu-id="5190f-132">actionState</span><span class="sxs-lookup"><span data-stu-id="5190f-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5190f-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5190f-133">State of the action.</span></span> <span data-ttu-id="5190f-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="5190f-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5190f-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5190f-135">startDateTime</span></span>|<span data-ttu-id="5190f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5190f-136">DateTimeOffset</span></span>|<span data-ttu-id="5190f-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="5190f-137">Time the action was initiated</span></span>|
|<span data-ttu-id="5190f-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5190f-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="5190f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5190f-139">DateTimeOffset</span></span>|<span data-ttu-id="5190f-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="5190f-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5190f-141">关系</span><span class="sxs-lookup"><span data-stu-id="5190f-141">Relationships</span></span>
<span data-ttu-id="5190f-142">无</span><span class="sxs-lookup"><span data-stu-id="5190f-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5190f-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5190f-143">JSON Representation</span></span>
<span data-ttu-id="5190f-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5190f-144">Here is a JSON representation of the resource.</span></span>
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





