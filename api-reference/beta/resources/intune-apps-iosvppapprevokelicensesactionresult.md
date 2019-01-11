---
title: iosVppAppRevokeLicensesActionResult 资源类型
description: 在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。
localization_priority: Normal
ms.openlocfilehash: 8ed57465e263245cfc18ca22899c2142d949855d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842082"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="7c566-103">iosVppAppRevokeLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c566-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="7c566-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7c566-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c566-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7c566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c566-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7c566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c566-107">在 iOS Vpp 应用程序定义的操作的结果，包含 ActionResult 继承的属性。</span><span class="sxs-lookup"><span data-stu-id="7c566-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="7c566-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c566-108">Properties</span></span>
|<span data-ttu-id="7c566-109">属性</span><span class="sxs-lookup"><span data-stu-id="7c566-109">Property</span></span>|<span data-ttu-id="7c566-110">类型</span><span class="sxs-lookup"><span data-stu-id="7c566-110">Type</span></span>|<span data-ttu-id="7c566-111">Description</span><span class="sxs-lookup"><span data-stu-id="7c566-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c566-112">userId</span><span class="sxs-lookup"><span data-stu-id="7c566-112">userId</span></span>|<span data-ttu-id="7c566-113">String</span><span class="sxs-lookup"><span data-stu-id="7c566-113">String</span></span>|<span data-ttu-id="7c566-114">与操作关联的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="7c566-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="7c566-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7c566-115">managedDeviceId</span></span>|<span data-ttu-id="7c566-116">字符串</span><span class="sxs-lookup"><span data-stu-id="7c566-116">String</span></span>|<span data-ttu-id="7c566-117">DeviceId 与操作关联。</span><span class="sxs-lookup"><span data-stu-id="7c566-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="7c566-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="7c566-118">totalLicensesCount</span></span>|<span data-ttu-id="7c566-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7c566-119">Int32</span></span>|<span data-ttu-id="7c566-120">Revoke 尝试建立为其许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="7c566-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="7c566-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="7c566-121">failedLicensesCount</span></span>|<span data-ttu-id="7c566-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7c566-122">Int32</span></span>|<span data-ttu-id="7c566-123">失败的吊销许可证数的计数。</span><span class="sxs-lookup"><span data-stu-id="7c566-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="7c566-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="7c566-124">actionFailureReason</span></span>|[<span data-ttu-id="7c566-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="7c566-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="7c566-126">Revoke 许可证操作失败的原因。</span><span class="sxs-lookup"><span data-stu-id="7c566-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="7c566-127">可取值为：`none`、`appleFailure`、`internalError`、`expiredVppToken`、`expiredApplePushNotificationCertificate`。</span><span class="sxs-lookup"><span data-stu-id="7c566-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="7c566-128">actionName</span><span class="sxs-lookup"><span data-stu-id="7c566-128">actionName</span></span>|<span data-ttu-id="7c566-129">String</span><span class="sxs-lookup"><span data-stu-id="7c566-129">String</span></span>|<span data-ttu-id="7c566-130">操作名</span><span class="sxs-lookup"><span data-stu-id="7c566-130">Action name</span></span>|
|<span data-ttu-id="7c566-131">actionState</span><span class="sxs-lookup"><span data-stu-id="7c566-131">actionState</span></span>|[<span data-ttu-id="7c566-132">actionState</span><span class="sxs-lookup"><span data-stu-id="7c566-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7c566-133">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7c566-133">State of the action.</span></span> <span data-ttu-id="7c566-134">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7c566-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7c566-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c566-135">startDateTime</span></span>|<span data-ttu-id="7c566-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c566-136">DateTimeOffset</span></span>|<span data-ttu-id="7c566-137">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="7c566-137">Time the action was initiated</span></span>|
|<span data-ttu-id="7c566-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c566-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="7c566-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c566-139">DateTimeOffset</span></span>|<span data-ttu-id="7c566-140">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="7c566-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c566-141">关系</span><span class="sxs-lookup"><span data-stu-id="7c566-141">Relationships</span></span>
<span data-ttu-id="7c566-142">无</span><span class="sxs-lookup"><span data-stu-id="7c566-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7c566-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c566-143">JSON Representation</span></span>
<span data-ttu-id="7c566-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c566-144">Here is a JSON representation of the resource.</span></span>
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





