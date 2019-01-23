---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f64f2df709d5332be46dd76216b1a1457d27a61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418902"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="9e499-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e499-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="9e499-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9e499-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e499-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9e499-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e499-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e499-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e499-107">在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。</span><span class="sxs-lookup"><span data-stu-id="9e499-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="9e499-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e499-108">Properties</span></span>
|<span data-ttu-id="9e499-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e499-109">Property</span></span>|<span data-ttu-id="9e499-110">类型</span><span class="sxs-lookup"><span data-stu-id="9e499-110">Type</span></span>|<span data-ttu-id="9e499-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e499-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e499-112">userId</span><span class="sxs-lookup"><span data-stu-id="9e499-112">userId</span></span>|<span data-ttu-id="9e499-113">String</span><span class="sxs-lookup"><span data-stu-id="9e499-113">String</span></span>|<span data-ttu-id="9e499-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="9e499-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="9e499-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9e499-115">managedDeviceId</span></span>|<span data-ttu-id="9e499-116">String</span><span class="sxs-lookup"><span data-stu-id="9e499-116">String</span></span>|<span data-ttu-id="9e499-117">DeviceId 与操作关联。</span><span class="sxs-lookup"><span data-stu-id="9e499-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="9e499-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9e499-118">totalLicensesCount</span></span>|<span data-ttu-id="9e499-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9e499-119">Int32</span></span>|<span data-ttu-id="9e499-120">Revoke 尝试建立为其许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="9e499-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="9e499-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="9e499-121">failedLicensesCount</span></span>|<span data-ttu-id="9e499-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9e499-122">Int32</span></span>|<span data-ttu-id="9e499-123">失败的吊销许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="9e499-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="9e499-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="9e499-124">actionFailureReason</span></span>|[<span data-ttu-id="9e499-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="9e499-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="9e499-126">Revoke 许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="9e499-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="9e499-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="9e499-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="9e499-128">actionName</span><span class="sxs-lookup"><span data-stu-id="9e499-128">actionName</span></span>|<span data-ttu-id="9e499-129">String</span><span class="sxs-lookup"><span data-stu-id="9e499-129">String</span></span>|<span data-ttu-id="9e499-130">操作名</span><span class="sxs-lookup"><span data-stu-id="9e499-130">Action name</span></span>|
|<span data-ttu-id="9e499-131">actionState</span><span class="sxs-lookup"><span data-stu-id="9e499-131">actionState</span></span>|[<span data-ttu-id="9e499-132">actionState</span><span class="sxs-lookup"><span data-stu-id="9e499-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9e499-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9e499-133">State of the action.</span></span> <span data-ttu-id="9e499-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9e499-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9e499-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e499-135">startDateTime</span></span>|<span data-ttu-id="9e499-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e499-136">DateTimeOffset</span></span>|<span data-ttu-id="9e499-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="9e499-137">Time the action was initiated</span></span>|
|<span data-ttu-id="9e499-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e499-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="9e499-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e499-139">DateTimeOffset</span></span>|<span data-ttu-id="9e499-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="9e499-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e499-141">关系</span><span class="sxs-lookup"><span data-stu-id="9e499-141">Relationships</span></span>
<span data-ttu-id="9e499-142">无</span><span class="sxs-lookup"><span data-stu-id="9e499-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e499-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e499-143">JSON Representation</span></span>
<span data-ttu-id="9e499-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e499-144">Here is a JSON representation of the resource.</span></span>
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




