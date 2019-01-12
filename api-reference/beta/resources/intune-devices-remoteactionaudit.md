---
title: remoteActionAudit 资源类型
description: 属于某些租户的设备上启动远程操作的报告。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad583f13311e5baece70c5ec28ca8f7c73f5349e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972591"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="1408a-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="1408a-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="1408a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1408a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1408a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1408a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1408a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1408a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1408a-107">属于某些租户的设备上启动远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="1408a-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="1408a-108">方法</span><span class="sxs-lookup"><span data-stu-id="1408a-108">Methods</span></span>
|<span data-ttu-id="1408a-109">方法</span><span class="sxs-lookup"><span data-stu-id="1408a-109">Method</span></span>|<span data-ttu-id="1408a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1408a-110">Return Type</span></span>|<span data-ttu-id="1408a-111">说明</span><span class="sxs-lookup"><span data-stu-id="1408a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1408a-112">列表 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="1408a-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="1408a-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="1408a-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="1408a-114">列出属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1408a-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="1408a-115">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="1408a-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="1408a-117">读取属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1408a-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="1408a-118">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="1408a-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="1408a-120">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1408a-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="1408a-121">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="1408a-122">无</span><span class="sxs-lookup"><span data-stu-id="1408a-122">None</span></span>|<span data-ttu-id="1408a-123">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="1408a-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="1408a-124">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="1408a-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="1408a-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="1408a-126">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1408a-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1408a-127">属性</span><span class="sxs-lookup"><span data-stu-id="1408a-127">Properties</span></span>
|<span data-ttu-id="1408a-128">属性</span><span class="sxs-lookup"><span data-stu-id="1408a-128">Property</span></span>|<span data-ttu-id="1408a-129">类型</span><span class="sxs-lookup"><span data-stu-id="1408a-129">Type</span></span>|<span data-ttu-id="1408a-130">说明</span><span class="sxs-lookup"><span data-stu-id="1408a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1408a-131">id</span><span class="sxs-lookup"><span data-stu-id="1408a-131">id</span></span>|<span data-ttu-id="1408a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1408a-132">String</span></span>|<span data-ttu-id="1408a-133">报告 id。</span><span class="sxs-lookup"><span data-stu-id="1408a-133">Report Id.</span></span>|
|<span data-ttu-id="1408a-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1408a-134">deviceDisplayName</span></span>|<span data-ttu-id="1408a-135">String</span><span class="sxs-lookup"><span data-stu-id="1408a-135">String</span></span>|<span data-ttu-id="1408a-136">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="1408a-136">Intune device name.</span></span>|
|<span data-ttu-id="1408a-137">userName</span><span class="sxs-lookup"><span data-stu-id="1408a-137">userName</span></span>|<span data-ttu-id="1408a-138">String</span><span class="sxs-lookup"><span data-stu-id="1408a-138">String</span></span>|<span data-ttu-id="1408a-139">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="1408a-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="1408a-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1408a-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="1408a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="1408a-141">String</span></span>|<span data-ttu-id="1408a-142">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="1408a-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="1408a-143">action</span><span class="sxs-lookup"><span data-stu-id="1408a-143">action</span></span>|[<span data-ttu-id="1408a-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="1408a-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="1408a-145">操作名称。</span><span class="sxs-lookup"><span data-stu-id="1408a-145">The action name.</span></span> <span data-ttu-id="1408a-146">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="1408a-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="1408a-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="1408a-147">requestDateTime</span></span>|<span data-ttu-id="1408a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1408a-148">DateTimeOffset</span></span>|<span data-ttu-id="1408a-149">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1408a-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="1408a-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1408a-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="1408a-151">字符串</span><span class="sxs-lookup"><span data-stu-id="1408a-151">String</span></span>|<span data-ttu-id="1408a-152">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="1408a-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="1408a-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="1408a-153">deviceIMEI</span></span>|<span data-ttu-id="1408a-154">字符串</span><span class="sxs-lookup"><span data-stu-id="1408a-154">String</span></span>|<span data-ttu-id="1408a-155">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="1408a-155">IMEI of the device.</span></span>|
|<span data-ttu-id="1408a-156">actionState</span><span class="sxs-lookup"><span data-stu-id="1408a-156">actionState</span></span>|[<span data-ttu-id="1408a-157">actionState</span><span class="sxs-lookup"><span data-stu-id="1408a-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1408a-158">操作状态。</span><span class="sxs-lookup"><span data-stu-id="1408a-158">Action state.</span></span> <span data-ttu-id="1408a-159">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="1408a-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1408a-160">关系</span><span class="sxs-lookup"><span data-stu-id="1408a-160">Relationships</span></span>
<span data-ttu-id="1408a-161">无</span><span class="sxs-lookup"><span data-stu-id="1408a-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1408a-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1408a-162">JSON Representation</span></span>
<span data-ttu-id="1408a-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1408a-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```





