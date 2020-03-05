---
title: macOsVppAppRevokeLicensesActionResult 资源类型
description: 定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccbdc0fe0e1d288571a768551691b539692572fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42492920"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="2262c-103">macOsVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2262c-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="2262c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2262c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2262c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2262c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2262c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2262c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2262c-107">定义操作的结果在 MacOS Vpp 应用中，包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="2262c-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="2262c-108">属性</span><span class="sxs-lookup"><span data-stu-id="2262c-108">Properties</span></span>
|<span data-ttu-id="2262c-109">属性</span><span class="sxs-lookup"><span data-stu-id="2262c-109">Property</span></span>|<span data-ttu-id="2262c-110">类型</span><span class="sxs-lookup"><span data-stu-id="2262c-110">Type</span></span>|<span data-ttu-id="2262c-111">说明</span><span class="sxs-lookup"><span data-stu-id="2262c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2262c-112">userId</span><span class="sxs-lookup"><span data-stu-id="2262c-112">userId</span></span>|<span data-ttu-id="2262c-113">String</span><span class="sxs-lookup"><span data-stu-id="2262c-113">String</span></span>|<span data-ttu-id="2262c-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="2262c-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="2262c-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2262c-115">managedDeviceId</span></span>|<span data-ttu-id="2262c-116">String</span><span class="sxs-lookup"><span data-stu-id="2262c-116">String</span></span>|<span data-ttu-id="2262c-117">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="2262c-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="2262c-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="2262c-118">totalLicensesCount</span></span>|<span data-ttu-id="2262c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2262c-119">Int32</span></span>|<span data-ttu-id="2262c-120">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="2262c-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="2262c-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="2262c-121">failedLicensesCount</span></span>|<span data-ttu-id="2262c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2262c-122">Int32</span></span>|<span data-ttu-id="2262c-123">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="2262c-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="2262c-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="2262c-124">actionFailureReason</span></span>|[<span data-ttu-id="2262c-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="2262c-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="2262c-126">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="2262c-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="2262c-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="2262c-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="2262c-128">actionName</span><span class="sxs-lookup"><span data-stu-id="2262c-128">actionName</span></span>|<span data-ttu-id="2262c-129">String</span><span class="sxs-lookup"><span data-stu-id="2262c-129">String</span></span>|<span data-ttu-id="2262c-130">操作名</span><span class="sxs-lookup"><span data-stu-id="2262c-130">Action name</span></span>|
|<span data-ttu-id="2262c-131">actionState</span><span class="sxs-lookup"><span data-stu-id="2262c-131">actionState</span></span>|[<span data-ttu-id="2262c-132">actionState</span><span class="sxs-lookup"><span data-stu-id="2262c-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2262c-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2262c-133">State of the action.</span></span> <span data-ttu-id="2262c-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2262c-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2262c-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2262c-135">startDateTime</span></span>|<span data-ttu-id="2262c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2262c-136">DateTimeOffset</span></span>|<span data-ttu-id="2262c-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="2262c-137">Time the action was initiated</span></span>|
|<span data-ttu-id="2262c-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2262c-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="2262c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2262c-139">DateTimeOffset</span></span>|<span data-ttu-id="2262c-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="2262c-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2262c-141">关系</span><span class="sxs-lookup"><span data-stu-id="2262c-141">Relationships</span></span>
<span data-ttu-id="2262c-142">无</span><span class="sxs-lookup"><span data-stu-id="2262c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2262c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2262c-143">JSON Representation</span></span>
<span data-ttu-id="2262c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2262c-144">Here is a JSON representation of the resource.</span></span>
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



