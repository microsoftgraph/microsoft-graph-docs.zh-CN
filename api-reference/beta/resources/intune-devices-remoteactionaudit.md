---
title: remoteActionAudit 资源类型
description: 属于某些租户的设备上启动远程操作的报告。
ms.openlocfilehash: 9183330971e5c624d1e88532e4ea2c16691875da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047567"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="b3e1b-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3e1b-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="b3e1b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3e1b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3e1b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3e1b-107">属于某些租户的设备上启动远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="b3e1b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b3e1b-108">Methods</span></span>
|<span data-ttu-id="b3e1b-109">方法</span><span class="sxs-lookup"><span data-stu-id="b3e1b-109">Method</span></span>|<span data-ttu-id="b3e1b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3e1b-110">Return Type</span></span>|<span data-ttu-id="b3e1b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3e1b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3e1b-112">列表 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="b3e1b-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="b3e1b-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3e1b-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="b3e1b-114">列出属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="b3e1b-115">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="b3e1b-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b3e1b-117">读取属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="b3e1b-118">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="b3e1b-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b3e1b-120">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="b3e1b-121">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="b3e1b-122">无</span><span class="sxs-lookup"><span data-stu-id="b3e1b-122">None</span></span>|<span data-ttu-id="b3e1b-123">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="b3e1b-124">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="b3e1b-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="b3e1b-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="b3e1b-126">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3e1b-127">属性</span><span class="sxs-lookup"><span data-stu-id="b3e1b-127">Properties</span></span>
|<span data-ttu-id="b3e1b-128">属性</span><span class="sxs-lookup"><span data-stu-id="b3e1b-128">Property</span></span>|<span data-ttu-id="b3e1b-129">类型</span><span class="sxs-lookup"><span data-stu-id="b3e1b-129">Type</span></span>|<span data-ttu-id="b3e1b-130">说明</span><span class="sxs-lookup"><span data-stu-id="b3e1b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e1b-131">id</span><span class="sxs-lookup"><span data-stu-id="b3e1b-131">id</span></span>|<span data-ttu-id="b3e1b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b3e1b-132">String</span></span>|<span data-ttu-id="b3e1b-133">报告 id。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-133">Report Id.</span></span>|
|<span data-ttu-id="b3e1b-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b3e1b-134">deviceDisplayName</span></span>|<span data-ttu-id="b3e1b-135">String</span><span class="sxs-lookup"><span data-stu-id="b3e1b-135">String</span></span>|<span data-ttu-id="b3e1b-136">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-136">Intune device name.</span></span>|
|<span data-ttu-id="b3e1b-137">userName</span><span class="sxs-lookup"><span data-stu-id="b3e1b-137">userName</span></span>|<span data-ttu-id="b3e1b-138">String</span><span class="sxs-lookup"><span data-stu-id="b3e1b-138">String</span></span>|<span data-ttu-id="b3e1b-139">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="b3e1b-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3e1b-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="b3e1b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b3e1b-141">String</span></span>|<span data-ttu-id="b3e1b-142">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="b3e1b-143">action</span><span class="sxs-lookup"><span data-stu-id="b3e1b-143">action</span></span>|[<span data-ttu-id="b3e1b-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="b3e1b-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="b3e1b-145">操作名称。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-145">The action name.</span></span> <span data-ttu-id="b3e1b-146">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="b3e1b-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="b3e1b-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e1b-147">requestDateTime</span></span>|<span data-ttu-id="b3e1b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3e1b-148">DateTimeOffset</span></span>|<span data-ttu-id="b3e1b-149">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="b3e1b-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3e1b-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="b3e1b-151">字符串</span><span class="sxs-lookup"><span data-stu-id="b3e1b-151">String</span></span>|<span data-ttu-id="b3e1b-152">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="b3e1b-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="b3e1b-153">deviceIMEI</span></span>|<span data-ttu-id="b3e1b-154">字符串</span><span class="sxs-lookup"><span data-stu-id="b3e1b-154">String</span></span>|<span data-ttu-id="b3e1b-155">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-155">IMEI of the device.</span></span>|
|<span data-ttu-id="b3e1b-156">actionState</span><span class="sxs-lookup"><span data-stu-id="b3e1b-156">actionState</span></span>|[<span data-ttu-id="b3e1b-157">actionState</span><span class="sxs-lookup"><span data-stu-id="b3e1b-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b3e1b-158">操作状态。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-158">Action state.</span></span> <span data-ttu-id="b3e1b-159">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3e1b-160">关系</span><span class="sxs-lookup"><span data-stu-id="b3e1b-160">Relationships</span></span>
<span data-ttu-id="b3e1b-161">无</span><span class="sxs-lookup"><span data-stu-id="b3e1b-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3e1b-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3e1b-162">JSON Representation</span></span>
<span data-ttu-id="b3e1b-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3e1b-163">Here is a JSON representation of the resource.</span></span>
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





