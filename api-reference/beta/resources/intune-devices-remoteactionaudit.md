---
title: remoteActionAudit 资源类型
description: 在属于特定租户的设备上启动的远程操作的报告。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d1d9e7a340db9cc176b2ebc11bfcb4e7bd5f8de
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611879"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="0032a-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="0032a-103">remoteActionAudit resource type</span></span>

<span data-ttu-id="0032a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0032a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0032a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0032a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0032a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0032a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0032a-107">在属于特定租户的设备上启动的远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="0032a-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="0032a-108">方法</span><span class="sxs-lookup"><span data-stu-id="0032a-108">Methods</span></span>
|<span data-ttu-id="0032a-109">方法</span><span class="sxs-lookup"><span data-stu-id="0032a-109">Method</span></span>|<span data-ttu-id="0032a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0032a-110">Return Type</span></span>|<span data-ttu-id="0032a-111">Description</span><span class="sxs-lookup"><span data-stu-id="0032a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0032a-112">列出 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="0032a-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="0032a-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0032a-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="0032a-114">列出 [remoteActionAudit 对象的属性和](../resources/intune-devices-remoteactionaudit.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0032a-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="0032a-115">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="0032a-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="0032a-117">读取 [remoteActionAudit 对象的属性和](../resources/intune-devices-remoteactionaudit.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0032a-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="0032a-118">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="0032a-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="0032a-120">创建新的 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0032a-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="0032a-121">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="0032a-122">无</span><span class="sxs-lookup"><span data-stu-id="0032a-122">None</span></span>|<span data-ttu-id="0032a-123">删除 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="0032a-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="0032a-124">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="0032a-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0032a-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="0032a-126">更新 [remoteActionAudit 对象](../resources/intune-devices-remoteactionaudit.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0032a-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0032a-127">属性</span><span class="sxs-lookup"><span data-stu-id="0032a-127">Properties</span></span>
|<span data-ttu-id="0032a-128">属性</span><span class="sxs-lookup"><span data-stu-id="0032a-128">Property</span></span>|<span data-ttu-id="0032a-129">类型</span><span class="sxs-lookup"><span data-stu-id="0032a-129">Type</span></span>|<span data-ttu-id="0032a-130">说明</span><span class="sxs-lookup"><span data-stu-id="0032a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0032a-131">id</span><span class="sxs-lookup"><span data-stu-id="0032a-131">id</span></span>|<span data-ttu-id="0032a-132">String</span><span class="sxs-lookup"><span data-stu-id="0032a-132">String</span></span>|<span data-ttu-id="0032a-133">报告 ID。</span><span class="sxs-lookup"><span data-stu-id="0032a-133">Report Id.</span></span>|
|<span data-ttu-id="0032a-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0032a-134">deviceDisplayName</span></span>|<span data-ttu-id="0032a-135">String</span><span class="sxs-lookup"><span data-stu-id="0032a-135">String</span></span>|<span data-ttu-id="0032a-136">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="0032a-136">Intune device name.</span></span>|
|<span data-ttu-id="0032a-137">userName</span><span class="sxs-lookup"><span data-stu-id="0032a-137">userName</span></span>|<span data-ttu-id="0032a-138">String</span><span class="sxs-lookup"><span data-stu-id="0032a-138">String</span></span>|<span data-ttu-id="0032a-139">\[已弃用 \] 请改为使用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="0032a-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="0032a-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0032a-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="0032a-141">String</span><span class="sxs-lookup"><span data-stu-id="0032a-141">String</span></span>|<span data-ttu-id="0032a-142">启动设备操作的用户，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="0032a-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="0032a-143">action</span><span class="sxs-lookup"><span data-stu-id="0032a-143">action</span></span>|[<span data-ttu-id="0032a-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="0032a-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="0032a-145">操作名称。</span><span class="sxs-lookup"><span data-stu-id="0032a-145">The action name.</span></span> <span data-ttu-id="0032a-146">可能的值是 `unknown` `factoryReset` `removeCompanyData` ：、、、、、、、、、、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` 。</span><span class="sxs-lookup"><span data-stu-id="0032a-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="0032a-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="0032a-147">requestDateTime</span></span>|<span data-ttu-id="0032a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0032a-148">DateTimeOffset</span></span>|<span data-ttu-id="0032a-149">发出操作的时间（以 UTC 表示）。</span><span class="sxs-lookup"><span data-stu-id="0032a-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="0032a-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0032a-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="0032a-151">String</span><span class="sxs-lookup"><span data-stu-id="0032a-151">String</span></span>|<span data-ttu-id="0032a-152">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="0032a-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="0032a-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="0032a-153">deviceIMEI</span></span>|<span data-ttu-id="0032a-154">String</span><span class="sxs-lookup"><span data-stu-id="0032a-154">String</span></span>|<span data-ttu-id="0032a-155">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="0032a-155">IMEI of the device.</span></span>|
|<span data-ttu-id="0032a-156">actionState</span><span class="sxs-lookup"><span data-stu-id="0032a-156">actionState</span></span>|[<span data-ttu-id="0032a-157">actionState</span><span class="sxs-lookup"><span data-stu-id="0032a-157">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="0032a-158">操作状态。</span><span class="sxs-lookup"><span data-stu-id="0032a-158">Action state.</span></span> <span data-ttu-id="0032a-159">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0032a-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0032a-160">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0032a-160">managedDeviceId</span></span>|<span data-ttu-id="0032a-161">String</span><span class="sxs-lookup"><span data-stu-id="0032a-161">String</span></span>|<span data-ttu-id="0032a-162">操作目标。</span><span class="sxs-lookup"><span data-stu-id="0032a-162">Action target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0032a-163">关系</span><span class="sxs-lookup"><span data-stu-id="0032a-163">Relationships</span></span>
<span data-ttu-id="0032a-164">无</span><span class="sxs-lookup"><span data-stu-id="0032a-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0032a-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0032a-165">JSON Representation</span></span>
<span data-ttu-id="0032a-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0032a-166">Here is a JSON representation of the resource.</span></span>
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




