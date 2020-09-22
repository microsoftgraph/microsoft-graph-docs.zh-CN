---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 在 Apple Volume Purchase Program 令牌上执行的吊销许可证操作的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb95f91bcdce22ca51ed9fa36fbee1dc15fa2720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029342"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="dce34-103">vppTokenRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="dce34-103">vppTokenRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="dce34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dce34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dce34-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dce34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dce34-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dce34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce34-107">在 Apple Volume Purchase Program 令牌上执行的吊销许可证操作的状态。</span><span class="sxs-lookup"><span data-stu-id="dce34-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="dce34-108">继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dce34-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dce34-109">属性</span><span class="sxs-lookup"><span data-stu-id="dce34-109">Properties</span></span>
|<span data-ttu-id="dce34-110">属性</span><span class="sxs-lookup"><span data-stu-id="dce34-110">Property</span></span>|<span data-ttu-id="dce34-111">类型</span><span class="sxs-lookup"><span data-stu-id="dce34-111">Type</span></span>|<span data-ttu-id="dce34-112">说明</span><span class="sxs-lookup"><span data-stu-id="dce34-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dce34-113">actionName</span><span class="sxs-lookup"><span data-stu-id="dce34-113">actionName</span></span>|<span data-ttu-id="dce34-114">String</span><span class="sxs-lookup"><span data-stu-id="dce34-114">String</span></span>|<span data-ttu-id="dce34-115">从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作名称</span><span class="sxs-lookup"><span data-stu-id="dce34-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="dce34-116">actionState</span><span class="sxs-lookup"><span data-stu-id="dce34-116">actionState</span></span>|[<span data-ttu-id="dce34-117">actionState</span><span class="sxs-lookup"><span data-stu-id="dce34-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="dce34-118">继承自 [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="dce34-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="dce34-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="dce34-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dce34-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dce34-120">startDateTime</span></span>|<span data-ttu-id="dce34-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce34-121">DateTimeOffset</span></span>|<span data-ttu-id="dce34-122">从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承的操作的开始时间</span><span class="sxs-lookup"><span data-stu-id="dce34-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="dce34-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dce34-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="dce34-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce34-124">DateTimeOffset</span></span>|<span data-ttu-id="dce34-125">上次更新操作状态的时间从[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承</span><span class="sxs-lookup"><span data-stu-id="dce34-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="dce34-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="dce34-126">totalLicensesCount</span></span>|<span data-ttu-id="dce34-127">Int32</span><span class="sxs-lookup"><span data-stu-id="dce34-127">Int32</span></span>|<span data-ttu-id="dce34-128">试图吊销的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="dce34-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="dce34-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="dce34-129">failedLicensesCount</span></span>|<span data-ttu-id="dce34-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dce34-130">Int32</span></span>|<span data-ttu-id="dce34-131">无法撤消的许可证数量的计数。</span><span class="sxs-lookup"><span data-stu-id="dce34-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="dce34-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="dce34-132">actionFailureReason</span></span>|[<span data-ttu-id="dce34-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="dce34-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="dce34-134">吊销许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="dce34-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="dce34-135">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="dce34-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dce34-136">关系</span><span class="sxs-lookup"><span data-stu-id="dce34-136">Relationships</span></span>
<span data-ttu-id="dce34-137">无</span><span class="sxs-lookup"><span data-stu-id="dce34-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dce34-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dce34-138">JSON Representation</span></span>
<span data-ttu-id="dce34-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dce34-139">Here is a JSON representation of the resource.</span></span>
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






