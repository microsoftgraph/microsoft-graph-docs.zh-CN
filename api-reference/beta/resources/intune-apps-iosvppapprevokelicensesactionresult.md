---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 13bc69a0c04eb7b9742f6c549fd1ae976cf25561
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986990"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="ceaa1-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="ceaa1-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="ceaa1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceaa1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceaa1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceaa1-107">在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="ceaa1-108">属性</span><span class="sxs-lookup"><span data-stu-id="ceaa1-108">Properties</span></span>
|<span data-ttu-id="ceaa1-109">属性</span><span class="sxs-lookup"><span data-stu-id="ceaa1-109">Property</span></span>|<span data-ttu-id="ceaa1-110">类型</span><span class="sxs-lookup"><span data-stu-id="ceaa1-110">Type</span></span>|<span data-ttu-id="ceaa1-111">说明</span><span class="sxs-lookup"><span data-stu-id="ceaa1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceaa1-112">userId</span><span class="sxs-lookup"><span data-stu-id="ceaa1-112">userId</span></span>|<span data-ttu-id="ceaa1-113">String</span><span class="sxs-lookup"><span data-stu-id="ceaa1-113">String</span></span>|<span data-ttu-id="ceaa1-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="ceaa1-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ceaa1-115">managedDeviceId</span></span>|<span data-ttu-id="ceaa1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ceaa1-116">String</span></span>|<span data-ttu-id="ceaa1-117">DeviceId 与操作关联。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="ceaa1-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ceaa1-118">totalLicensesCount</span></span>|<span data-ttu-id="ceaa1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ceaa1-119">Int32</span></span>|<span data-ttu-id="ceaa1-120">Revoke 尝试建立为其许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="ceaa1-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ceaa1-121">failedLicensesCount</span></span>|<span data-ttu-id="ceaa1-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ceaa1-122">Int32</span></span>|<span data-ttu-id="ceaa1-123">失败的吊销许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="ceaa1-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ceaa1-124">actionFailureReason</span></span>|[<span data-ttu-id="ceaa1-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ceaa1-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="ceaa1-126">Revoke 许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="ceaa1-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="ceaa1-128">actionName</span><span class="sxs-lookup"><span data-stu-id="ceaa1-128">actionName</span></span>|<span data-ttu-id="ceaa1-129">String</span><span class="sxs-lookup"><span data-stu-id="ceaa1-129">String</span></span>|<span data-ttu-id="ceaa1-130">操作名</span><span class="sxs-lookup"><span data-stu-id="ceaa1-130">Action name</span></span>|
|<span data-ttu-id="ceaa1-131">actionState</span><span class="sxs-lookup"><span data-stu-id="ceaa1-131">actionState</span></span>|[<span data-ttu-id="ceaa1-132">actionState</span><span class="sxs-lookup"><span data-stu-id="ceaa1-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ceaa1-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-133">State of the action.</span></span> <span data-ttu-id="ceaa1-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ceaa1-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ceaa1-135">startDateTime</span></span>|<span data-ttu-id="ceaa1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceaa1-136">DateTimeOffset</span></span>|<span data-ttu-id="ceaa1-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="ceaa1-137">Time the action was initiated</span></span>|
|<span data-ttu-id="ceaa1-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceaa1-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="ceaa1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceaa1-139">DateTimeOffset</span></span>|<span data-ttu-id="ceaa1-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="ceaa1-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceaa1-141">关系</span><span class="sxs-lookup"><span data-stu-id="ceaa1-141">Relationships</span></span>
<span data-ttu-id="ceaa1-142">无</span><span class="sxs-lookup"><span data-stu-id="ceaa1-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ceaa1-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ceaa1-143">JSON Representation</span></span>
<span data-ttu-id="ceaa1-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceaa1-144">Here is a JSON representation of the resource.</span></span>
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





