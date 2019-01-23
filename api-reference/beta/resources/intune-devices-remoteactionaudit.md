---
title: remoteActionAudit 资源类型
description: 属于某些租户的设备上启动远程操作的报告。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404909"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="f2235-103">remoteActionAudit 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2235-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="f2235-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f2235-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2235-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2235-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2235-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2235-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2235-107">属于某些租户的设备上启动远程操作的报告。</span><span class="sxs-lookup"><span data-stu-id="f2235-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="f2235-108">方法</span><span class="sxs-lookup"><span data-stu-id="f2235-108">Methods</span></span>
|<span data-ttu-id="f2235-109">方法</span><span class="sxs-lookup"><span data-stu-id="f2235-109">Method</span></span>|<span data-ttu-id="f2235-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2235-110">Return Type</span></span>|<span data-ttu-id="f2235-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2235-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2235-112">列表 remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="f2235-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="f2235-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="f2235-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="f2235-114">列出属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="f2235-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="f2235-115">获取 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="f2235-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f2235-117">读取属性和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f2235-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="f2235-118">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="f2235-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f2235-120">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2235-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="f2235-121">删除 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="f2235-122">无</span><span class="sxs-lookup"><span data-stu-id="f2235-122">None</span></span>|<span data-ttu-id="f2235-123">删除[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)。</span><span class="sxs-lookup"><span data-stu-id="f2235-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="f2235-124">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="f2235-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="f2235-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="f2235-126">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2235-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2235-127">属性</span><span class="sxs-lookup"><span data-stu-id="f2235-127">Properties</span></span>
|<span data-ttu-id="f2235-128">属性</span><span class="sxs-lookup"><span data-stu-id="f2235-128">Property</span></span>|<span data-ttu-id="f2235-129">类型</span><span class="sxs-lookup"><span data-stu-id="f2235-129">Type</span></span>|<span data-ttu-id="f2235-130">说明</span><span class="sxs-lookup"><span data-stu-id="f2235-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2235-131">id</span><span class="sxs-lookup"><span data-stu-id="f2235-131">id</span></span>|<span data-ttu-id="f2235-132">String</span><span class="sxs-lookup"><span data-stu-id="f2235-132">String</span></span>|<span data-ttu-id="f2235-133">报告 id。</span><span class="sxs-lookup"><span data-stu-id="f2235-133">Report Id.</span></span>|
|<span data-ttu-id="f2235-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2235-134">deviceDisplayName</span></span>|<span data-ttu-id="f2235-135">String</span><span class="sxs-lookup"><span data-stu-id="f2235-135">String</span></span>|<span data-ttu-id="f2235-136">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="f2235-136">Intune device name.</span></span>|
|<span data-ttu-id="f2235-137">userName</span><span class="sxs-lookup"><span data-stu-id="f2235-137">userName</span></span>|<span data-ttu-id="f2235-138">String</span><span class="sxs-lookup"><span data-stu-id="f2235-138">String</span></span>|<span data-ttu-id="f2235-139">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f2235-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="f2235-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2235-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="f2235-141">String</span><span class="sxs-lookup"><span data-stu-id="f2235-141">String</span></span>|<span data-ttu-id="f2235-142">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="f2235-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="f2235-143">action</span><span class="sxs-lookup"><span data-stu-id="f2235-143">action</span></span>|[<span data-ttu-id="f2235-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="f2235-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="f2235-145">操作名称。</span><span class="sxs-lookup"><span data-stu-id="f2235-145">The action name.</span></span> <span data-ttu-id="f2235-146">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="f2235-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="f2235-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="f2235-147">requestDateTime</span></span>|<span data-ttu-id="f2235-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2235-148">DateTimeOffset</span></span>|<span data-ttu-id="f2235-149">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f2235-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="f2235-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2235-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="f2235-151">String</span><span class="sxs-lookup"><span data-stu-id="f2235-151">String</span></span>|<span data-ttu-id="f2235-152">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="f2235-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="f2235-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="f2235-153">deviceIMEI</span></span>|<span data-ttu-id="f2235-154">String</span><span class="sxs-lookup"><span data-stu-id="f2235-154">String</span></span>|<span data-ttu-id="f2235-155">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="f2235-155">IMEI of the device.</span></span>|
|<span data-ttu-id="f2235-156">actionState</span><span class="sxs-lookup"><span data-stu-id="f2235-156">actionState</span></span>|[<span data-ttu-id="f2235-157">actionState</span><span class="sxs-lookup"><span data-stu-id="f2235-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f2235-158">操作状态。</span><span class="sxs-lookup"><span data-stu-id="f2235-158">Action state.</span></span> <span data-ttu-id="f2235-159">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="f2235-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2235-160">关系</span><span class="sxs-lookup"><span data-stu-id="f2235-160">Relationships</span></span>
<span data-ttu-id="f2235-161">无</span><span class="sxs-lookup"><span data-stu-id="f2235-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2235-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2235-162">JSON Representation</span></span>
<span data-ttu-id="f2235-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2235-163">Here is a JSON representation of the resource.</span></span>
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




