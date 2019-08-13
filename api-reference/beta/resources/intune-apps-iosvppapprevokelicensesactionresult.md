---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 定义适用于 iOS Vpp 应用程序的操作的结果, 包含 ActionResult 的继承属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb297bff4c51a23076fb2d6ff2c4505be017989b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365949"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="d3907-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3907-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="d3907-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3907-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3907-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3907-106">定义适用于 iOS Vpp 应用程序的操作的结果, 包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="d3907-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="d3907-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3907-107">Properties</span></span>
|<span data-ttu-id="d3907-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3907-108">Property</span></span>|<span data-ttu-id="d3907-109">类型</span><span class="sxs-lookup"><span data-stu-id="d3907-109">Type</span></span>|<span data-ttu-id="d3907-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3907-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3907-111">userId</span><span class="sxs-lookup"><span data-stu-id="d3907-111">userId</span></span>|<span data-ttu-id="d3907-112">String</span><span class="sxs-lookup"><span data-stu-id="d3907-112">String</span></span>|<span data-ttu-id="d3907-113">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="d3907-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="d3907-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d3907-114">managedDeviceId</span></span>|<span data-ttu-id="d3907-115">String</span><span class="sxs-lookup"><span data-stu-id="d3907-115">String</span></span>|<span data-ttu-id="d3907-116">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="d3907-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="d3907-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="d3907-117">totalLicensesCount</span></span>|<span data-ttu-id="d3907-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d3907-118">Int32</span></span>|<span data-ttu-id="d3907-119">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="d3907-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="d3907-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="d3907-120">failedLicensesCount</span></span>|<span data-ttu-id="d3907-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d3907-121">Int32</span></span>|<span data-ttu-id="d3907-122">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="d3907-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="d3907-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="d3907-123">actionFailureReason</span></span>|[<span data-ttu-id="d3907-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="d3907-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="d3907-125">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="d3907-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="d3907-126">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="d3907-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="d3907-127">actionName</span><span class="sxs-lookup"><span data-stu-id="d3907-127">actionName</span></span>|<span data-ttu-id="d3907-128">String</span><span class="sxs-lookup"><span data-stu-id="d3907-128">String</span></span>|<span data-ttu-id="d3907-129">操作名</span><span class="sxs-lookup"><span data-stu-id="d3907-129">Action name</span></span>|
|<span data-ttu-id="d3907-130">actionState</span><span class="sxs-lookup"><span data-stu-id="d3907-130">actionState</span></span>|[<span data-ttu-id="d3907-131">actionState</span><span class="sxs-lookup"><span data-stu-id="d3907-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d3907-132">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d3907-132">State of the action.</span></span> <span data-ttu-id="d3907-133">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d3907-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d3907-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d3907-134">startDateTime</span></span>|<span data-ttu-id="d3907-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3907-135">DateTimeOffset</span></span>|<span data-ttu-id="d3907-136">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="d3907-136">Time the action was initiated</span></span>|
|<span data-ttu-id="d3907-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3907-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="d3907-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3907-138">DateTimeOffset</span></span>|<span data-ttu-id="d3907-139">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="d3907-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3907-140">关系</span><span class="sxs-lookup"><span data-stu-id="d3907-140">Relationships</span></span>
<span data-ttu-id="d3907-141">无</span><span class="sxs-lookup"><span data-stu-id="d3907-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3907-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3907-142">JSON Representation</span></span>
<span data-ttu-id="d3907-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3907-143">Here is a JSON representation of the resource.</span></span>
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



