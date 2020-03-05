---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 定义适用于 iOS Vpp 应用程序的操作的结果，包含 ActionResult 的继承属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbc7ea19fb2a644b889ac1a6a00f5a3fba503f93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493221"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="1c194-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c194-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="1c194-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1c194-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c194-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c194-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c194-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c194-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c194-107">定义适用于 iOS Vpp 应用程序的操作的结果，包含 ActionResult 的继承属性。</span><span class="sxs-lookup"><span data-stu-id="1c194-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="1c194-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c194-108">Properties</span></span>
|<span data-ttu-id="1c194-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c194-109">Property</span></span>|<span data-ttu-id="1c194-110">类型</span><span class="sxs-lookup"><span data-stu-id="1c194-110">Type</span></span>|<span data-ttu-id="1c194-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c194-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c194-112">userId</span><span class="sxs-lookup"><span data-stu-id="1c194-112">userId</span></span>|<span data-ttu-id="1c194-113">String</span><span class="sxs-lookup"><span data-stu-id="1c194-113">String</span></span>|<span data-ttu-id="1c194-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="1c194-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="1c194-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1c194-115">managedDeviceId</span></span>|<span data-ttu-id="1c194-116">String</span><span class="sxs-lookup"><span data-stu-id="1c194-116">String</span></span>|<span data-ttu-id="1c194-117">与操作相关联的 DeviceId。</span><span class="sxs-lookup"><span data-stu-id="1c194-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="1c194-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1c194-118">totalLicensesCount</span></span>|<span data-ttu-id="1c194-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1c194-119">Int32</span></span>|<span data-ttu-id="1c194-120">尝试吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="1c194-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="1c194-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1c194-121">failedLicensesCount</span></span>|<span data-ttu-id="1c194-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1c194-122">Int32</span></span>|<span data-ttu-id="1c194-123">吊销失败的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="1c194-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="1c194-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1c194-124">actionFailureReason</span></span>|[<span data-ttu-id="1c194-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1c194-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="1c194-126">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="1c194-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="1c194-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="1c194-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="1c194-128">actionName</span><span class="sxs-lookup"><span data-stu-id="1c194-128">actionName</span></span>|<span data-ttu-id="1c194-129">String</span><span class="sxs-lookup"><span data-stu-id="1c194-129">String</span></span>|<span data-ttu-id="1c194-130">操作名</span><span class="sxs-lookup"><span data-stu-id="1c194-130">Action name</span></span>|
|<span data-ttu-id="1c194-131">actionState</span><span class="sxs-lookup"><span data-stu-id="1c194-131">actionState</span></span>|[<span data-ttu-id="1c194-132">actionState</span><span class="sxs-lookup"><span data-stu-id="1c194-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1c194-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1c194-133">State of the action.</span></span> <span data-ttu-id="1c194-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="1c194-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1c194-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1c194-135">startDateTime</span></span>|<span data-ttu-id="1c194-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c194-136">DateTimeOffset</span></span>|<span data-ttu-id="1c194-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="1c194-137">Time the action was initiated</span></span>|
|<span data-ttu-id="1c194-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c194-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="1c194-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c194-139">DateTimeOffset</span></span>|<span data-ttu-id="1c194-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="1c194-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c194-141">关系</span><span class="sxs-lookup"><span data-stu-id="1c194-141">Relationships</span></span>
<span data-ttu-id="1c194-142">无</span><span class="sxs-lookup"><span data-stu-id="1c194-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c194-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c194-143">JSON Representation</span></span>
<span data-ttu-id="1c194-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c194-144">Here is a JSON representation of the resource.</span></span>
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



