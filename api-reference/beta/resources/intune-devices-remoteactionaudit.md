---
title: remoteActionAudit 资源类型
description: 在属于某个租户的设备上启动的远程操作的报告。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a4a95019db6ca3025d0090981ca6563d335ffe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526256"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="fa80f-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa80f-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="fa80f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa80f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa80f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa80f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa80f-106">在属于某个租户的设备上启动的远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="fa80f-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="fa80f-107">方法</span><span class="sxs-lookup"><span data-stu-id="fa80f-107">Methods</span></span>
|<span data-ttu-id="fa80f-108">方法</span><span class="sxs-lookup"><span data-stu-id="fa80f-108">Method</span></span>|<span data-ttu-id="fa80f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fa80f-109">Return Type</span></span>|<span data-ttu-id="fa80f-110">说明</span><span class="sxs-lookup"><span data-stu-id="fa80f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa80f-111">列出 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="fa80f-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="fa80f-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="fa80f-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="fa80f-113">列出[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa80f-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="fa80f-114">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="fa80f-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="fa80f-116">读取[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa80f-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="fa80f-117">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="fa80f-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="fa80f-119">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa80f-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="fa80f-120">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="fa80f-121">无</span><span class="sxs-lookup"><span data-stu-id="fa80f-121">None</span></span>|<span data-ttu-id="fa80f-122">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="fa80f-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="fa80f-123">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="fa80f-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="fa80f-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="fa80f-125">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa80f-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa80f-126">属性</span><span class="sxs-lookup"><span data-stu-id="fa80f-126">Properties</span></span>
|<span data-ttu-id="fa80f-127">属性</span><span class="sxs-lookup"><span data-stu-id="fa80f-127">Property</span></span>|<span data-ttu-id="fa80f-128">类型</span><span class="sxs-lookup"><span data-stu-id="fa80f-128">Type</span></span>|<span data-ttu-id="fa80f-129">说明</span><span class="sxs-lookup"><span data-stu-id="fa80f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa80f-130">id</span><span class="sxs-lookup"><span data-stu-id="fa80f-130">id</span></span>|<span data-ttu-id="fa80f-131">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-131">String</span></span>|<span data-ttu-id="fa80f-132">报告 Id。</span><span class="sxs-lookup"><span data-stu-id="fa80f-132">Report Id.</span></span>|
|<span data-ttu-id="fa80f-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fa80f-133">deviceDisplayName</span></span>|<span data-ttu-id="fa80f-134">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-134">String</span></span>|<span data-ttu-id="fa80f-135">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="fa80f-135">Intune device name.</span></span>|
|<span data-ttu-id="fa80f-136">userName</span><span class="sxs-lookup"><span data-stu-id="fa80f-136">userName</span></span>|<span data-ttu-id="fa80f-137">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-137">String</span></span>|<span data-ttu-id="fa80f-138">\[弃用\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fa80f-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="fa80f-139">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa80f-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="fa80f-140">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-140">String</span></span>|<span data-ttu-id="fa80f-141">启动设备操作的用户的格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="fa80f-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="fa80f-142">action</span><span class="sxs-lookup"><span data-stu-id="fa80f-142">action</span></span>|[<span data-ttu-id="fa80f-143">remoteAction</span><span class="sxs-lookup"><span data-stu-id="fa80f-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="fa80f-144">操作名称。</span><span class="sxs-lookup"><span data-stu-id="fa80f-144">The action name.</span></span> <span data-ttu-id="fa80f-145">可能的值为`unknown`: `factoryReset`、 `removeCompanyData`、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan`、、、、、、、、、、、、、、、、 `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="fa80f-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="fa80f-146">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="fa80f-146">requestDateTime</span></span>|<span data-ttu-id="fa80f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa80f-147">DateTimeOffset</span></span>|<span data-ttu-id="fa80f-148">发出操作的时间, 以 UTC 表示。</span><span class="sxs-lookup"><span data-stu-id="fa80f-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="fa80f-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa80f-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="fa80f-150">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-150">String</span></span>|<span data-ttu-id="fa80f-151">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="fa80f-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="fa80f-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="fa80f-152">deviceIMEI</span></span>|<span data-ttu-id="fa80f-153">String</span><span class="sxs-lookup"><span data-stu-id="fa80f-153">String</span></span>|<span data-ttu-id="fa80f-154">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="fa80f-154">IMEI of the device.</span></span>|
|<span data-ttu-id="fa80f-155">actionState</span><span class="sxs-lookup"><span data-stu-id="fa80f-155">actionState</span></span>|[<span data-ttu-id="fa80f-156">actionState</span><span class="sxs-lookup"><span data-stu-id="fa80f-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fa80f-157">动作状态。</span><span class="sxs-lookup"><span data-stu-id="fa80f-157">Action state.</span></span> <span data-ttu-id="fa80f-158">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="fa80f-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa80f-159">关系</span><span class="sxs-lookup"><span data-stu-id="fa80f-159">Relationships</span></span>
<span data-ttu-id="fa80f-160">无</span><span class="sxs-lookup"><span data-stu-id="fa80f-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa80f-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa80f-161">JSON Representation</span></span>
<span data-ttu-id="fa80f-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa80f-162">Here is a JSON representation of the resource.</span></span>
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





