---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 在 Apple Volume Purchase Program 令牌上执行的吊销许可证操作的状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 543ec2a75c61c516cfe32632a82a7cfd08810f94
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940251"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="cbe89-103">vppTokenRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbe89-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="cbe89-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbe89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbe89-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbe89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbe89-106">在 Apple Volume Purchase Program 令牌上执行的吊销许可证操作的状态。</span><span class="sxs-lookup"><span data-stu-id="cbe89-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="cbe89-107">继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cbe89-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cbe89-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbe89-108">Properties</span></span>
|<span data-ttu-id="cbe89-109">属性</span><span class="sxs-lookup"><span data-stu-id="cbe89-109">Property</span></span>|<span data-ttu-id="cbe89-110">类型</span><span class="sxs-lookup"><span data-stu-id="cbe89-110">Type</span></span>|<span data-ttu-id="cbe89-111">说明</span><span class="sxs-lookup"><span data-stu-id="cbe89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe89-112">actionName</span><span class="sxs-lookup"><span data-stu-id="cbe89-112">actionName</span></span>|<span data-ttu-id="cbe89-113">String</span><span class="sxs-lookup"><span data-stu-id="cbe89-113">String</span></span>|<span data-ttu-id="cbe89-114">从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作名称</span><span class="sxs-lookup"><span data-stu-id="cbe89-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cbe89-115">actionState</span><span class="sxs-lookup"><span data-stu-id="cbe89-115">actionState</span></span>|[<span data-ttu-id="cbe89-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cbe89-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cbe89-117">继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="cbe89-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="cbe89-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="cbe89-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cbe89-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cbe89-119">startDateTime</span></span>|<span data-ttu-id="cbe89-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbe89-120">DateTimeOffset</span></span>|<span data-ttu-id="cbe89-121">从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作的开始时间</span><span class="sxs-lookup"><span data-stu-id="cbe89-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cbe89-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbe89-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="cbe89-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbe89-123">DateTimeOffset</span></span>|<span data-ttu-id="cbe89-124">上次更新操作状态的时间从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承</span><span class="sxs-lookup"><span data-stu-id="cbe89-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cbe89-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cbe89-125">totalLicensesCount</span></span>|<span data-ttu-id="cbe89-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe89-126">Int32</span></span>|<span data-ttu-id="cbe89-127">试图吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="cbe89-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="cbe89-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cbe89-128">failedLicensesCount</span></span>|<span data-ttu-id="cbe89-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe89-129">Int32</span></span>|<span data-ttu-id="cbe89-130">无法撤消的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="cbe89-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="cbe89-131">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="cbe89-131">actionFailureReason</span></span>|[<span data-ttu-id="cbe89-132">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="cbe89-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="cbe89-133">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="cbe89-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="cbe89-134">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="cbe89-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbe89-135">关系</span><span class="sxs-lookup"><span data-stu-id="cbe89-135">Relationships</span></span>
<span data-ttu-id="cbe89-136">无</span><span class="sxs-lookup"><span data-stu-id="cbe89-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbe89-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbe89-137">JSON Representation</span></span>
<span data-ttu-id="cbe89-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbe89-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```




