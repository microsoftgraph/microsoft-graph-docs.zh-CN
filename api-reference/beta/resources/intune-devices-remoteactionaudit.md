---
title: remoteActionAudit 资源类型
description: 在属于某个租户的设备上启动的远程操作的报告。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f0e2efd04cbb2fff10ac51b463438d758b59006c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528502"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="c9543-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9543-103">remoteActionAudit resource type</span></span>

<span data-ttu-id="c9543-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c9543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9543-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9543-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9543-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9543-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9543-107">在属于某个租户的设备上启动的远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="c9543-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="c9543-108">方法</span><span class="sxs-lookup"><span data-stu-id="c9543-108">Methods</span></span>
|<span data-ttu-id="c9543-109">方法</span><span class="sxs-lookup"><span data-stu-id="c9543-109">Method</span></span>|<span data-ttu-id="c9543-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9543-110">Return Type</span></span>|<span data-ttu-id="c9543-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9543-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9543-112">列出 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="c9543-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="c9543-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9543-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="c9543-114">列出[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9543-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="c9543-115">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="c9543-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="c9543-117">读取[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9543-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="c9543-118">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="c9543-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="c9543-120">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9543-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="c9543-121">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="c9543-122">无</span><span class="sxs-lookup"><span data-stu-id="c9543-122">None</span></span>|<span data-ttu-id="c9543-123">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="c9543-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="c9543-124">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="c9543-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c9543-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="c9543-126">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9543-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9543-127">属性</span><span class="sxs-lookup"><span data-stu-id="c9543-127">Properties</span></span>
|<span data-ttu-id="c9543-128">属性</span><span class="sxs-lookup"><span data-stu-id="c9543-128">Property</span></span>|<span data-ttu-id="c9543-129">类型</span><span class="sxs-lookup"><span data-stu-id="c9543-129">Type</span></span>|<span data-ttu-id="c9543-130">说明</span><span class="sxs-lookup"><span data-stu-id="c9543-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9543-131">id</span><span class="sxs-lookup"><span data-stu-id="c9543-131">id</span></span>|<span data-ttu-id="c9543-132">String</span><span class="sxs-lookup"><span data-stu-id="c9543-132">String</span></span>|<span data-ttu-id="c9543-133">报告 Id。</span><span class="sxs-lookup"><span data-stu-id="c9543-133">Report Id.</span></span>|
|<span data-ttu-id="c9543-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c9543-134">deviceDisplayName</span></span>|<span data-ttu-id="c9543-135">String</span><span class="sxs-lookup"><span data-stu-id="c9543-135">String</span></span>|<span data-ttu-id="c9543-136">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="c9543-136">Intune device name.</span></span>|
|<span data-ttu-id="c9543-137">userName</span><span class="sxs-lookup"><span data-stu-id="c9543-137">userName</span></span>|<span data-ttu-id="c9543-138">String</span><span class="sxs-lookup"><span data-stu-id="c9543-138">String</span></span>|<span data-ttu-id="c9543-139">\[弃用\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="c9543-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="c9543-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9543-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="c9543-141">String</span><span class="sxs-lookup"><span data-stu-id="c9543-141">String</span></span>|<span data-ttu-id="c9543-142">启动设备操作的用户的格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="c9543-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="c9543-143">action</span><span class="sxs-lookup"><span data-stu-id="c9543-143">action</span></span>|[<span data-ttu-id="c9543-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="c9543-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="c9543-145">操作名称。</span><span class="sxs-lookup"><span data-stu-id="c9543-145">The action name.</span></span> <span data-ttu-id="c9543-146">可能的值为`unknown`： `factoryReset`、 `removeCompanyData`、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `getFileVaultKey` `setDeviceName`、、、、、、、、、、、、、、、、、、、、。 `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey`</span><span class="sxs-lookup"><span data-stu-id="c9543-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="c9543-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="c9543-147">requestDateTime</span></span>|<span data-ttu-id="c9543-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9543-148">DateTimeOffset</span></span>|<span data-ttu-id="c9543-149">发出操作的时间，以 UTC 表示。</span><span class="sxs-lookup"><span data-stu-id="c9543-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="c9543-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9543-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="c9543-151">String</span><span class="sxs-lookup"><span data-stu-id="c9543-151">String</span></span>|<span data-ttu-id="c9543-152">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="c9543-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="c9543-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="c9543-153">deviceIMEI</span></span>|<span data-ttu-id="c9543-154">String</span><span class="sxs-lookup"><span data-stu-id="c9543-154">String</span></span>|<span data-ttu-id="c9543-155">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="c9543-155">IMEI of the device.</span></span>|
|<span data-ttu-id="c9543-156">actionState</span><span class="sxs-lookup"><span data-stu-id="c9543-156">actionState</span></span>|[<span data-ttu-id="c9543-157">actionState</span><span class="sxs-lookup"><span data-stu-id="c9543-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c9543-158">动作状态。</span><span class="sxs-lookup"><span data-stu-id="c9543-158">Action state.</span></span> <span data-ttu-id="c9543-159">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c9543-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c9543-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c9543-160">managedDeviceId</span></span>|<span data-ttu-id="c9543-161">String</span><span class="sxs-lookup"><span data-stu-id="c9543-161">String</span></span>|<span data-ttu-id="c9543-162">操作目标。</span><span class="sxs-lookup"><span data-stu-id="c9543-162">Action target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9543-163">关系</span><span class="sxs-lookup"><span data-stu-id="c9543-163">Relationships</span></span>
<span data-ttu-id="c9543-164">无</span><span class="sxs-lookup"><span data-stu-id="c9543-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9543-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9543-165">JSON Representation</span></span>
<span data-ttu-id="c9543-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9543-166">Here is a JSON representation of the resource.</span></span>
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
  "actionState": "String",
  "managedDeviceId": "String"
}
```



