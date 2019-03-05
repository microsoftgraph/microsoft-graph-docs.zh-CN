---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 定义适用于 iOS Vpp 应用程序的操作的结果, 包含 ActionResult 的继承属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 542382411fcc1070dc0c397efbf43431081d73f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153450"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="40a71-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="40a71-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="40a71-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40a71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40a71-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40a71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40a71-106">定义适用于 iOS Vpp 应用程序的操作的结果, 包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="40a71-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="40a71-107">属性</span><span class="sxs-lookup"><span data-stu-id="40a71-107">Properties</span></span>
|<span data-ttu-id="40a71-108">属性</span><span class="sxs-lookup"><span data-stu-id="40a71-108">Property</span></span>|<span data-ttu-id="40a71-109">类型</span><span class="sxs-lookup"><span data-stu-id="40a71-109">Type</span></span>|<span data-ttu-id="40a71-110">说明</span><span class="sxs-lookup"><span data-stu-id="40a71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40a71-111">userId</span><span class="sxs-lookup"><span data-stu-id="40a71-111">userId</span></span>|<span data-ttu-id="40a71-112">String</span><span class="sxs-lookup"><span data-stu-id="40a71-112">String</span></span>|<span data-ttu-id="40a71-113">与操作关联的用户 id。</span><span class="sxs-lookup"><span data-stu-id="40a71-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="40a71-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="40a71-114">managedDeviceId</span></span>|<span data-ttu-id="40a71-115">String</span><span class="sxs-lookup"><span data-stu-id="40a71-115">String</span></span>|<span data-ttu-id="40a71-116">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="40a71-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="40a71-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="40a71-117">totalLicensesCount</span></span>|<span data-ttu-id="40a71-118">Int32</span><span class="sxs-lookup"><span data-stu-id="40a71-118">Int32</span></span>|<span data-ttu-id="40a71-119">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="40a71-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="40a71-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="40a71-120">failedLicensesCount</span></span>|<span data-ttu-id="40a71-121">Int32</span><span class="sxs-lookup"><span data-stu-id="40a71-121">Int32</span></span>|<span data-ttu-id="40a71-122">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="40a71-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="40a71-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="40a71-123">actionFailureReason</span></span>|[<span data-ttu-id="40a71-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="40a71-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="40a71-125">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="40a71-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="40a71-126">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="40a71-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="40a71-127">actionName</span><span class="sxs-lookup"><span data-stu-id="40a71-127">actionName</span></span>|<span data-ttu-id="40a71-128">String</span><span class="sxs-lookup"><span data-stu-id="40a71-128">String</span></span>|<span data-ttu-id="40a71-129">操作名</span><span class="sxs-lookup"><span data-stu-id="40a71-129">Action name</span></span>|
|<span data-ttu-id="40a71-130">actionState</span><span class="sxs-lookup"><span data-stu-id="40a71-130">actionState</span></span>|[<span data-ttu-id="40a71-131">actionState</span><span class="sxs-lookup"><span data-stu-id="40a71-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="40a71-132">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="40a71-132">State of the action.</span></span> <span data-ttu-id="40a71-133">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="40a71-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="40a71-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="40a71-134">startDateTime</span></span>|<span data-ttu-id="40a71-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a71-135">DateTimeOffset</span></span>|<span data-ttu-id="40a71-136">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="40a71-136">Time the action was initiated</span></span>|
|<span data-ttu-id="40a71-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="40a71-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="40a71-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40a71-138">DateTimeOffset</span></span>|<span data-ttu-id="40a71-139">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="40a71-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="40a71-140">关系</span><span class="sxs-lookup"><span data-stu-id="40a71-140">Relationships</span></span>
<span data-ttu-id="40a71-141">无</span><span class="sxs-lookup"><span data-stu-id="40a71-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40a71-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40a71-142">JSON Representation</span></span>
<span data-ttu-id="40a71-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40a71-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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




