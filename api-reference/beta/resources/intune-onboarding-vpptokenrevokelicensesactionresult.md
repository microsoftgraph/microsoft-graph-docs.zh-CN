---
title: vppTokenRevokeLicensesActionResult 资源类型
description: 在 Apple 卷购买计划令牌上执行吊销许可证操作的状态。
author: tfitzmac
ms.openlocfilehash: a4188a269f9273b955fd29b32348dec82023b181
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351455"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="6a0c9-103">vppTokenRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a0c9-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="6a0c9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a0c9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a0c9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a0c9-107">在 Apple 卷购买计划令牌上执行吊销许可证操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="6a0c9-108">继承自[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a0c9-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a0c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="6a0c9-109">Properties</span></span>
|<span data-ttu-id="6a0c9-110">属性</span><span class="sxs-lookup"><span data-stu-id="6a0c9-110">Property</span></span>|<span data-ttu-id="6a0c9-111">类型</span><span class="sxs-lookup"><span data-stu-id="6a0c9-111">Type</span></span>|<span data-ttu-id="6a0c9-112">说明</span><span class="sxs-lookup"><span data-stu-id="6a0c9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a0c9-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6a0c9-113">actionName</span></span>|<span data-ttu-id="6a0c9-114">String</span><span class="sxs-lookup"><span data-stu-id="6a0c9-114">String</span></span>|<span data-ttu-id="6a0c9-115">操作名称继承[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a0c9-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6a0c9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6a0c9-116">actionState</span></span>|[<span data-ttu-id="6a0c9-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6a0c9-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6a0c9-118">从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="6a0c9-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6a0c9-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0c9-120">startDateTime</span></span>|<span data-ttu-id="6a0c9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0c9-121">DateTimeOffset</span></span>|<span data-ttu-id="6a0c9-122">初始化的操作的时间从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)继承</span><span class="sxs-lookup"><span data-stu-id="6a0c9-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6a0c9-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0c9-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6a0c9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0c9-124">DateTimeOffset</span></span>|<span data-ttu-id="6a0c9-125">上次使用的操作状态的时间从[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)更新继承</span><span class="sxs-lookup"><span data-stu-id="6a0c9-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="6a0c9-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6a0c9-126">totalLicensesCount</span></span>|<span data-ttu-id="6a0c9-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6a0c9-127">Int32</span></span>|<span data-ttu-id="6a0c9-128">已尝试撤消的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="6a0c9-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6a0c9-129">failedLicensesCount</span></span>|<span data-ttu-id="6a0c9-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6a0c9-130">Int32</span></span>|<span data-ttu-id="6a0c9-131">无法撤消的许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="6a0c9-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6a0c9-132">actionFailureReason</span></span>|[<span data-ttu-id="6a0c9-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6a0c9-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="6a0c9-134">Revoke 许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="6a0c9-135">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a0c9-136">Relationships</span><span class="sxs-lookup"><span data-stu-id="6a0c9-136">Relationships</span></span>
<span data-ttu-id="6a0c9-137">无</span><span class="sxs-lookup"><span data-stu-id="6a0c9-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a0c9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a0c9-138">JSON Representation</span></span>
<span data-ttu-id="6a0c9-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a0c9-139">Here is a JSON representation of the resource.</span></span>
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





